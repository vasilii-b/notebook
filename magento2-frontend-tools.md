
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
