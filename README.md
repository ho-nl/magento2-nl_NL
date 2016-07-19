# H&O Magento 2 Nederlandse vertalingen / Dutch Translations

## Install:
```BASH
composer require ho-nl/magento2-ho_nl
```

## Development install:
```BASH
composer require ho-nl/magento2-ho_nl "dev-master"
```

The translations are based on https://crowdin.com/project/magento-2/nl#/Head

Import translations:
```
curl http://107.170.242.99/build.php
cd vendor/ho-nl/magento2-nl-nl
wget -O nl_NL.csv http://107.170.242.99/var/Head/source_nl_NL.csv
```

## How are translations files loaded

In the file `Magento\Framework\App\Language\Dictionary::readPackCsv` all ``*.csv` files are loaded, no specific filename
required.
