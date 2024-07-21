# Changes and migration requirements

## Version 0.0.13

* Fix problem installing system Psycopg2 package on Ubuntu 22.

## Version 0.0.12

* Support Docker-based Python application (via emptyhammock-role-docker-application);
  set `application_mode` to `"docker"`.
* Support Ubuntu 24.

## Version 0.0.11

* Install `pkg-config` package.

## Version 0.0.10

* Support Ubuntu >= 20.

## Version 0.0.9

* Fix deprecation warnings with Ansible 2.10.

## Version 0.0.8

* `nodesource_repo` now defaults to `"os"`.  Set to `"nodesource"` to install node from
  the nodesource apt repo.

* Allow de-installation of arbitrary apt packages, to handle the case where a package is
  no longer needed.  Set `system_packages_to_remove` to a list of packages to remove.

* Allow installation of arbitrary apt packages as long as the repo is configured.  Set
  `extra_system_packages` to a list of additional packages to install.

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
