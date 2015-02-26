# [laravel-disqus](http://roumen.it/projects/laravel-disqus) package

[![Latest Stable Version](https://poser.pugx.org/roumen/disqus/version.png)](https://packagist.org/packages/roumen/disqus) [![Total Downloads](https://poser.pugx.org/roumen/disqus/d/total.png)](https://packagist.org/packages/roumen/disqus)

A Laravel 5 package for Disqus API.

## Notes

Latest supported version for Laravel 4 is v0.1.1.3

Branch dev-master is for development and is unstable

## Installation

Run the following command and provide the latest stable version (e.g v1.1) :

```bash
composer require roumen/disqus
```

or add the following to your `composer.json` file :

```json
"roumen/disqus": "~1"
```

Then register this service provider with Laravel :

```php
'Roumen\Disqus\DisqusServiceProvider',
```

## Example

```php
$secret_key = 'YOUR_SECRET_KEY';

$disqus = new DisqusAPI($secret_key);

// to turn off SSL
$disqus->setSecure(false);

// call the API
$disqus->trends->listThreads();
```

Documentation on all methods, as well as general API usage can be found at http://disqus.com/api/


## About DisqusAPI library

Author:		DISQUS <team@disqus.com>

Copyright:	2007-2010 Big Head Labs

License:    Apache version 2.0 (see disqusapi/LICENSE for more information)

Link:		http://disqus.com/