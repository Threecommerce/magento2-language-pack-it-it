# Threecommerce Italian (it_IT) language pack for Magento 2 / Mage-OS

A native Magento 2 language pack that registers the `it_IT` locale and translates more than 100 key storefront strings, in correct and consistent Italian.

**Compatibility:** Magento Open Source / Adobe Commerce 2.4.4 – 2.4.9 · Mage-OS 1.x / 3.x · PHP 8.1 – 8.4 · Themes: Luma, Hyvä, Breeze
**License:** free · **Current version:** see [Releases](../../releases)

## Features

- **Cart and mini-cart:** Add to cart, Proceed to checkout, empty cart message.
- **Checkout and order:** addresses, shipping and payment methods, coupons, totals, order confirmation.
- **Customer account:** login, registration, password, order history, addresses.
- **Catalog:** availability, sorting, compare, wishlist, reviews.
- **Newsletter:** subscription, confirmation and error messages.
- Not a module: a language pack, nothing to configure.

## Requirements

- Magento Open Source / Adobe Commerce 2.4.4+ or Mage-OS
- PHP 8.1 – 8.4
- Package: `magento/framework`

## Installation

The package is distributed through our Composer repository at `repo.threecommerce.it`. Request the credentials from the [product page](https://www.threecommerce.it/traduzione-italiana-it-it-per-magento-2?utm_source=github&utm_medium=readme&utm_campaign=magento2-language-pack-it-it), then:

```bash
composer config repositories.threecommerce composer https://repo.threecommerce.it
composer require threecommerce/m2-language-it-it
bin/magento setup:upgrade
bin/magento cache:flush
```

In production mode regenerate the static content: `bin/magento setup:static-content:deploy it_IT`.

## Configuration

Set the locale of your store view to **Italian (Italy)** in Stores → Configuration → General → Locale Options, then regenerate the static content.

## Documentation and support

- Product page: [threecommerce.it/traduzione-italiana-it-it-per-magento-2](https://www.threecommerce.it/traduzione-italiana-it-it-per-magento-2?utm_source=github&utm_medium=readme&utm_campaign=magento2-language-pack-it-it)
- [Changelog](CHANGELOG.md) (in Italian)
- Support and custom development: [threecommerce.it/contatti](https://www.threecommerce.it/contatti?utm_source=github&utm_medium=readme&utm_campaign=magento2-language-pack-it-it)

---

*This repository is the public showcase of the module. The source code is kept in a private repository.*
