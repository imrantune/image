# Task # 2
TODOs
* Add testing
* Extend usage to other methods if they allow options
* Move key into constant
* Update documentation
* Read defaults from config if defined (leave current values as fallback)
* Define if needed on Commands and how to pass it from CLI

# Task # 1

https://github.com/Intervention/image/issues/1077

Remember your job is to make *incremental* progress, break the task into smaller tasks, or finish something in 15 minutes, then pass it along to the next contributor. 
No responsibility, only fun.

If you don't finish, add your next task to the readme.md. When you're done make a pull request to the repo

* Add additionalOptions in the call chain for initUrl as optional



Email with questions

# Intervention Image

Intervention Image is a **PHP image handling and manipulation** library providing an easier and expressive way to create, edit, and compose images. The package includes ServiceProviders and Facades for easy **Laravel** integration.

[![Latest Version](https://img.shields.io/packagist/v/intervention/image.svg)](https://packagist.org/packages/intervention/image)
[![Build Status](https://travis-ci.org/Intervention/image.png?branch=master)](https://travis-ci.org/Intervention/image)
[![Monthly Downloads](https://img.shields.io/packagist/dm/intervention/image.svg)](https://packagist.org/packages/intervention/image/stats)

## Requirements

- PHP >=5.4
- Fileinfo Extension

## Supported Image Libraries

- GD Library (>=2.0)
- Imagick PHP extension (>=6.5.7)

## Getting started

- [Installation](http://image.intervention.io/getting_started/installation)
- [Laravel Framework Integration](http://image.intervention.io/getting_started/installation#laravel)
- [Basic Usage](http://image.intervention.io/use/basics)

## Code Examples

```php
// open an image file
$img = Image::make('public/foo.jpg');

// you can also pass additional headers options for an url
$additionalOptions['url_options']['http']['headers'] = "Accept: image/webp";
$img = Image::make($url, $additionalOptions);

// resize image instance
$img->resize(320, 240);

// insert a watermark
$img->insert('public/watermark.png');

// save image in desired format
$img->save('public/bar.jpg');
```

Refer to the [official documentation](http://image.intervention.io/) to learn more about Intervention Image.

## Contributing

Contributions to the Intervention Image library are welcome. Please note the following guidelines before submitting your pull request.

- Follow [PSR-2](http://www.php-fig.org/psr/psr-2/) coding standards.
- Write tests for new functions and added features
- API calls should work consistently with both GD and Imagick drivers

## License

Intervention Image is licensed under the [MIT License](http://opensource.org/licenses/MIT).

Copyright 2017 [Oliver Vogel](http://olivervogel.com/)
