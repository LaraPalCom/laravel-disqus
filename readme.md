# [laravel-disqus](http://roumen.it/projects/laravel-disqus) bundle

A Laravel bundle for the DisqusAPI library.


## Installation

Download the latest bundle from: https://github.com/RoumenDamianoff/laravel-disqus/archive/laravel3.zip

and extract the archive to your bundles folder.

To autoload the bundle you need to edit your ``application/bundles.php`` end add:

```php
'disqus' => array('auto' => true)
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

License:        Apache version 2.0 (see disqusapi/LICENSE for more information)

Link:		http://disqus.com/