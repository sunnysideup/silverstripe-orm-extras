# Silverstripe orm-extras module
[![Build Status](https://travis-ci.org/sunnysideup/silverstripe-orm-extras.svg?branch=master)](https://travis-ci.org/sunnysideup/silverstripe-orm-extras)
[![Scrutinizer Code Quality](https://scrutinizer-ci.com/g/sunnysideup/silverstripe-orm-extras/badges/quality-score.png?b=master)](https://scrutinizer-ci.com/g/sunnysideup/silverstripe-orm-extras/?branch=master)
[![codecov.io](https://codecov.io/github/sunnysideup/silverstripe-orm-extras/coverage.svg?branch=master)](https://codecov.io/github/sunnysideup/silverstripe-orm-extras?branch=master)

[![Latest Stable Version](https://poser.pugx.org/sunnysideup/orm-extras/version)](https://packagist.org/packages/sunnysideup/orm-extras)
[![License](https://poser.pugx.org/sunnysideup/orm-extras/license)](https://packagist.org/packages/sunnysideup/orm-extras)
[![Monthly Downloads](https://poser.pugx.org/sunnysideup/orm-extras/d/monthly)](https://packagist.org/packages/sunnysideup/orm-extras)

# TL;DR

## filter without worrying about empty arrays

```php
$filterSafeArray = ArraMethods::filter_array([]);
$list = MyDataObject::get()->filter($filterSafeArray);
```

## sort by any id sequence

```php
$sortByStatement = ArraMethods::create_sort_statement_from_id_array([44,222,434,22,]);
$sortedList = MyDataObject::get()->sort($sortByStatement);

```


## Documentation

 * [Developer Docs](docs/en/INDEX.md)
 * [User Guide](docs/en/userguide.md)
 * [API Docs](http://docs.ssmods.com/sunnysideup/orm-extras/classes.xhtml)


## Requirements



See [composer.json](composer.json) for details


### Suggested Modules



See [composer.json](composer.json) for details


## Installation


```
composer require sunnysideup/orm-extras
```

### Configuration



In the `_config` folder you will find the `orm-extras.yml.example`
file that shows options for the configuration of this module.

We recommend that you:

  1. copy these `orm-extras.yml.example` files into your
`app/_config` folder (where available - otherwise search for `private static $` in the module to see what can be configured)
  2. remove the .example extension,
  3. delete the lines you do not care about, and
  4. adjust the configurations that you would like to use.


## Contributing



We welcome any contributions. See [CONTRIBUTING.md](CONTRIBUTING.md) for more details.

## Paid assistance



You can pay us to create an improved / adapted version of this module for your own projects.  Please contact us if you like to find out more: [www.sunnysideup.co.nz](http://www.sunnysideup.co.nz).  For example, we can write tests for this module.  

## Author



Sunny Side Up Ltd.


## Care to see more modules?

To find other modules, please visit [ssmods.com](http://ssmods.com/).
