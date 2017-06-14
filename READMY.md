# http://sypex.net/ API PHP

###Sypex Geo is released under the terms of the BSD license                  |
###http://sypex.net/bsd_license.txt 

##Download BD sxgeocity.dat
###http://sypexgeo.net/ru/download/

## Installation

The recommended installation way is through [Composer](https://getcomposer.org).

```sh
$ composer require klev/sypex-geo
```
Change the configuration file

    config/config.php


## Usage:
Two API methods
 - №1 - BD sxgeocity.dat
 - №2 - REST API http://sypexgeo.net/ru/api/

## Metod JSON:
Class SxGeo

    src/sxgeo.php
    
bd

    src/sxgeocity.dat


Example: 

    require(__DIR__ . "/../vendor/autoload.php");
    $SxGeo = new SxGeo();
    $ip = $_SERVER['REMOTE_ADDR'];
    var_damp($SxGeo->get($ip));
    
