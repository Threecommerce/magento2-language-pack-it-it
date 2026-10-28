# Changelog

All notable changes to this project are documented in this file.

The format is based on [Keep a Changelog](https://keepachangelog.com/en/1.0.0/),
and this project adheres to [Semantic Versioning](https://semver.org/spec/v2.0.0.html).

## [1.1.1] - 2026-10-06

### Fixed
- Moved `i18n/it_IT.csv` to the package root (`it_IT.csv`): Magento language
  packages only load CSV dictionaries from the package root, so the
  translations were never applied.

### Changed
- `composer.json`: PHP constraint aligned with the other Threecommerce modules
  (`^8.1`) and `magento/framework` constraint set to `*`.

## [1.1.0] - 2026-06-23

### Changed
- Converted the package from a Magento 2 module into a proper Magento 2 language
  package:
  - `composer.json` `type` changed from `magento2-module` to `magento2-language`.
  - `registration.php` now registers a `ComponentRegistrar::LANGUAGE` component
    (`threecommerce_it_it`) instead of a module.
  - Added `etc/language.xml` declaring the `it_IT` locale (vendor `threecommerce`,
    package `it_it`).
- Fixed the `composer.json` description, which incorrectly read
  "A Magento 2 module for maintenance mode".
- Replaced the `threecommerce/m2-base` dependency with `magento/framework` and
  dropped the unused VCS repository entry and PSR-4 autoload mapping.

### Removed
- Removed `etc/module.xml`, which is not used by a language package.

### Fixed
- Removed duplicate entries from `i18n/it_IT.csv` (`Add to Cart`,
  `Rate this product`, `Submit`).
- Resolved the conflicting translation for `Change Password`
  (`Cambia la password` vs `Cambia password`); now standardized to
  `Cambia la password`.

## [1.0.0]

### Added
- Initial Italian (it_IT) translations for Magento 2.