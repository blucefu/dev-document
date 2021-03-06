# 活动商户关系

**简要描述：**

- 这里唯一标示可以使用id，也可以使用活动id和商户id，推荐使用后者，因为风险更小。

**请求URL：**
- `/base_data/v1/act_shop_ref`

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
            "act_id":5419,
            "create_time":"2016-05-24 18:59:58.223999",
            "id":452,
            "shop_id":158576,
            "status":1,
            "update_time":"2016-05-24 18:59:58.224020"
        },
        {
            "act_id":5419,
            "create_time":"2016-05-24 18:59:58.223999",
            "id":451,
            "shop_id":158582,
            "status":1,
            "update_time":"2016-05-24 18:59:58.224019"
        },
        .....
    ]
}
```

**返回参数说明：** 

|参数名|类型|说明|
|:-----  |:-----|-----                           |
|id |int   |对象唯一标示  |
|act_id |int   |活动id  |
|shop_id |int   |商户id  |
|status|int|状态（1：正常，0：无效）|
|create_time|string|创建时间|
|update_time|string|更新时间|
