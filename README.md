# Laravel 5.5 Notification for Lumen 5.x #

[![Software License](https://img.shields.io/github/license/ciptohadi-web-id/lumen-notifications.svg)](LICENSE.md)
[![GitHub forks](https://img.shields.io/github/forks/ciptohadi-web-id/lumen-notifications.svg)](https://github.com/ciptohadi-web-id/lumen-notifications/network)
[![GitHub stars](https://img.shields.io/github/stars/ciptohadi-web-id/lumen-notifications.svg)](https://github.com/ciptohadi-web-id/lumen-notifications/stargazers)

[![Latest version](https://img.shields.io/packagist/v/ciptohadi-web-id/lumen-notifications.svg)](https://packagist.org/packages/ciptohadi-web-id/lumen-notifications)
[![Total Downloads](https://img.shields.io/packagist/dt/ciptohadi-web-id/lumen-notifications.svg)](https://packagist.org/packages/ciptohadi-web-id/lumen-notifications)

[![Twitter](https://img.shields.io/twitter/url/https/github.com/ciptohadi-web-id/lumen-notifications.svg?style=social)](https://twitter.com/intent/tweet?text=Wow:&url=https%3A%2F%2Fgithub.com%2Fciptohadi-web-id%2Flumen-notifications)

This package is a wrapper around [Laravel Notifications](https://laravel.com/docs/5.3/notifications) package, that enable it to work with Lumen 5.x

## Contents

- [Installation](#installation)
- [Usage](#usage)
- [Changelog](#changelog)
- [Testing](#testing)
- [Security](#security)
- [Contributing](#contributing)
- [Credits](#credits)
- [License](#license)

## Installation ##

To install the packge, we can run below command in terminal:

	composer require ciptohadi-web-id/lumen-notifications

After that, we should register the package in the section "Register Service Providers" in `bootstrap/app.php`

	$app->register(\ciptohadi\LumenNotifications\LumenNotificationsServiceProvider::class);
	

## Usage

After registering the Service Provider, we will have access to three new artisan commands, as shown below:

To create a new notification, we run below command:
 
	php artisan make:notification [notification-name]
	
To create database migration for notifications, we run below command
 
	php artisan notifications:table
	

To use the views from Laravel Notifications, we run below command:

	php artisan lumen-notifications:publish
	
### More information on how to use Laravel Notifications, we can consult wonderful Laravel documentation: [Laravel Notifications](https://laravel.com/docs/notifications) ###

## Changelog

Please see [CHANGELOG](CHANGELOG.md) for more information what has changed recently.

## Testing

``` bash
$ composer test
```

## Security

If you discover any security related issues, please email me at `ciptohadi79@gmail.com` instead of using the issue tracker.

## Contributing

Please see [CONTRIBUTING](CONTRIBUTING.md) for details.

## Credits

- [Cipto Hadi](https://ciptohadi.web.id)
- Inspired by [lab123it/lumen-notification](https://github.com/lab123it/lumen-notification)

## License

The MIT License (MIT). Please see [License File](LICENSE.md) for more information.