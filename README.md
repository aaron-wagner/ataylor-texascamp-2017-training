# ataylor-texascamp-2017-training

[![CircleCI](https://circleci.com/gh/texascamp-2017-training/ataylor-texascamp-2017-training.svg?style=shield)](https://circleci.com/gh/texascamp-2017-training/ataylor-texascamp-2017-training)
[![Dashboard ataylor-texascamp-2017-training](https://img.shields.io/badge/dashboard-ataylor_texascamp_2017_training-yellow.svg)](https://dashboard.pantheon.io/sites/11ac4ab0-273e-4a0b-844a-76456e209cbf#dev/code)
[![Dev Site ataylor-texascamp-2017-training](https://img.shields.io/badge/site-ataylor_texascamp_2017_training-blue.svg)](http://dev-ataylor-texascamp-2017-training.pantheonsite.io/)

---

## Install a Drupal patch with Composer

1. Check out [this address module issue on Drupal.org](https://www.drupal.org/node/2881391)
2. Run `composer require "cweagans/composer-patches ~1.0"` to install `composer-patches`
3. Add a `patches` section to `composer.json` nested under the `extra` section.
```
"enable-patching": true,
"composer-exit-on-patch-failure": true,
"patches": {
    "drupal/address": {
        "The locality.name data is missed in PlainFormater": "https://www.drupal.org/files/issues/locality-name-data-missed-plainformater-2881391-1.patch"
    }
},
```
4. Run `composer update`
5. Add, commit and push the `composer.json` and `composer.lock`
7. Push the changes to GitHub
8. Check the CircleCI logs to see if the patch applied correctly

Move on to [Configuration management](https://github.com/texascamp-2017-training/ataylor-texascamp-2017-training/tree/config-management)