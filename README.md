Ansible Role: php
=========

本 Role 用于在PHP运行环境下安装 [PHP](https://www.php.net/)。

## Requirements

运行本 Role，请确认符合如下的必要条件：

| **Items**      | **Details** |
| ------------------| ------------------|
| Operating system | CentOS7.x Ubuntu18.04 AmazonLinux |
| Python 版本 | Python2  |
| Python 组件 |    |
| Runtime |  |


## Related roles

本 Role 在运行时需要确保已经运行：common。以下为例：

```
roles:
    - {role: role_common, tags: "role_common"}
    - {role: role_php-fpm, tags: "role_php-fpm"}
```


## Variables

本 Role 主要变量以及使用方法如下：

| **Items**      | **Details** | **Format**  | **是否初始化** |
| ------------------| ------------------|-----|-----|
| php_version | [ 5.6, 7.0, 7.1, 7.2（默认）, 7.3 ] | 字符串 | 否 |
| php_ioncube | [Trure, Fasle（默认）] | 布尔 | 否|
| php_configuration_extras | - | 列表 | 否|



## Example

```
php_configuration_extras:
  - name: max_execution_time
    value: "800"
```

## FAQ


