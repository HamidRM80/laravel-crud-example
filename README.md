# laravel-crud-example

This package provides an example of Post CRUD operations in Laravel. It includes basic functionality for creating, reading, updating, and deleting posts.

## Installation

1. You can install this package via Composer:

### Via Packagist

```bash
composer require hamidreza/laravel-crud-example:dev-main
```
2. then add below code to bootstrap/providers.php:
```php
return [
    App\Providers\AppServiceProvider::class,
    Hamidreza\LaravelCrudExample\PostServiceProvider::class,
];
```
3. Optionally, publish the configuration file if you want to change any defaults:
```bash
php artisan vendor:publish --provider="Hamidreza\LaravelCrudExample\PostServiceProvider"
```
if you run above code, config and views and migrations will be published

4. change your DB_DATABASE name in .env file to laravel:
```php
DB_DATABASE=laravel
```
5. run your project by:
```bash
php artisan serve
```
6. connect to your mysql database
7. add below code to app/providers/AppServiceProvider.php file in boot function and import it's Schema class from Facades:
```php
public function boot(): void
    {
        Schema::defaultStringLength(191);
    }
```
8. run below commands for create migrations:
```bash
php artisan migrate
```
9. you can use project by this url: post/index
