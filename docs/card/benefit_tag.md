# 权益标签

**简要描述：**

- 卡片权益标签接口。

**请求URL：**
- `/base_data/v2/benefit_tag`

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
            "name_cn": "洗牙",
            "level": 2,
            "parent_id": 122,
            "status": 1,
            "update_time": "2017-05-22 10:21:55.395000"
        },
        {
            "create_time": "2017-05-22 10:21:55.390000",
            "id": 175,
            "name_cn": "保障",
            "level": 1,
            "parent_id": -1,
            "status": 1,
            "update_time": "2017-05-22 10:21:55.390000"
        },
        {
            "create_time": "2017-05-22 10:21:55.384000",
            "id": 162,
            "name_cn": "意外险",
            "level": 2,
            "parent_id": 175,
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
|name_cn |string   |权益名称|
|level|int | 权益级别 |
|parent_id | int | 父级别id |
|status|int|状态（1：正常，0：无效）|
|create_time|string|创建时间|
|update_time|string|更新时间|



