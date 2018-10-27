# Changes and migration requirements

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
