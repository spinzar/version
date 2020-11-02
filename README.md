# Version management package for Laravel.
[![Release](https://img.shields.io/github/v/release/spinzar/version?label=release)](https://github.com/spinzar/version/releases)
![Downloads](https://img.shields.io/github/downloads/spinzar/version/total?label=downloads)
[![Tests](https://img.shields.io/github/workflow/status/spinzar/version/Tests?label=tests)](https://github.com/spinzar/version/actions)
[![License](https://img.shields.io/github/license/spinzar/version?label=license)](LICENSE.txt)



A [SemVer](http://semver.org) compatible version management package for softwares built on Laravel.

## Getting Started

### 1. Install

Run the following command:

```bash
composer require spinzar/version
```

### 2. Register (for Laravel < 5.5)

Register the service provider in `config/app.php`

```php
Spinzar\Version\Provider::class,
```

Add alias if you want to use the facade.

```php
'Version' => Spinzar\Version\Facade::class,
```

### 3. Publish

Publish config file.

```bash
php artisan vendor:publish --tag=version
```


### 4. Configure

You can change the version information of your app from `config/version.php` file

## Usage

### version($method = null)

You can either enter the method like `version('short')` or leave it empty so you could firstly get the instance then call the methods like `version()->short()`

## Changelog

Please see [Releases](../../releases) for more information what has changed recently.

## Contributing

Pull requests are more than welcome. You must follow the PSR coding standards.

## Security

If you discover any security related issues, please email security@spinzar.co instead of using the issue tracker.

## Credits

- [Nassim Nasibullah](https://github.com/spinzar)
- [All Contributors](../../contributors)

## License

The MIT License (MIT). Please see [LICENSE](LICENSE.md) for more information.