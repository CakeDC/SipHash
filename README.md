SipHash  [![Build Status](https://travis-ci.org/duzun/SipHash.svg?branch=master)](https://travis-ci.org/duzun/SipHash)
==========

[SipHash-2-4](https://131002.net/siphash/) implementation written in PHP

# Install

### With [composer](https://getcomposer.org/)

```sh
composer require duzun/siphash
```

### Vanilla PHP (no composer)

Copy `src/SipHash.php` to your project, then

```php
require_once 'src/SipHash.php';
```


# Usage

```php
use duzun\SipHash; // PHP >= 5.3.0

// 128-bit $key is a string of max 16 chars
// $message is any string you want to hash
$hash = SipHash::hash_2_4($key, $message); // eg. "6dd48df68066d1bd"
```
