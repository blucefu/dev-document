# 卡片反馈

**简要描述：**

- 如果在卡片查询列表中没有找用户的卡片，则需要通过这个接口把用户的卡片信息反馈给烈熊系统。

**请求URL：**
- `/callback/v1/card`

**请求方式：**
- POST

**参数：**
```json
	{
            'token': 'TGHCPOQuSyiZ6dbbEp361utP4f3X39DPCDvMeOElfexHsMohdt2adPVvWwnKwxZN',
            "first_code": "12345678",
            "last_code": "1234",
            'b64_image': b64_str
        }
```

**请求参数说明：** 

|参数名|类型|说明|
|:-----  |:-----|-----                           |
|token |str   |token  |
|first_code |string   |卡bin前八位  |
|last_code |string   |卡bin后四位  |
|b64_image |string   | 图片信息base64格式话之后的字符串，可以参考[图片/BASE64转换](http://tool.oschina.net/encrypt?type=4) |

**返回示例：**

```json
{
    "msg":"success",
    "status":"200",
    "sync_time":"1469586420332999",
}
```
