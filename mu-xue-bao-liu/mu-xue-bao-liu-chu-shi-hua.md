#### 接口**路径：**

[http//localhost:8080/fsyGroupApp/interment/interface/initPermanentRetain](http:8080/fsyGroupApp/common/interface/appIndex)

---

#### 接口参数：

| 参数 | 类型 | 是否必填 | 最大长度 | 描述 | 示例值 |
| :--- | :--- | :--- | :--- | :--- | :--- |
| tokenUUID | String | 是 | 32 | 令牌 | A97D1A1BAB0F4556B214F34B9699F827 |

#### 请求示例：

```json
{
    "tokenUUID": "A82ADE66C0824A7F943C17EFEF46C35F",                 //令牌
}
```

#### 返回结果：

```json
{
    "alertFlag": true,                                               //成功标识
    "alertCode": "1"                                                 //成功编码
    "maxDays": 2,                                                    //墓穴保留最大天数
    "sexList": [                                                     //性别数据
        {
            "key": "0",
            "value": "未知的性别"
        },
        {
            "key": "1",
            "value": "男"
        },
        {
            "key": "2",
            "value": "女"
        },
        {
            "key": "9",
            "value": "未说明的性别"
        }
    ]
}
```



