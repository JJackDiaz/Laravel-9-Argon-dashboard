<p align="center"><a href="https://laravel.com" target="_blank"><img src="https://raw.githubusercontent.com/laravel/art/master/logo-lockup/5%20SVG/2%20CMYK/1%20Full%20Color/laravel-logolockup-cmyk-red.svg" width="400" alt="Laravel Logo"></a></p>

<p align="center">
<a href="https://travis-ci.org/laravel/framework"><img src="https://travis-ci.org/laravel/framework.svg" alt="Build Status"></a>
<a href="https://packagist.org/packages/laravel/framework"><img src="https://img.shields.io/packagist/dt/laravel/framework" alt="Total Downloads"></a>
<a href="https://packagist.org/packages/laravel/framework"><img src="https://img.shields.io/packagist/v/laravel/framework" alt="Latest Stable Version"></a>
<a href="https://packagist.org/packages/laravel/framework"><img src="https://img.shields.io/packagist/l/laravel/framework" alt="License"></a>
</p>


## Installation

After initializing a fresh instance of Laravel (and making all the necessary configurations), install the preset using one of the provided methods:
Via composer

1. [Cd] to your Laravel app
2. Type in your terminal: [composer require laravel/ui]
3. Install this preset via [composer require laravel-frontend-presets/argon]. No need to register the service provider. Laravel 9.x & up can auto detect the package.]**
4. Run php artisan ui argon command to install the Argon preset. This will install all the necessary assets and also the 
5. custom auth views, it will also add the auth route in routes/web.php (NOTE: If you run this command several times, be sure to clean up the duplicate Auth entries in routes/web.php)]**
6. In your terminal run composer dump-autoload]**
7. Run php artisan migrate:fresh --seed to create basic users table]**


## By using the archive

1. In your application's root create a presets folder
2. Download the archive of the repo and unzip it
3. Copy and paste the downloaded folder in presets (created in step 2) and rename it to argon
4. Open composer.json file
5. Add "LaravelFrontendPresets\\ArgonPreset\\": "presets/argon/src" to autoload/psr-4 and to autoload-dev/psr-4
6. Add LaravelFrontendPresets\ArgonPreset\ArgonPresetServiceProvider::class to config/app.php file
7. Type in your terminal: composer require laravel/ui
8. In your terminal run composer dump-autoload
9. Run php artisan ui argon command to install the Argon preset. This will install all the necessary assets and also the custom auth views, it will also add the auth route in routes/web.php (NOTE: If you run this command several times, be sure to clean up the duplicate Auth entries in routes/web.php)
10. Add in your .env file the info for your database
11. Run php artisan migrate:fresh --seed to create basic users table
12. Run npm install perfect-scrollbar

