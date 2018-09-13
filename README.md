php-compat-cache
================

Make [danielbachhuber/php-compat-command](https://github.com/danielbachhuber/php-compat-command/) faster by using this cache of scan results.

Scan and cache results of the `twentysixteen` theme:

    wp php-compat-cache theme twentysixteen ~/php-compat-cache

Or scan and cache results of all plugins already tracked in cache:

    ls ~/php-compat-cache/plugins | xargs -I % wp php-compat-cache plugin % ~/php-compat-cache > plugin.log 2>&1

Then, use the cache results when scanning a WordPress install:

    WP_CLI_PHP_COMPAT_CACHE=~/php-compat-cache wp php-compat --path=<path-to-wp>

