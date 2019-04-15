**This project has been abandoned and is no longer maintained.**

# PHPUnit Skeleton Generator

`phpunit-skelgen` is a tool that can generate skeleton test classes from production code classes and vice versa.

## Installation

### PHP Archive (PHAR)

The easiest way to obtain phpunit-skelgen is to download a [PHP Archive (PHAR)](http://php.net/phar) that has all required dependencies of phpunit-skelgen bundled in a single file:

    curl https://github.com/forest2087/phpunit-skeleton-generator/blob/master/build/phpunit-skelgen?raw=true --output phpunit-skelgen
    chmod +x phpunit-skelgen
    mv phpunit-skelgen /usr/local/bin/phpunit-skelgen


### Composer

Simply add a dependency on `phpunit/phpunit-skeleton-generator` to your project's `composer.json` file if you use [Composer](http://getcomposer.org/) to manage the dependencies of your project. Here is a minimal example of a `composer.json` file that just defines a development-time dependency on phpunit/phpunit-skeleton-generator:

    {
        "require-dev": {
            "phpunit/phpunit-skeleton-generator": "*"
        }
    }

For a system-wide installation via Composer, you can run:

    composer global require "phpunit/phpunit-skeleton-generator=*"

Make sure you have `~/.composer/vendor/bin/` in your path.

### Dependencies

*   apache ant - build tool
*   phpab - build phar
