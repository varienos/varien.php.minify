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

echo "<style>".$minifier->css('/* path/to/file.1.css */').$minifier->css('/* path/to/file.2.css */')."</style>";
```

### JS

```php
use Varien\Minify\Minifier;

$minifier   = new Minifier();

echo "<script>".$minifier->js('/* path/to/file.1.js */').$minifier->js('/* path/to/file.2.js */')."</script>";
```

### HTML

```php
use Varien\Minify\Minifier;

$minifier   = new Minifier();

echo $minifier->html('/* HTML CODES */');
```