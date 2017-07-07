#### 接口**路径：**

[http//localhost:8080/fsyGroupApp/interment/interface/receComfirm](http:8080/fsyGroupApp/common/interface/appIndex)

---

#### 接口参数：

| 参数 | 类型 | 是否必填 | 最大长度 | 描述 | 示例值 |
| :--- | :--- | :--- | :--- | :--- | :--- |
| tokenUUID | String | 是 | 32 | 令牌 | A97D1A1BAB0F4556B214F34B9699F827 |
| name | String | 是 | 10 | 联系人姓名 | 张三 |
| sex | String | 是 | 10 | 联系人性别 | 1 |
| phoneNo | String | 否 | 20 | 电话号码 | 021-8888888 |
| mobileNo | String | 是 | 20 | 手机号码 | 1388888888 |
| sellerId | String | 是 | 10 | 营销人ID | 1 |
| userName | String | 是 | 10 | 使用人 | 李四 |
| arriveTime | String | 是 | 10 | 来园时间 | 2018-08-08 |
| remark | String | 否 | 50 | 备注 | 备注 |

#### 请求示例：

```json
{
    "tokenUUID": "A82ADE66C0824A7F943C17EFEF46C35F",                 //令牌
    "linkmanId": "张三",                                              //售前联系人ID
    "receiveFlag": "0",                                               //是否购买
    "unbuyReason": "1",                                               //未购买原因
    "unbuyReasonOther": "其他原因"                                     //其他原因
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



