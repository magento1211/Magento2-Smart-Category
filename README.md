# Magento2 Smart Category

[![Total Downloads](https://poser.pugx.org/faonni/module-smart-category/downloads)](https://packagist.org/packages/faonni/module-smart-category)
[![Latest Stable Version](https://poser.pugx.org/faonni/module-smart-category/v/stable)](https://packagist.org/packages/faonni/module-smart-category)	

Extension Smart Category rules dynamically change the product selection according to a set of conditions (Similar Smart Playlists on iTunes).

You can create categories based on rules you specify, and then update these categories automatically as your products changes.

For example, you could create a category  includes only new products. Or you could create a categories of products by a particular brand, color, size, etc. You can add as many conditions to the expression as needed to describe the products to include.

## Compatibility

Magento CE 2.1.x, 2.2.x

## Install

To install the Smart Category, You must install kit of extensions:
- Smart Category - base of Smart Categories functionality.
- [Smart Category Configurable](https://github.com/karliuka/m2.SmartCategoryConfigurable) - changes simple products to their parents for configurable products.

#### Install via Composer (recommend)
The corresponding version of the Smart Category Kit will be installed automatically.

1. Go to Magento2 root folder

2. Enter following commands to install module:

    ```bash
    composer require faonni/module-smart-category-kit
    ```
   Wait while dependencies are updated.
   
#### Manual Installation
   
1. Create a folder {Magento root}/app/code/Faonni/SmartCategory

2. Download the corresponding [latest version](https://github.com/karliuka/m2.SmartCategory/releases)

3. Copy the unzip content to the folder ({Magento root}/app/code/Faonni/SmartCategory)

4. Install [Smart Category Configurable](https://github.com/karliuka/m2.SmartCategoryConfigurable)

### Completion of installation

1. Go to Magento2 root folder

2. Enter following commands:

    ```bash
	php bin/magento setup:upgrade
	php bin/magento setup:di:compile
	php bin/magento setup:static-content:deploy  (optional)
    ```

### Category edit page

<img alt="Magento2 Smart Category" src="https://karliuka.github.io/m2/smart-category/category.png" style="width:100%"/>
