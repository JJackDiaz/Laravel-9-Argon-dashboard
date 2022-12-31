<p align="center"><a href="https://laravel.com" target="_blank"><img src="https://raw.githubusercontent.com/laravel/art/master/logo-lockup/5%20SVG/2%20CMYK/1%20Full%20Color/laravel-logolockup-cmyk-red.svg" width="400" alt="Laravel Logo"></a></p>

<p align="center">
<a href="https://travis-ci.org/laravel/framework"><img src="https://travis-ci.org/laravel/framework.svg" alt="Build Status"></a>
<a href="https://packagist.org/packages/laravel/framework"><img src="https://img.shields.io/packagist/dt/laravel/framework" alt="Total Downloads"></a>
<a href="https://packagist.org/packages/laravel/framework"><img src="https://img.shields.io/packagist/v/laravel/framework" alt="Latest Stable Version"></a>
<a href="https://packagist.org/packages/laravel/framework"><img src="https://img.shields.io/packagist/l/laravel/framework" alt="License"></a>
</p>

## About Laravel

Installation

After initializing a fresh instance of Laravel (and making all the necessary configurations), install the preset using one of the provided methods:
Via composer

    Cd to your Laravel app
    Type in your terminal: composer require laravel/ui
    Install this preset via composer require laravel-frontend-presets/argon. No need to register the service provider. Laravel 9.x & up can auto detect the package.
    Run php artisan ui argon command to install the Argon preset. This will install all the necessary assets and also the custom auth views, it will also add the auth route in routes/web.php (NOTE: If you run this command several times, be sure to clean up the duplicate Auth entries in routes/web.php)
    In your terminal run composer dump-autoload
    Run php artisan migrate:fresh --seed to create basic users table

By using the archive

    In your application's root create a presets folder
    Download the archive of the repo and unzip it
    Copy and paste the downloaded folder in presets (created in step 2) and rename it to argon
    Open composer.json file
    Add "LaravelFrontendPresets\\ArgonPreset\\": "presets/argon/src" to autoload/psr-4 and to autoload-dev/psr-4
    Add LaravelFrontendPresets\ArgonPreset\ArgonPresetServiceProvider::class to config/app.php file
    Type in your terminal: composer require laravel/ui
    In your terminal run composer dump-autoload
    Run php artisan ui argon command to install the Argon preset. This will install all the necessary assets and also the custom auth views, it will also add the auth route in routes/web.php (NOTE: If you run this command several times, be sure to clean up the duplicate Auth entries in routes/web.php)
    Add in your .env file the info for your database
    Run php artisan migrate:fresh --seed to create basic users table
    Run npm install perfect-scrollbar
