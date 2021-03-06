# server-sdk-php

Rong Cloud Server SDK in PHP for Composer.

## API文档
- 官方文档(https://www.rongcloud.cn/docs/server_sdk_api/)

## 使用教程
* 请参考 example 上面提供了所有的 API 接口的调用用例。

## 安装

* 推荐通过 composer 安装，使用 composer.json 声明依赖，或者运行下面的命令：

```bash
$ composer require lawmil/rongcloud
```

* 直接下载安装，SDK 没有依赖其他第三方库，可直接下载引入使用。

## 使用方法
```php
$appKey = 'appKey';
$appSecret = 'appSecret';
...
    $rongCloud = new RongCloud($appKey,$appSecret);
    $user = [
        'id'=> '用户id',
        'name'=> '用户名称',
        'portrait'=> '用户头像'
    ];
    $token = $rongCloud->getUser()->register($user);
...
```

## 代码许可

The MIT License (MIT).详情见 [License文件](https://github.com/qiniu/php-sdk/blob/master/LICENSE).