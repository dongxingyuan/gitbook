#### 接口**路径：**

[http//localhost:8080/fsyGroupApp/interment/interface/saveTemporaryRetain](http:8080/fsyGroupApp/common/interface/appIndex)

---

#### 接口参数：

| 参数 | 类型 | 是否必填 | 最大长度 | 描述 | 示例值 |
| :--- | :--- | :--- | :--- | :--- | :--- |
| tokenUUID | String | 是 | 32 | 令牌 | A97D1A1BAB0F4556B214F34B9699F827 |
| sellerId | Int | 是 | 10 | 营销人呢ID | 1 |
| linkManName | String | 是 | 1 | 联系人 | 张三 |
| userName | Int | 是 | 10 | 使用人 | 李四 |
| tombId | Int | 是 | 50 | 墓穴ID | 1 |
| bookTime | Int | 是 | 50 | 保留时间 | 2 |

#### 请求示例：

```json
{
    "tokenUUID": "A82ADE66C0824A7F943C17EFEF46C35F",                 //令牌
    "sellerId": 1,                                                   //营销人ID
    "linkManName": "张三",                                            //联系人
    "userName": "李四",                                               //使用人
    "tombId": 1                                                       //墓穴ID
    "bookTime": 2                                                     //保留时间
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



