# Abandoned / End-of-life
We're sorry, but this extension is no longer actively maintained. Please use https://github.com/magento-l10n/language-nl_NL instead.

# Reach Digital Magento 2 Nederlandse vertalingen / Dutch Translations with e-mailtranslations
<p align="center">
  <img src="https://github.com/ho-nl/magento2-nl_NL/blob/57d36db4477c37e1d6c19087f847558cd6be412a/docs/reach-dutch-translations.png" alt="Magento-2-nederlandse-vertalingen" height="300" width="300"/><br />
  <a href="https://www.reachdigital.nl/blog/correcte-nederlandse-vertalingen-voor-magento-2-magento-2-nl-inclusief-e-mailvertalingen">Find it on our website</a><br /></p>

<p align="center">
<img src="https://github.com/ho-nl/magento2-nl_NL/blob/master/docs/admin-catalog-product-listing2.png?raw=true" width="49%">
<img src="https://github.com/ho-nl/magento2-nl_NL/blob/master/docs/admin-dashboard2.png?raw=true" width="49%">
<img src="https://github.com/ho-nl/magento2-nl_NL/blob/master/docs/frontend-checkout.png?raw=true" width="49%">
<img src="https://github.com/ho-nl/magento2-nl_NL/blob/master/docs/frontend-customer-login2.png?raw=true" width="49%">
<br /></p>

- Complete translations for Magento 2.x CE and EE.
- Added Dutch [address formatting](src/etc/config.xml)

## Installation through Marketplace
As Reach Digital extensions are offered in the official Magento® Marketplace you can directly install them via the Magento® 2 backend. Magento® did a great job simplifying this process, they also provided a really good documentation. Please read the official documentation for installing extensions over the marketplace. 

http://devdocs.magento.com/guides/v2.0/comp-mgr/module-man/compman-start.html

## Installation through composer
```BASH
composer require honl/magento2-nl-nl
```

### Development install:
```BASH
composer require honl/magento2-nl-nl:^1@dev
```

## Contributing
Go to <a href="https://crowdin.com/project/magento-2/nl#/Head">CrowdIn</a> and translate files.
<p align="center"><img src="https://github.com/ho-nl/magento2-nl_NL/blob/master/docs/Crowdin-screenshot.png?raw=true" width="75%"></p>


## Import translations:
```BASH
curl http://107.170.242.99/build.php
cd vendor/honl/magento2-nl-nl
wget -O crowdin.csv http://107.170.242.99/var/Head/source_nl_NL.csv
git commit -am"Imported translations from crowdin"
git push

```

## How are translations files loaded
In the file `Magento\Framework\App\Language\Dictionary::readPackCsv` all ``*.csv` files are loaded, no specific filename
required.

## Credits
This extension was developed by Reach Digital with a lot of help from the Magento Community on CrowdIn. https://www.reachdigital.nl
