# Hybrid PHPCS Rules.
PHPCS rules used in ThemeHybrid projects.

* PHPCS

[PHP_CodeSniffer](https://github.com/squizlabs/PHP_CodeSniffer) coding standards ruleset for the ThemeHybrid projects.

## Installation

### Standalone

```
git clone https://github.com/themehybrid/phpcs-rules
cd phpcs-rules
composer install
```

### Dependency

```
composer config repositories.phpcs-rules vcs https://github.com/themehybrid/phpcs-rules
composer require themehybrid/phpcs-rules:dev-main --dev
```

Create or modify `phpcs.xml` in project root:
```xml
<?xml version="1.0"?>
<ruleset>
    <file>src</file>
    <rule ref="ThemeHybrid"/>
</ruleset>
```

### Run

```
$ composer exec -v phpcs -- -s [<file>] ...
```
