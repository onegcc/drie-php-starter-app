# drie-php-starter-app

A barebones PHP app, based on the [Laravel](https://laravel.com/) framework.

## Requirements

1. [PHP](http://php.net/manual/en/install.php). Note on macOS PHP is installed out of the box but is some versions behind the current release.
2. [Composer](https://getcomposer.org/download/). Follow the command-line instructions at the top of the page to install Composer in your working directory. These commands will leave a file named `composer.phar` in your working directory which you can use to run `composer` commands.

## Setup

We've used [Composer](https://getcomposer.org/download/) to create the project and manage the dependencies. Once you've cloned this repo you can install dependencies using `composer install`.

## Development

You can test changes locally with the following command once you've set everything up: `php artisan serve`.

## Forking this repo?

Laravel makes use of the `APP_KEY` environment variable to find the encryption key it should use for securing itself. We make this variable available to the running app on drie by setting it in `.drie.yml`.

For expediency's sake we haven't encrypted this value, since this is a starter app. If you're forking this repo then **we strongly recommend that you create a new encryption key and store it securely** (e.g. by encrypting it with the drie CLI). You can generate a new encrytion key using `php artisan key:generate`.
