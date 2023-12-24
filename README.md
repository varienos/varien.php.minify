## Installation

Simply add a dependency on `varienos/varien.php.minify` to your composer.json file if you use [Composer](https://getcomposer.org/) to manage the dependencies of your project:

```sh
composer require varienos/varien.php.minify
```

## Usage

### CSS

```php
use Varien\Minify\Minifier;

$minifier   = new Minifier();

echo "<style>".$minifier->cssMinify('/* path/to/file.1.css */').$minifier->cssMinify('/* path/to/file.2.css */')."</style>";
```

### JS

```php
use Varien\Minify\Minifier;

$minifier   = new Minifier();

echo "<script>".$minifier->jsMinify('/* path/to/file.1.js */').$minifier->jsMinify('/* path/to/file.2.js */')."</script>";
```

### HTML

```php
use Varien\Minify\Minifier;

$minifier   = new Minifier();

echo $minifier->htmlMinify('/* HTML CODES */');
```