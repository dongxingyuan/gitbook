#### 接口**路径：**

[http//localhost:8080/fsyGroupApp/interment/interface/initTemporaryRetain](http:8080/fsyGroupApp/common/interface/appIndex)

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

#### 返回结果\(墓区\)：

```json
{
    "alertFlag": true,                                               //成功标识
    "alertCode": "1"                                                 //成功编码
    "maxHours": 2                                                    //暂时保留最大时间
}
```





