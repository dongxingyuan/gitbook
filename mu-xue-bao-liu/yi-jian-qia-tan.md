#### 接口**路径：**

[http//localhost:8080/fsyGroupApp/interment/interface/retainToReg](http:8080/fsyGroupApp/common/interface/appIndex)

---

#### 接口参数：

| 参数 | 类型 | 是否必填 | 最大长度 | 描述 | 示例值 |
| :--- | :--- | :--- | :--- | :--- | :--- |
| tokenUUID | String | 是 | 32 | 令牌 | A97D1A1BAB0F4556B214F34B9699F827 |
| objId | String | 是 | 10 | 保留ID | 1 |
| type | String | 是 | 10 | 洽谈类型 | 2 |

#### 请求示例：

```json
{
    "tokenUUID": "A82ADE66C0824A7F943C17EFEF46C35F",                //令牌
    "objId": "1",                                                     //保留ID
    "type": "2",                                                      //洽谈类型(1:暂时保留洽谈;2:墓穴保留洽谈)
}
```

#### 返回结果：

```json
{
    "alertFlag": true,                                               //成功标识
    "alertCode": "1"                                                 //成功编码
    "bean": {
        "tombId": "710262",
        "layerCode": "归宁047010201",
        "tombPath": "大蜀山文化陵园归宁园1区GN2-1",
        "graveNo": "2",
        "basicPrice": "1000.00",
        "sellplaceId": "1",
        "sellplaceName": "陵园",
        "sellerId": "4",
        "sellerName": "韩洋",
        "linkMan": "张三",
        "linkManSex": "9",
        "linkManPhoneNo": "18662528814",
        "linkManMobileNo": "18662528814",
        "addressProvince": "340000",
        "addressCity": "340100",
        "addressCountty": "340102",
        "addressProvinceName": "安徽省",
        "addressCityName": "合肥市",
        "addressCounttyName": "瑶海区",
        "addressDetail": "新村路",
        "userName": "李四,未知",
        "userSex": "9,9",
        "userGraveType": "0,0",
        "userCertificateId": "",
        "userCertificateNo": "",
        "bookSaveId": "",
        "bookingId": "7411"
    },
}
```



