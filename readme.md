# laravel-cms-skeleton

## Installation
### Composer
* Use the composer create-project command to install:
```php
composer create-project --prefer-dist --repository=https://toran.webmodularity.com/repo/private/ webmod/laravel-cms-skeleton cms
```

### Database
* Create a new schema (or use an existing) using utf8mb4 charset if possible
* Make any changes needed to DB permissions and add DB credentials to `.env`
* Run DB Migrations & Seeders:
```php
php artisan migrate --seed
```

### [AdminLTE](https://github.com/jeroennoten/Laravel-AdminLTE)
* Publish public assets:
```php
php artisan vendor:publish --provider="JeroenNoten\LaravelAdminLte\ServiceProvider" --tag=assets
````
* Publish config file:
```php
php artisan vendor:publish --provider="JeroenNoten\LaravelAdminLte\ServiceProvider" --tag=config
```
* Setup AdminLTE via the `config/adminlte.php` file.

### [webmodularity/laravel-auth](https://github.com/webmodularity/laravel-auth)
* Publish config file:
```php
php artisan vendor:publish --provider="WebModularity\LaravelAuth\AuthServiceProvider" --tag=config
```
* Configure [Social Logins](https://github.com/webmodularity/laravel-auth#social-logins) if needed.
