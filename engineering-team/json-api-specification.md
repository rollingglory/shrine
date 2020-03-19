# JSON API Specification

## Goal

Goal of this document is standardize: 1. how a client should request that resources be fetched or modified 1. how a server should respond to those requests, how JSON response from REST API should be formatted

Example

```text
{
  "data": {
    "type": "articles",
    "id": "1",
    "attributes": {
      "title": "JSON API Specification",
      "body": "Goal of this document is standardize how a client should request that resources be fetched or modified
and how a server should respond to those requests, how JSON response from REST API should be formatted",
      "createdAt": "2015-05-22T14:56:29.000Z",
      "updatedAt": "2015-05-22T14:56:28.000Z"
    }
  }
}
```

## References

We are not reinventing the wheels. We adopt \(_partially, just the basic and appropriate for our work_\) from [jsonapi.org](http://jsonapi.org).

This document will rewrite selected specification we adopt, and some of it will be adjusted for our needs.

## Table of Contents

1. Media Type Contract
2. Top Level
3. Primary Data
4. Resource Objects
5. Naming Conventions
6. Data Operations
7. Response Code and Message
8. Errors

## Media Type

JSON:API requires use of the JSON:API media type `application/vnd.api+json` for exchanging data.

Clients MUST send all JSON:API data in request documents with the header `Content-Type: application/vnd.api+json` without any media type parameters.

Servers MUST send all JSON:API data in response documents with the header `Content-Type: application/vnd.api+json` without any media type parameters.

## Top Level

A JSON object MUST be at the root

Contain at least one of the following top-level members: 1. **data**: “primary data” 1. **errors**: an array of error objects 1. **meta**: contains non-standard meta-information

Data and errors MUST NOT coexist in the same document

## Primary Data

Primary data MUST be either: 1. **a single resource object**, or null _for requests that target single resources_ 1. **an array of resource objects**, or an empty array \(\[\]\), _for requests that target resource collections_

## Resource Objects

MUST contain at least the following top-level members: **id** and **type**

The values of the id and type members MUST be **strings**

Each resource object’s type and id pair MUST identify a single, unique resource.

```text
{
  "data": {
    "type": "articles",
    "id": "1"
  }
}
```

## Naming Conventions

Property naming conventions is same with what defined on [AirBnb Javascript Style Guide](https://github.com/airbnb/javascript/blob/master/README.md#naming-conventions).

* Use camelCase when naming properties
* Do not use trailing or leading underscores

## Data Operations

Data, including resources and relationships, can be fetched by sending a GET request to an endpoint.

A server MUST support fetching resource data for every URL provided as:

1. a self link as part of the top-level links object
2. a self link as part of a resource-level links object
3. a related link as part of a relationship-level links object

The HTTP protocol define a set of operations that can be executed on a single or multiple resources

| HTTP Method | Link | Server method |  |
| :--- | :--- | :--- | :--- |
| GET | /articles | articles.find\(\) | reads a list of resources |
| GET | /articles/1 | articles.get\(1\) | reads a single resource |
| GET | /articles/1/authors | articles.get\(1\).authors | reads a single resource's relationship |
| POST | /articles | articles.create\(body\) | create a new resource |
| PUT | /articles/1 | articles.update\(1, body\) | completely replaces the resource\(s\) |
| PATCH | /articles/1 | articles.patch\(1, body\) | merges the resource\(s\) data |
| DELETE | /articles/1 | articles.remove\(1, body\) | deletes the resource\(s\) |

### Fetching

#### Sorting

A server MAY choose to support requests to sort resource collections according to one or more criteria \(“sort fields”\).

With a **sort** query parameter

The value for sort MUST represent sort fields

Support **multiple sort** fields by allowing **comma-separated**

Sort order for each sort field MUST be **ascending**

Unless it is prefixed with a minus “-“, in which case it MUST be descending

`GET /people?sort=name HTTP/1.1`

`GET /articles?sort=-created,title HTTP/1.1`

#### Pagination

Pagination links MUST appear in the links object that corresponds to a collection.

The following keys MUST be used for pagination links:

* `first`: the first page of data
* `last`: the last page of data
* `prev`: the previous page of data
* `next`: the next page of data

`GET /articles?page[number]=3&page[size]=1 HTTP/1.1`

```text
{
  "meta": {
    "totalPages": 13
  },
  "data": [
    {
      "type": "articles",
      "id": "3",
      "attributes": {
        "title": "JSON:API paints my bikeshed!",
        "body": "The shortest article. Ever.",
      }
    }
  ],
  "links": {
    "first": "http://example.com/articles?page[number]=1&page[size]=1",
    "prev": "http://example.com/articles?page[number]=2&page[size]=1",
    "next": "http://example.com/articles?page[number]=4&page[size]=1",
    "last": "http://example.com/articles?page[number]=13&page[size]=1"
  }
}
```

#### Filtering

The **filter** query parameter is reserved for filtering data.

### Creating, Updating, Deleting

A request MUST completely succeed or fail \(in a single “transaction”\). No partial updates are allowed.

The PATCH request MUST include a single resource object as primary data. The resource object MUST contain type and id members.

## Response Code and Message

_TO DO_

## Errors

Error objects MUST be returned as an array keyed by errors in the top level of a JSON:API document.

An error object MAY have the following members:

* id: a unique identifier for this particular occurrence of the problem.
* status: the HTTP status code applicable to this problem, expressed as a string value.
* code: an application-specific error code, expressed as a string value.
* title: a short, human-readable summary of the problem that SHOULD NOT change from occurrence to occurrence of the problem, except for purposes of localization.
* detail: a human-readable explanation specific to this occurrence of the problem. Like title, this field’s value can be localized.

```text
{
  "errors": [
    {    
      "status": "422",
      "code": "InvalidAttribute",
      "title":  "Invalid Attribute",
      "detail": "First name must contain at least three characters."
    }    
  ]
}
```

