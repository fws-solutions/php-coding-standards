# Forwardslash PHP Coding Standards

## Install

To install in your project, use:

```bash
composer require fws/php-coding-standards --dev
```

Then add a `phpcs.xml` file to your project:

```xml
<?xml version="1.0"?>
<ruleset name="Project">
    <rule ref="FWS"/>
</ruleset>
```

To do this quickly, run:

```bash
echo '<?xml version="1.0"?><ruleset name="Project"><rule ref="FWS"/></ruleset>' > phpcs.xml
```

Installation will automatically install `Forwardslash` standard for `vendor/bin/phpcs`.

## CLI Linting

### Lint a single file

```bash
./vendor/bin/phpcs -s path/to/file.php
```

### Lint multiple files

```bash
./vendor/bin/phpcs -s --extensions=php /path/to/dir
```

## Editor Linting

In your favorite editor install it's `phpcs` plugin, and it will automatically detect your `phpcs.xml` file and lint any PHP file you have open.
