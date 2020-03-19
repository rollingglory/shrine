# Git Commit Best Practice

## Table of Contents

1. Writing Good Commit Messages
2. When To Commit

## Writing Good Commit Messages

Commit message contains

**subject line**: tell briefly what changes have been done

**body message**: optional part to give more explanation about the commit

### 1. Imperative Subject

Write a subject line in an imperative form \(bentuk aktif dalam bahasa Indonesia\)

Commit messages have to complete this sentence:

> "If applied, this commit will **\_**"

or

> "Jika ditambahkan, commit ini akan **\_**"

Examples

* _If applied, this commit will_ `Add login page layout`
* _If applied, this commit will_ `Remove deprecated methods`
* _If applied, this commit will_ `Fix a bug where app will crash when user login for the second time`
* _If applied, this commit will_ `Fix a bug on the login page`
* _If applied, this commit will_ `Release version 1.0.0`
* _Jika ditambahkan, commit ini akan_ `Memperbaiki bug pada halaman dashboard`
* _Jika ditambahkan, commit ini akan_ `Menambahkan grafik pada halaman dashboard`

### 2. Limit Subject chars to 72

### 3. Separate **subject** and **body** with exactly 1 line

```text
Update chat mechanism

- resend pending image
- add upload progress percentage
- cache 24 hours of data
```

```text
Fix bug out of memory pada logger

Pada versi sebelumnya log dibuat dengan meng-append ke dalam object String. 
Hal tersebut bisa mengakibatkan OOM karena melebihi kapasitas penyimpanan String. 
Untuk menghindari hal tersebut, setiap log disimpan secara terpisah ke dalam database 
lalu akan digabungkan di dalam satu file di akhir proses.
```

### 4. Use body message to explain "what" or "why" instead of "how"

Your code should tell the story better

Do

```text
Pada versi sebelumnya log dibuat dengan meng-append ke dalam object String. 
Hal tersebut bisa mengakibatkan OOM karena melebihi kapasitas penyimpanan String. 
Untuk menghindari hal tersebut, setiap log disimpan secara terpisah ke dalam database 
lalu akan digabungkan di dalam satu file di akhir proses.
```

Don't

```text
Penulisan log dilakukan dengan mengiterasi setiap item di dalam database. 
Setiap item akan ditulis ke dalam file di dalam folder temporary. 
Jika sebelumnya sudah ada file dengan nama yang sama, tulis ulang file tersebut. 
Setelah semua proses sudah beres, semua item dihapus dari database.
```

### 5. Capitalize the first char in subject

### 6. Don't use a period \(.\) at the end of the subject

### 7. Don't use emoji in your commit message

`git gak dipake buat chattingan mas parkun`  _~ some dev ops engineer to some front end developer, circa 2019_

## When to Commit

Partially refers to [this link](https://www.git-tower.com/blog/version-control-best-practices/)

**Atomic and granular** commits make it easier for developers to understand the changes and roll them back if something went wrong. With tools like the staging area and the ability to stage only parts of a file, Git makes it easy to create very granular commits.

### 1. Commit often for every task

The task is a part of a feature which is standalone and can be tested

```text
Task fitur login

layout code
validasi input
handle API
```

### 2. Don't commit half-done work

### 3. Separate commit of bug fixes and feature addition or updates

### 4. Test before you commit

