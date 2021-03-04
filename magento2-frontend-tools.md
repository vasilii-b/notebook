
## Magento 2 storefront information in browser

### Method #1 - [MageSpecialist's Chrome Toolbar](https://github.com/magespecialist/mage-chrome-toolbar#magento-chrome-toolbar-for-msp-devtools)

![Magento chrom devtools tab](https://user-images.githubusercontent.com/13456702/109925248-2fac6f80-7cca-11eb-8802-47b1279050b4.png)
![Inspect element magento details](https://user-images.githubusercontent.com/13456702/109925344-49e64d80-7cca-11eb-890b-31bbcc66f601.png)


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


✅ **can be enabled by IP**

⚠️ breaks the `/graphql` endpoint


#### Installation

From CLI:

1. `composer require msp/devtools --dev`
2. `bin/magento c:f`
3. `bin/magento c:d full_page`
4. `bin/magento s:up`
5. `bin/magento config:set msp_devtools/general/enabled 1`


### Method 2 - [MGT Developer Toolbar for Magento 2](https://github.com/mgtcommerce/Mgt_Developertoolbar)

![Showing layout blocks](https://www.mgt-commerce.com/docs/img/mgt-developer-toolbar/magento2/blocks.png)

✅ **can be enabled by IP**

#### Installation

Follow the steps [here](https://www.mgt-commerce.com/docs/mgt-developer-toolbar/magento2/installation).


## A faster drop in replacement for `bin/magento cache:clean` with a file watcher.

See [Magento 2 Cache Clean](https://github.com/mage2tv/magento-cache-clean#magento-2-cache-clean) for more details.

#### Installation

From CLI

1. `composer require --dev mage2tv/magento-cache-clean`
2. `bin/magento cache:enable`

#### Preconditions

Need to install `nodejs` version > 10.8.

`sudo apt-get install nodejs`

#### Usage

`vendor/bin/cache-clean.js --watch`

In case of errors see [known issues](https://github.com/mage2tv/magento-cache-clean#known-issues).
