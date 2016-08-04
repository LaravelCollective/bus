# Bus

[![Build Status](https://travis-ci.org/LaravelCollective/bus.svg)](https://travis-ci.org/LaravelCollective/bus)
[![Total Downloads](https://poser.pugx.org/LaravelCollective/bus/downloads)](https://packagist.org/packages/laravelcollective/bus)
[![Latest Stable Version](https://poser.pugx.org/LaravelCollective/bus/v/stable.svg)](https://packagist.org/packages/laravelcollective/bus)
[![Latest Unstable Version](https://poser.pugx.org/LaravelCollective/bus/v/unstable.svg)](https://packagist.org/packages/laravelcollective/bus)
[![License](https://poser.pugx.org/LaravelCollective/bus/license.svg)](https://packagist.org/packages/laravelcollective/bus)

This package provides an implementation of the `Illuminate\Contracts\Bus\Dispatcher` interface that matches the Laravel 5.1.x implementation with separate commands and handlers.

## Installation

- Remove `Illuminate\Bus\BusServiceProvider` from your `app.php` configuration file.
- Add `Collective\Bus\BusServiceProvider` to your `app.php` configuration file.

If you are type-hinting `Illuminate\Bus\Dispatcher`, you should now type-hint `Collective\Bus\Dispatcher`.

If upgrading from 5.2, you should use `Collective\Bus\Contracts\SelfHandling` instead of `Illuminate\Contracts\Bus\SelfHandling` to indicate that a command does not use a separate handler class.
