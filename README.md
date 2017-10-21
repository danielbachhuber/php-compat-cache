php-compat-cache
================

Make [danielbachhuber/php-compat-command](https://github.com/danielbachhuber/php-compat-command/) faster by using this cache of scan results.

Scan and cache results of the `twentysixteen` theme:

    wp --require=danielbachhuber/php-compat-command/bin/php-compat-cache.php php-compat-cache theme twentysixteen ~/php-compat-cache

Then, use the cache results when scanning a WordPress install:

    WP_CLI_PHP_COMPAT_CACHE=~/php-compat-cache wp php-compat --path=<path-to-wp>

