![Particle\Filter](https://cloud.githubusercontent.com/assets/6495166/7777918/406635e8-00c7-11e5-90e3-96c590828ffd.png)
===

[![Travis-CI](https://img.shields.io/travis/particle-php/Filter/master.svg)](https://travis-ci.org/particle-php/Filter)
[![Packagist](https://img.shields.io/packagist/v/particle/filter.svg)](https://packagist.org/packages/particle/filter)
[![Packagist downloads](https://img.shields.io/packagist/dt/particle/filter.svg)](https://packagist.org/packages/particle/filter)
[![Scrutinizer](https://img.shields.io/scrutinizer/g/particle-php/Filter.svg)](https://scrutinizer-ci.com/g/particle-php/Filter/?branch=master)
[![Scrutinizer](https://img.shields.io/scrutinizer/coverage/g/particle-php/Filter/master.svg)](https://scrutinizer-ci.com/g/particle-php/Filter/?branch=master)

*Particle\Filter* is a very small filtering library, with the easiest and most usable API we could possibly create.

## Small usage example

```php
$f = new Particle\Filter;

$f->value('first_name')->trim()->lower()->upperFirst();

$result = $f->filter([
    'first_name' => '  rick ',
]);

var_dump($result); // array(1) { ["first_name"]=> string(4) "Rick" }
```

## Features

* Filter an array of values
* Get a cleaned array after filtering

Included filters:

* trim
* lower
* upper
* upperFirst
* stripHtml
* replace
* regexReplace
* int
* bool
* string
* float
* camelCase
* underscore

===

Find more information and advanced usage examples at [filter.particle-php.com](http://filter.particle-php.com)
