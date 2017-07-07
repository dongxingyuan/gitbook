#### 接口**路径：**

[http//localhost:8080/fsyGroupApp/interment/interface/getTombArea](http:8080/fsyGroupApp/common/interface/appIndex)

---

#### 接口参数：

| 参数 | 类型 | 是否必填 | 最大长度 | 描述 | 示例值 |
| :--- | :--- | :--- | :--- | :--- | :--- |
| tokenUUID | String | 是 | 32 | 令牌 | A97D1A1BAB0F4556B214F34B9699F827 |
| objId | String | 否 | 10 | 墓区ID | 1 |
| filterType | String | 否 | 1 | 过滤类型 | 1:查询可售;2:查询可划地 |

#### 请求示例：

```json
json={
    "tokenUUID": "A82ADE66C0824A7F943C17EFEF46C35F",                 //令牌
}
&objId="1"                                                           //墓区ID
&filterType="1"                                                      //过滤类型
```

#### 返回结果：

```json
{
    "alertFlag": true,                                               //成功标识
    "alertCode": "1"                                                 //成功编码
    "alertMessage": "保存成功"                                        //成功信息
}
```



