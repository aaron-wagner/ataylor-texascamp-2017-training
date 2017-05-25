# ataylor-texascamp-2017-training

[![CircleCI](https://circleci.com/gh/texascamp-2017-training/ataylor-texascamp-2017-training.svg?style=shield)](https://circleci.com/gh/texascamp-2017-training/ataylor-texascamp-2017-training)
[![Dashboard ataylor-texascamp-2017-training](https://img.shields.io/badge/dashboard-ataylor_texascamp_2017_training-yellow.svg)](https://dashboard.pantheon.io/sites/11ac4ab0-273e-4a0b-844a-76456e209cbf#dev/code)
[![Dev Site ataylor-texascamp-2017-training](https://img.shields.io/badge/site-ataylor_texascamp_2017_training-blue.svg)](http://dev-ataylor-texascamp-2017-training.pantheonsite.io/)

---

## Configuring Address Module
1) Visit the address module multidev on Pantheon
2) Login to the Drupal admin
3) Create a new content type, such as _store locations_
4) Add the address field and other fields, as desired, to the content type
5) Create some dummy content with the new content type
6) Export and commit config
    - Make sure the multidev is in SFTP mode on Pantheon
    - Go to `/admin/config/development/configuration/full/update`
    - Login with username `admin` and password `texascamp` if needed
    - Select `sync` under _Config source_
    - Click _Update configuration_
    - Go back to the Pantheon site dashboard
    - Type a commit message
    - Click _Commit_
7) Wait a few minutes then check out the pushback to GitHub
8) Create pull request on GitHub from the `address-module` branch
