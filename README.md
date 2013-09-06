# [laravel4-disqus](http://roumen.it/projects/laravel4-disqus) package

[![Latest Stable Version](https://poser.pugx.org/roumen/disqus/version.png)](https://packagist.org/packages/roumen/disqus) [![Total Downloads](https://poser.pugx.org/roumen/disqus/d/total.png)](https://packagist.org/packages/roumen/disqus)

A Laravel 4 package for Disqus API.


## Installation

Add the following to your `composer.json` file :

```json
"roumen/disqus": "dev-master"
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