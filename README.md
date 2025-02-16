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

