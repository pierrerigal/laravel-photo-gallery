Laravel Photo Gallery
=====================

A photo gallery for Laravel 4.

## Installation
First you should install this package through Composer and edit your project's `composer.json`:

    "require": {
		"laravel/framework": "4.0.*",
		"jeroen-g/laravel-photo-gallery": "1.*"
	}

Next, update Composer via the command line:

    composer update

The next step is to add the service provider in `app/config/app.php`:

    'JeroenG\LaravelPhotoGallery\LaravelPhotoGalleryServiceProvider',

In the same file, add the following to the aliases array (so you can use the facade):

	'Gallery'		=>		'JeroenG\LaravelPhotoGallery\Facades\Gallery',

The last thing to do is to migrate:

	php artisan migrate --package="jeroen-g/laravel-photo-gallery"

This will create the tables for the gallery. Now you're ready to start!

## Usage