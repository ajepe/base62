## BASE62
Base is a small package that  encode integer as a string and decode the string back to an integer, this is can useful in making  URL shortening web application or generating unique URL. This package convert the id in decimal to base 62 with the encode method and convert it back to decimal with the decode public method.

* It converts non-negative integer number like _42000000_  up to _PHP\_INT\_SIZE_ of the platform in which the package is being use on into a string like _2Qe7m_. The action is reversible.
* It can also decode the id back from _2Qe7m_ to _42000000_.
* This is useful in youtube like url or simply using them making url shortening website.


### Install

Via Composer
``` bash
composer require ajepe/base62:*
```

### Usage

``` php
require 'vendor/autoload.php';


$encode = new Base\Encode();
$decode = new Base\Decode();
$encode = $encode->encode(PHP_INT_MAX); //return Z
$decode = $decode->decode($encode); // return 24815682095
printf('The encode value of %s map directly to %s', $encode, $decode);

```
[README.md](README.md), [CHANGELOG.md](CHANGELOG.md), [CONTRIBUTING.md](CONTRIBUTING.md), [LICENSE.txt](LICENSE) and [composer.json](composer.json)

## Change log

Please see [CHANGELOG](CHANGELOG.md) for more information what has changed recently.