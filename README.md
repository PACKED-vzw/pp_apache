# pp_apache

#### Table of Contents

1. [Description](#description)
2. [Setup](#setup)
    * [What pp_apache affects](#what-pp_apache-affects)
    * [Setup requirements](#setup-requirements)
    * [Beginning with pp_apache](#beginning-with-pp_apache)
3. [Usage](#usage)
4. [Reference](#reference)
5. [Limitations](#limitations)
6. [Development](#development)

## Description

Configure [Apache HTTP Web Server](https://httpd.apache.org/) by using [puppetlabs-apache](https://forge.puppet.com/puppetlabs/apache) and setting some parameters to strict defaults.

Configuring Apache with puppetlabs-apache is easy, and most of the defaults are sane. However, some settings, especially related to SSL could be set to some stricter defaults. This module takes care of that, but still allows you to override them.

## Setup

### What pp_apache affects

* `pp_apache` uses `puppetlabs-apache`, and sets `purge_vhost_dir` to `true` and `default_vhost` to `false`. The `mpm_module` is set to `prefork` (to support PHP).

* In every document root, access to the folder `.git` is forbidden by default. This can be overrider per `vhost`.

### Setup Requirements

* `puppetlabs-apache` is required.

### Beginning with pp_apache


## Usage

### Virtual Hosts


### SSL


### Let's Encrypt


## Reference

### Class pp_apache


#### Parameters



### Under-the-hood classes



## Limitations

This module was tested on Ubuntu 14.04, but should work with all Ubuntu versions. Only works for Apache >= 2.4.

## Development

Pull requests welcome at [https://github.com/PACKED-vzw/pp_apache](https://github.com/PACKED-vzw/pp_apache).
