# laravel-cms-skeleton

## Installation
Use the composer create-project command:
```php
composer create-project --prefer-dist --stability=dev --repository=https://toran.webmodularity.com/repo/private/ webmod/laravel-cms-skeleton cms
```

## Config
1. Follow the Config setup guide for the [webmodularity/laravel-auth](https://github.com/webmodularity/laravel-auth) package (including social logins if needed)
2. Setup AdminLTE
    * Publish public assets:
    ```php
    php artisan vendor:publish --provider="JeroenNoten\LaravelAdminLte\ServiceProvider" --tag=assets
    ````
    * Publish config file:
    ```php
    php artisan vendor:publish --provider="JeroenNoten\LaravelAdminLte\ServiceProvider" --tag=config
    ```
    * Modify the `config/adminlte.php` config file.
3. Modify the `.env` file.

