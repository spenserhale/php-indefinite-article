# PHP Indefinite Article Library

PHP implementation of the [Lingua::EN::Inflect](http://search.cpan.org/dist/Lingua-EN-Inflect/lib/Lingua/EN/Inflect.pm) 
Perl module's A() and AN() subroutines, 
originally [ported to PHP](https://github.com/Kaivosukeltaja/php-indefinite-article) by [Niko Salminen](http://nikosalminen.com),
and then by [make into composer package](https://github.com/zachflower/php-indefinite-article) by [Zach Flower](https://zacharyflower.com/).

## Installation

### Via Composer

Require the library and update via [Composer](https://getcomposer.org/):

```
composer require spenserhale/indefinite-article
composer update
```

### Manually

Download the [latest release](https://github.com/spenserhale/php-indefinite-article/archive/master.zip), extract into a directory called `indefinite-article`, and include the library at the beginning of your script:

```
include_once('./indefinite-articles/src/IndefiniteArticle.php');
use \IndefiniteArticle\IndefiniteArticle;
```

## Usage

The PHP Indefinite Article Library is used to determine the proper indefinite article to use before a word ('a' or 'an'). To do so, simply call the `A()` method with your word or phrase:

```
IndefiniteArticle::A('elephant')
```

The method will return a string prefixed with the appropriate indefinite article:

```
an elephant
```

## Copyright and License

Original Perl module Copyright &copy; 1997-2009 Damian Conway; Original PHP port Copyright &copy; 2012 Niko Salminen; Original library copyright &copy; 2016 Zachary Flower; Current library copyright &copy; 2018 Spenser Hale; Code released under the [BSD license](LICENSE).
