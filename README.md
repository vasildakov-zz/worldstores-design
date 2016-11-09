# IT Workshop - Code Structure and Design

## Initialize our package

After installing composer, run this command in your project's directory.

```
$ composer init
```


## Basic dependencies

```json
{
    "name": "vasildakov/worldstores-design",
    "description": "IT Workshop - Code Structure and Design",
    "type": "library",
    "license": "MIT",
    "authors": [
        {
            "name": "Vasil Dakov",
            "email": "vasildakov@gmail.com"
        }
    ],
    "require": {
        "php": "^5.5 || ^7.0"
    },
    "require-dev": {
        "phpunit/phpunit": "^4.7 | ^5.0",
        "phpunit/php-code-coverage": "^3.0 | ^4.0",
        "phpunit/phpcov": "^3.1",
        "phpspec/phpspec": "^3.1"
    },
    "autoload": {
        "psr-4": {
            "Domain\\": "src/Domain/"
        }
    },
    "autoload-dev": {
        "psr-4": {
            "DomainTest\\": "test/DomainTest/"
        }
    }
}

```


## Install dependencies

```
$ composer install
```

## Running PHPUnit tests

```
$ php vendor/bin/phpunit

PHPUnit 5.6.2 by Sebastian Bergmann and contributors.

Time: 10 ms, Memory: 2.00MB

No tests executed!

```

