# Changes and migration requirements

## Version 0.0.7

* nodejs: Choose OS repo or nodesource repo (`nodejs_repo: ["nodesource"|"os"]`)
* nodejs: when installed from nodesource: Choose Version (`nodesource_nodejs_version: node_6.x`)
* npm: Allow installing this separate package (`install_npm: "yes"`)

## Version 0.0.6

* Install unzip

## Version 0.0.5

* Allow skipping PostgreSQL installation (`install_postgres: "no"`).
* Allow skipping Node installation (`install_nodejs: "no"`).
* Fix Ubuntu 18.04 incompatibility with `python-software-properties`.

## Version 0.0.4

* Fix problem in 0.0.3.

## Version 0.0.3

* No longer install apticron; remove if previously installed.

* System package python-openssl now installed; needed for Ansible's
  openssl_privatekey.
