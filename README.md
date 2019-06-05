# Compressor IO Helper PHP Class

## Usage
```php
use renj1e\phpImgCompress\CompressorIO;

$files = [];

$compress = new CompressorIO();
$compress->backup = true; // default: true. when it's true, create a directory and files will be copied to there before compressed.

$files[] = '/path/to/source/image/file.jpg';
$compress->compress($files);

// you can compress one file or get file list by a folder and compress.
$files = $compress->findFolder('png|jpg|jpeg|gif');
$compress->compress($files);
```


## Installation

Simply add a dependency on renj1e/php-image-compress to your composer.json file if you use [Composer](https://getcomposer.org/) to manage the dependencies of your project:

```sh
composer require renj1e/php-image-compress
```

## License

Minify is [MIT](http://opensource.org/licenses/MIT) licensed.
