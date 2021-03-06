# 活动支付渠道

**简要描述：**

- 活动支付渠道接口。

**请求URL：**
- `/base_data/v2/act_pay_brand`

**请求方式：**
- GET

**参数：**

- 同[参数规定](http://doc.liexiong.cc/#/%E6%8E%A5%E5%8F%A3%E8%A7%84%E5%88%99/%E5%8F%82%E6%95%B0%E8%A7%84%E5%AE%9A)

**返回示例：**

```json
{
    "msg":"success",
    "status":"200",
    "sync_time":"1469586420332999",
    "data":[
         {
            "create_time": "2017-05-22 10:21:55.395000",
            "id": 339,
            "name": "微信",
            "category": "第三方",
            "status": 1,
            "update_time": "2017-05-22 10:21:55.395000"
        },
        {
            "create_time": "2017-05-22 10:21:55.390000",
            "id": 175,
            "name": "银联",
            "category": "卡组织",
            "status": 1,
            "update_time": "2017-05-22 10:21:55.390000"
        },
        {
            "create_time": "2017-05-22 10:21:55.384000",
            "id": 162,
            "name": "银行",
            "category": "网银",
            "status": 1,
            "update_time": "2017-05-22 10:21:55.384000"
        }
    ]
}
```

**返回参数说明：** 
 
|参数名|类型|说明|
|:-----  |:-----|-----|
|id |int   |对象唯一标识  |
|name |string   |活动支付渠道|
|category|string | 渠道所属类型 |
|status|int|状态（1：正常，0：无效）|
|create_time|string|创建时间|
|update_time|string|更新时间|



