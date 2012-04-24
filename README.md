googl-php
=========

Introduction
------------
googl-php is a small and simple PHP class intended to use with the Google URL shortening service "Goo.gl" and licensed under the GNU GPL v3.

Functions
---------
The class currently supports 2 actions:
  * *Shorten* a URL
  * *Expand* (looking up) an already shortened URL

Usage
-----
```php
<?php 

require_once('Googl.class.php');

$googl = new Googl('YOUR_API_KEY');

// Shorten URL
$googl->shorten('http://www.google.com/');

// Look up long URL
$googl->expand('http://goo.gl/fbsS');

unset($googl);
```

API key
-------
You don't need an API key to use the class (=the shortening service). 

But as Google writes in their own "Getting Started" guide, it's "highly recommended" to use one, and clicking a button doesn't really hurt, right? ;)

Further info
------------
For further information about Goo.gl and it's API, please visit: http://code.google.com/apis/urlshortener/.