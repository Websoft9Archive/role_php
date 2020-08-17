# CHANGELOG

## To do

1. 性能调优
2. Ubuntu支持
3. yum install php72w-pecl-imagick error
4. webtatic源版本跟不上，考虑用：remi,plesk等源替换

## Logs

### Bug Fixes

* 2020-08-17  modify vhost_dir: /etc/httpd/vhost to vhost_dir: /etc/httpd/conf.d in php_runtime_meta.yml
* 2020-05-31  add check php-fpm service, check version to file
* 2020-05-31  yum install php72w-pecl-imagick error, add skip_broken=yes
* 2020-03-03  max_input_vars=2000

### Features

* 2020-08-15  add php.service soft link to php-fpm.service
* 2020-02-14  rename php-fpm to php for this repository
