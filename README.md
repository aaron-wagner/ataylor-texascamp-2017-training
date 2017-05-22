# ataylor-texascamp-2017-training

[![CircleCI](https://circleci.com/gh/texascamp-2017-training/ataylor-texascamp-2017-training.svg?style=shield)](https://circleci.com/gh/texascamp-2017-training/ataylor-texascamp-2017-training)
[![Dashboard ataylor-texascamp-2017-training](https://img.shields.io/badge/dashboard-ataylor_texascamp_2017_training-yellow.svg)](https://dashboard.pantheon.io/sites/11ac4ab0-273e-4a0b-844a-76456e209cbf#dev/code)
[![Dev Site ataylor-texascamp-2017-training](https://img.shields.io/badge/site-ataylor_texascamp_2017_training-blue.svg)](http://dev-ataylor-texascamp-2017-training.pantheonsite.io/)

## Installing Address Module
1) Download address module with Composer
	- Create a new git branch `address-module`
	- `composer require "drupal/address ~1.0"`
	- Add and commit `composer.json` and `composer.lock` with git
2) Check CircleCI build for success and deployment to Pantheon
3) Visit Pantheon multidev
4) Login to the Drupal dashboard
5) Enable address module
6) Create a new store locations content type
7) Add the address field and other fields, as desired, to the content type
8) Create some dummy content with the new content type
9) Export and commit config
10) Check out pushback to GitHub
11) Create pull request on GitHub
