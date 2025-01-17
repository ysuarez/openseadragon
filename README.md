# ![Mascot](https://user-images.githubusercontent.com/5439169/65790675-0242b600-e115-11e9-817f-e31c41bf2ece.png) Openseadragon
[![Build Status](https://travis-ci.com/Islandora-CLAW/openseadragon.png?branch=8.x-1.x)](https://travis-ci.com/Islandora-CLAW/openseadragon)
[![Contribution Guidelines](http://img.shields.io/badge/CONTRIBUTING-Guidelines-blue.svg)](./CONTRIBUTING.md)
[![LICENSE](https://img.shields.io/badge/license-GPLv2-blue.svg?style=flat-square)](./LICENSE)

## Introduction

Drupal 8 FieldFormatter to display an image or generic file using a IIIF Image server and OpenSeadragon.

## Requirements

* [drupal/libraries](https://www.drupal.org/project/libraries)
* [drupal/token](https://www.drupal.org/project/token)
* [openseadragon library](https://github.com/openseadragon/openseadragon)

## Installation

As a Drupal module, this module can be installed via composer and enabled via drush, like:
1. `composer require islandora/openseadragon:dev-8.x-1.x`
2. download the version of openseadragon that you want to install (ie. download a release zip or tar from https://github.com/openseadragon/openseadragon/releases and unarchive it)
3. place the version of openseadragon in your drupal install in a location such as `web/sites/all/assets/vendor/openseadragon`
4. `drush pm-en openseadragon`

If you are using the [claw-playbook](https://github.com/Islandora-Devops/claw-playbook), there is an [ansible role](https://github.com/Islandora-Devops/ansible-role-drupal-openseadragon) already built for installing openseadragon.


## Configuration

The module, once enabled will create a configuration page under Configuration > Media > Openseadragon Settings.
There will be some default settings checked for you. The one setting which you will need to set as a required minimum is the IIIF Image Server Location, such as `http://127.0.0.1:8080/cantaloupe/iiif/2`
There are a myriad of other configuration settings available there. Additional openseadragon documentation is available [here](https://openseadragon.github.io/#examples-and-features)
# ![Config](https://user-images.githubusercontent.com/5439169/65790661-fd7e0200-e114-11e9-8d71-86b5f949d870.png)


## Documentation

Further documentation for this module is available on the [Islandora 8 documentation site](https://islandora-claw.github.io/CLAW/).

## Troubleshooting/Issues

Having problems or solved a problem? Check out the Islandora google groups for a solution.

* [Islandora Group](https://groups.google.com/forum/?hl=en&fromgroups#!forum/islandora) 
* [Islandora Dev Group](https://groups.google.com/forum/?hl=en&fromgroups#!forum/islandora-dev)

## Maintainers

Current maintainers:

* [Eli Zoller](https://github.com/elizoller)


## Development

If you would like to contribute, please get involved by attending our weekly [Tech Call](https://github.com/Islandora-CLAW/CLAW/wiki). We love to hear from you!

If you would like to contribute code to the project, you need to be covered by an Islandora Foundation [Contributor License Agreement](http://islandora.ca/sites/default/files/islandora_cla.pdf) or [Corporate Contributor License Agreement](http://islandora.ca/sites/default/files/islandora_ccla.pdf). Please see the [Contributors](http://islandora.ca/resources/contributors) pages on Islandora.ca for more information.

We recommend using the [claw-playbook](https://github.com/Islandora-Devops/claw-playbook) to get started. If you want to pull down the submodules for development, don't forget to run `git submodule update --init --recursive` after cloning.

## License

[GPLv2](./LICENSE)
