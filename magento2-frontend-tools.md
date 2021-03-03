
## Magento 2 storefront information in browser

This allows to see in the browser's code inspector:

- Applied theme
- Layout handles
- Layout Blocks/Containers
- PHP Blocks
- Controller
- Observers
- Plugins
- uiComponents
- ...

See [MageSpecialist's Chrome Toolbar](https://github.com/magespecialist/mage-chrome-toolbar#magento-chrome-toolbar-for-msp-devtools) for more details.

### Installation

From CLI:

1. `composer require msp/devtools --dev`
2. `bin/magento c:f`
3. `bin/magento c:d full_page`
4. `bin/magento s:up`
5. `bin/magento config:set msp_devtools/general/enabled 1`

## A faster drop in replacement for `bin/magento cache:clean` with a file watcher.

See [Magento 2 Cache Clean](https://github.com/mage2tv/magento-cache-clean#magento-2-cache-clean) for more details.

### Installation

From CLI

1. `composer require --dev mage2tv/magento-cache-clean`
2. `bin/magento cache:enable`

### Preconditions

Need to install `nodejs` version > 10.8.

`sudo apt-get install nodejs`

### Usage

`vendor/bin/cache-clean.js --watch`

In case of errors see [known issues](https://github.com/mage2tv/magento-cache-clean#known-issues).
