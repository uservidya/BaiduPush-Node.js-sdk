BaiduPush Node.js sdk  [![Build Status](https://travis-ci.org/youxiachai/BaiduPush-Node.js-sdk.png?branch=master)](https://travis-ci.org/youxiachai/BaiduPush-Node.js-sdk) [![NPM version](https://badge.fury.io/js/baidupush.png)](http://badge.fury.io/js/baidupush) ![](https://david-dm.org/youxiachai/JPush-Node.js-sdk.png)
======================
百度云推送 Node.js 服务端 sdk

基本api 除 ios 证书尚未实现,其他全部实现.

高级api 已经全部实现
## Usage

```
npm install baidupush
```

## Example

``` js
var BaiduPush = require('baidupush');

var baiduPushClient = BaiduPush.buildBaseApi({apiKey: 'your app key', secretKey: 'your secret key'});

    var queryBody = {}
    queryBody.push_type = 3;
    queryBody.messages = {title: "hello", description: "hello world from push msg"};
    queryBody.msg_keys = 'hello';
    queryBody.message_type = 1;

    baiduPushClient.pushMsg(queryBody, function (err, body) {
      console.log(body);
    })
```

## Api Docs

[在线API文档](http://blog.gfdsa.net/BaiduPush-Node.js-sdk/api.html)

## 支持本项目
如果你觉得这个项目还不错,就请作者喝杯咖啡吧

[![](http://blog.gfdsa.net/img/pay_encourage.png)](http://me.alipay.com/youxilua)
