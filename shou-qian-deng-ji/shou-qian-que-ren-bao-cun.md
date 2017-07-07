#### 接口**路径：**

[http//localhost:8080/fsyGroupApp/interment/interface/receComfirm](http:8080/fsyGroupApp/common/interface/appIndex)

---

#### 接口参数：

| 参数 | 类型 | 是否必填 | 最大长度 | 描述 | 示例值 |
| :--- | :--- | :--- | :--- | :--- | :--- |
| tokenUUID | String | 是 | 32 | 令牌 | A97D1A1BAB0F4556B214F34B9699F827 |
| linkmanId | Int | 是 | 10 | 售前联系人ID | 1 |
| receiveFlag | String | 是 | 1 | 是否购买 | 0 |
| unbuyReason | Int | 否 | 10 | 未购买原因 | 1 |
| unbuyReasonOther | String | 否 | 50 | 其他原因 | 其他原因 |
| remark | String | 否 | 50 | 备注 | 备注 |

#### 请求示例：

```json
{
    "tokenUUID": "A82ADE66C0824A7F943C17EFEF46C35F",                 //令牌
    "linkmanId": "1",                                              //售前联系人ID
    "receiveFlag": "0",                                              //是否购买
    "unbuyReason": "1",                                              //未购买原因
    "unbuyReasonOther": "其他原因"                                    //其他原因
    "remark": "备注"                                                  //备注
}
```

#### 返回结果：

```json
{
    "alertFlag": true,                                               //成功标识
    "alertCode": "1"                                                 //成功编码
    "alertMessage": "保存成功"                                        //成功信息
}
```



