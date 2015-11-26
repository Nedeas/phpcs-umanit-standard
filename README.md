# PHPCS UmanIT Standard

A coding standard for PHPCS.

## Installation

Our coding standard use Symfony2 and Wordpress standards.

```sh
mkdir -p path/to/standards
git clone https://github.com/escapestudios/Symfony2-coding-standard.git path/to/standards/symfony2
git clone https://github.com/WordPress-Coding-Standards/WordPress-Coding-Standards.git path/to/standards/wordpress
git clone https://github.com/vrobic/phpcs-umanit-standard.git path/to/standards/umanit
phpcs --config-set installed_paths /absolute/path/to/standards/symfony2,/absolute/path/to/standards/wordpress,/absolute/path/to/standards/umanit
phpcs -i
```

## Basic usage

To sniff a file or directory for coding standard violations :

```sh
phpcs --standard=path/to/ruleset.xml -s --colors path/to/file/or/directory
```

To fix the violations automatically, run :

```sh
phpcbf --standard=path/to/ruleset.xml path/to/file/or/directory
```
