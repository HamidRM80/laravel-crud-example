# laravel-crud-example

This package provides an example of Post CRUD operations in Laravel. It includes basic functionality for creating, reading, updating, and deleting posts.

## Installation

You can install this package via Composer:

### Via Packagist

```bash
composer require hamidreza/laravel-crud-example
```
then add below code to bootstrap/providers.php:
```php
return [
    App\Providers\AppServiceProvider::class,
    Hamidreza\LaravelCrudExample\PostServiceProvider::class,
];
```
Optionally, publish the configuration file if you want to change any defaults:
```bash
php artisan vendor:publish --provider="Hamidreza\LaravelCrudExample\PostServiceProvider"
```
if you run above code, config and views and migrations will be published

