#### 接口**路径：**

[http//localhost:8080/fsyGroupApp/interment/interface/initConfirm](http:8080/fsyGroupApp/common/interface/appIndex)

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
    "unbuyReasonList": [                                             //未购买原因
        {
            "id": 1,
            "isValidate": "1",
            "name": "价格贵",
            "indexNo": 0
        },
        {
            "id": 2,
            "isValidate": "1",
            "name": "没有满意的",
            "indexNo": 0
        },
        {
            "id": 3,
            "isValidate": "1",
            "name": "去其他墓园看看",
            "indexNo": 0
        },
        {
            "id": 4,
            "isValidate": "1",
            "name": "再考虑考虑",
            "indexNo": 0
        },
        {
            "id": 5,
            "isValidate": "1",
            "name": "客户不想说",
            "indexNo": 0
        },
        {
            "id": 6,
            "isValidate": "1",
            "name": "其他",
            "indexNo": 0
        }
    ],
}
```



