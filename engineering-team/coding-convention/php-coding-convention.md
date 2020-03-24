# PHP Coding Convention

## Goal

Sebuah kesepakatan untuk menstandardisasikan _coding_ PHP.

## Intro

_We are not reinventing the wheels._ Rolling Glory mengadopsi [PSR \(PHP Standard Recommendation\)](https://www.php-fig.org/psr/), sebuah standard dalam _coding_ PHP yang dibuat oleh sebuah konsorsium  bernama [PHP-FIG](https://www.php-fig.org/). Framework PHP yang banyak digunakan di Rolling Glory adalah [Yii Framework](https://www.yiiframework.com/) dan [Laravel](https://laravel.com/), dan keduanya merupakan anggota dari PHP-FIG.

Dalam document ini, akan dituliskan ulang beberapa guideline yang akan sering digunakan terutama dari [PSR-1 Basic Coding Standard](https://www.php-fig.org/psr/psr-12/) dan [PSR-12 Extended Coding Style](https://www.php-fig.org/psr/psr-12/). Untuk lengkapnya silakan baca di link ke [PSR](https://www.php-fig.org/psr/#numerical-index) yang lengkap.

## References

### PSR-1 Basic Coding Standard

#### [Overview](https://www.php-fig.org/psr/psr-1/#1-overview)

Files MUST use only `<?php` and `<?=` tags.

Files MUST use only UTF-8 without BOM for PHP code.

Class names MUST be declared in `StudlyCaps`

Class constants MUST be declared in all upper case with underscore separators.

Method names MUST be declared in `camelCase`.

### PSR-12 Extended Coding Style

#### [General](https://www.php-fig.org/psr/psr-12/#2-general)

All PHP files MUST use the Unix LF \(linefeed\) line ending only.

All PHP files MUST end with a non-blank line, terminated with a single LF.

The closing `?>` tag MUST be omitted from files containing only PHP.

There MUST NOT be a hard limit on line length.

The soft limit on line length MUST be 120 characters.

Lines SHOULD NOT be longer than 80 characters; lines longer than that SHOULD be split into multiple subsequent lines of no more than 80 characters each.

There MUST NOT be trailing whitespace at the end of lines.

Blank lines MAY be added to improve readability and to indicate related blocks of code except where explicitly forbidden.

There MUST NOT be more than one statement per line.

Code MUST use an indent of 4 spaces for each indent level, and MUST NOT use tabs for indenting.

Short form of type keywords MUST be used i.e. `bool` instead of `boolean`, `int` instead of `integer` etc.

#### [Classess, Properties, and Methods](https://www.php-fig.org/psr/psr-12/#4-classes-properties-and-methods)

Any closing brace MUST NOT be followed by any comment or statement on the same line.

When instantiating a new class, parentheses MUST always be present even when there are no arguments passed to the constructor.

```php
new Foo();
```

The `extends` and `implements` keywords MUST be declared on the same line as the class name.

The opening brace for the class MUST go on its own line; the closing brace for the class MUST go on the next line after the body.

Opening braces MUST be on their own line and MUST NOT be preceded or followed by a blank line.

Closing braces MUST be on their own line and MUST NOT be preceded by a blank line.

```php
class ClassName extends ParentClass implements \ArrayAccess, \Countable
{
    // constants, properties, methods
}
```

Visibility MUST be declared on all properties.

Visibility MUST be declared on all constants if your project PHP minimum version supports constant visibilities \(PHP 7.1 or later\).

The `var` keyword MUST NOT be used to declare a property.

There MUST NOT be more than one property declared per statement.

Property names MUST NOT be prefixed with a single underscore to indicate protected or private visibility. That is, an underscore prefix explicitly has no meaning.

```php
class ClassName
{
    public $foo = null;
    public static int $bar = 0;
}
```

A method declaration looks like the following. Note the placement of parentheses, commas, spaces, and braces:

```php
class ClassName
{
    public function fooBarBaz($arg1, &$arg2, $arg3 = [])
    {
        // method body
    }
}
```

When present, the `abstract` and `final` declarations MUST precede the visibility declaration.

When present, the `static` declaration MUST come after the visibility declaration.

When making a method or function call, there MUST NOT be a space between the method or function name and the opening parenthesis, there MUST NOT be a space after the opening parenthesis, and there MUST NOT be a space before the closing parenthesis. In the argument list, there MUST NOT be a space before each comma, and there MUST be one space after each comma.

```php
bar();
$foo->bar($arg1);
Foo::bar($arg2, $arg3);

$foo->bar(
    $longArgument,
    $longerArgument,
    $muchLongerArgument
);
```

#### [Control Structures](https://www.php-fig.org/psr/psr-12/#5-control-structures)

The general style rules for control structures are as follows:

* There MUST be one space after the control structure keyword
* There MUST NOT be a space after the opening parenthesis
* There MUST NOT be a space before the closing parenthesis
* There MUST be one space between the closing parenthesis and the opening brace
* The structure body MUST be indented once
* The body MUST be on the next line after the opening brace
* The closing brace MUST be on the next line after the body

The body of each structure MUST be enclosed by braces. This standardizes how the structures look and reduces the likelihood of introducing errors as new lines get added to the body.

```php
if ($expr1) {
    // if body
} elseif (
    $expr2
    && $expr3
) {
    // elseif body
} else {
    // else body;
}

for ($i = 0; $i < 10; $i++) {
    // for body
}

foreach ($iterable as $key => $value) {
    // foreach body
}

$variable = $foo ? 'foo' : 'bar';
```



