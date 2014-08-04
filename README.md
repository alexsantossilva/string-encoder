String Encode
==========================

Version 0.1.2

String Encode is a simple PHP wrapper package to facilitate the encoding of strings in different charsets.

This is a fork of paquettg/string-encoder that supports PHP 5.3.
The original author has expressed his unwillingness to merge the changes necessary to make his package compatible with PHP 5.3. I created this fork to fix that.

Install
-------

This package can be found on [packagist](https://packagist.org/packages/brjpeters/string-encode) and is best loaded using [composer](http://getcomposer.org/).

Usage
-----

This is a really simple package so there is not much to say about it. The following is just about the only usage for this package at the moment.

```php
use stringEncode\Encode;

$str    = "Calendrier de l'avent façon Necta!"
$encode = new Encode;
$encode->detect($str);
$newstr = $encode->convert($str);
echo $newstr; // "Calendrier de l'avent façon Necta!" in UTF-8 encoding (default)
```

As you can see, it is a very simple encoding converter.
