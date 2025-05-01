# PHPUnit Zero Configuration Setup

Requires [devbox](https://www.jetify.com/devbox).

```shell
# open the devbox shell
$ devbox shell
Starting a devbox shell...

# run phpunit using the provided configuration
(devbox) $ phpunit
PHPUnit 12.1.0 by Sebastian Bergmann and contributors.

Runtime:       PHP 8.4.6
Configuration: phpunit.dist.xml

..                                                                  2 / 2 (100%)

Time: 00:00.002, Memory: 8.00 MB

OK (2 tests, 2 assertions)

```


- Entering the shell runs the `init_hook` in `devbox.json`, which runs `composer install`, which sets up the autoloader, required for the phpunit bootstrap.
- You can also run `devbox run test` to run `phpunit`, included to demonstrate how to add scripts.
- The test php code has been adapted from [PHPUnit's documentation](https://phpunit.de/getting-started/phpunit-12.html).
- PHPStorm configuration added.
