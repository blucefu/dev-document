# 接入指南

1、先根据用例算对正确的签名

例如，
access_key = 'ta3gzb9lovq424zrgzkl0o13jqc4f7yd'
secret_key = 'wud1sfd3mrdmygs1z5l8bk4glo9v9qlz'
time = 1499767733.013236

正确的签名为：
9DAF21F50797DCBC9B643B7B306188C0

如果不对，请对照接口规则-获取token直到算对签名，注意签名转为大写。

2、用curl 或 postman获取token成功

![](http://doc.shuabeiapp.com/Public/Uploads/2017-07-11/5964a694e9563.png)

仔细对照图片看和自己设置是否一致，注意body选raw， Content-type选application/json。

或者curl的方式：
```bash
curl -X POST \
  https://openapi.billbear.cn/core/v1/token \
  -H 'cache-control: no-cache' \
  -H 'content-type: application/json' \
  -H 'postman-token: 6f0c880d-7195-be8a-f8d9-12f7fcc21b0a' \
  -d '{"access_key": "ta3gzb9lovq424zrgzkl0o13jqc4f7yd","sign": "AA796D88E1F77575F8DBFD08450E5FAE","time": 1499767090.093686}'
 ```
注意time是2分钟内有效。

3、在程序上成功获取token

第二步成功了，这里主要是再次检查一下程序的一些设置，Content-type等

4、根据token去请求其他接口，这一步基本不会有啥了。

如果提示超时，一般是客户本地时间比北京时间晚了，请检查时间，我们接口对于时间要求较高，要求客户时间和服务时间误差不超过2分钟。可以指定一个将来的时间，先把token调通。

  