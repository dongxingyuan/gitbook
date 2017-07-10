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
    "objId": "1",                                                   //保留ID
    "type": "2",                                                    //洽谈类型(1:暂时保留洽谈;2:墓穴保留洽谈)
}
```

#### 返回结果：

```json
{
    "alertFlag": true,                                               //成功标识
    "alertCode": "1"                                                 //成功编码
    "bean": {
        "tombId": "710262",                                          //墓穴ID
        "layerCode": "归宁047010201",                                //墓穴编号
        "tombPath": "大蜀山文化陵园归宁园1区GN2-1",                    //墓穴位置
        "graveNo": "2",                                              //穴数
        "basicPrice": "1000.00",                                     //墓穴基价
        "sellplaceId": "1",                                          //营销地点ID
        "sellplaceName": "陵园",                                     //营销地点名称
        "sellerId": "4",                                             //营销人ID
        "sellerName": "韩洋",                                        //营销人名称
        "linkMan": "张三",                                           //联系人
        "linkManSex": "9",                                           //联系人性别
        "linkManPhoneNo": "18662528814",                             //联系人电话
        "linkManMobileNo": "18662528814",                            //联系人手机
        "addressProvince": "340000",                                 //省编码
        "addressCity": "340100",                                     //市编码
        "addressCountty": "340102",                                  //区编码
        "addressProvinceName": "安徽省",                              //省名称
        "addressCityName": "合肥市",                                  //市名称
        "addressCounttyName": "瑶海区",                               //区名称
        "addressDetail": "新村路",                                    //详细地址
        "userName": "李四,未知",                                      //使用人
        "userSex": "9,9",                                            //使用人性别
        "userGraveType": "0,0",                                      //墓穴类型
        "userCertificateId": "",                                     //使用人证件类型
        "userCertificateNo": "",                                     //使用人证件编码
        "bookSaveId": "",                                            //暂时保留ID
        "bookingId": "7411"                                          //墓穴保留ID
    },
}
```



