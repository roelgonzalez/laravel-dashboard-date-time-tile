# A date & time tile for the Laravel Dashboard

[![Latest Version on Packagist](https://img.shields.io/packagist/v/roelgonzalez/laravel-dashboard-date-time-tile.svg?style=flat-square)](https://packagist.org/packages/roelgonzalez/laravel-dashboard-date-time-tile)
[![GitHub Tests Action Status](https://img.shields.io/github/workflow/status/roelgonzalez/laravel-dashboard-date-time-tile/run-tests?label=tests)](https://github.com/roelgonzalez/laravel-dashboard-date-time-tile/actions?query=workflow%3Arun-tests+branch%3Amaster)
[![Total Downloads](https://img.shields.io/packagist/dt/roelgonzalez/laravel-dashboard-date-time-tile.svg?style=flat-square)](https://packagist.org/packages/roelgonzalez/laravel-dashboard-date-time-tile)

This tile displays date & time for a specified timezone.

This tile can be used on [the Laravel Dashboard](https://docs.spatie.be/laravel-dashboard).

## Compatibility

- PHP `^8.3`
- `spatie/laravel-dashboard` `^4.0`

<p align="center">
    <img width="512" src="https://github.com/roelgonzalez/laravel-dashboard-date-time-tile/raw/master/screenshot.png">
</p>

## Credits
Forked from the original DateTimeTile package.

## Installation

You can install the package via composer:

```bash
composer require roelgonzalez/laravel-dashboard-date-time-tile
```

## Usage

In your dashboard view you use the `livewire:date-time-tile` component.

```html
<x-dashboard>
    <livewire:date-time-tile position="a1" timezone="Europe/Brussels" />
</x-dashboard>
```

By default, the title of the tile will display the timezone string, i.e. Europe/Brussels. This can be overridden using the optional `title` parameter, e.g.

```html
<livewire:date-time-tile position="a1" timezone="Europe/London" title="Greenwich Mean Time" />
```

### Customizing the view

If you want to customize the view used to render this tile, run this command:

```bash
php artisan vendor:publish --provider="RoelGonzalez\DateTimeTile\DateTimeTileServiceProvider" --tag="dashboard-date-time-tile-views"
```

## Changelog

Please see [CHANGELOG](CHANGELOG.md) for more information on what has changed recently.

## License

The MIT License (MIT). Please see [License File](LICENSE.md) for more information.
