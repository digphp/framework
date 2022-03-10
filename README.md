# framework

PHP应用开发框架

## 安装

``` bash
composer require digphp/framework
```

然后，需要加上：

``` json
{
    "scripts": {
        "post-package-install": "DigPHP\\Framework\\Script::onInstall",
        "post-package-update": "DigPHP\\Framework\\Script::onUpdate",
        "pre-package-uninstall": "DigPHP\\Framework\\Script::onUninstall"
    }
}
```

## 用例

``` php
\DigPHP\Framework\Framework::run();
```
