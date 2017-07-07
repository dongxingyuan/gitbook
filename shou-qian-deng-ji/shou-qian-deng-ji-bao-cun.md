#### 接口**路径：**

[http//localhost:8080/fsyGroupApp/interment/interface/saveReception](http:8080/fsyGroupApp/common/interface/appIndex)

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
    "tokenUUID": "A82ADE66C0824A7F943C17EFEF46C35F",                //令牌
    "name": "张三",
    "sex": "0",
    "phoneNo": "021-8888888",
    "mobileNo": "1388888888",
    "sellerId": "1",
    "userName": "李四",
    "arriveTime": "2018-08-08",
    "remark": "备注"
}
```

#### 返回结果：

```json
{
    "alertFlag": true,                                               //成功标识
    "alertCode": "1"                                                 //成功编码
    "page": {                                                        //分页数据
        "current": 1,                                                //当前页号
        "rowCount": 10,                                              //每页条数
        "rows": [                                                    //返回数据
            {
                "linkman": "张三",                                     //联系人
                "linkmanPhone": "**没有权限**",                        //联系手机
                "linkmanSex": "1",                                    //联系人性别
                "sellerName": "刘艳",                                  //营销人
                "sellplace": "陵园",                                   //营销地点
                "registerUser": "管理员9",                             //登记人
                "registerDate": "2017-07-07",                          //登记时间
                "linkmanId": 6,                                        //售前联系人ID
                "linkmanDetailId": 6,                                  //售前联系人详情ID 
                "receiveUser": "",                                     //确认人
                "buyFlag": "0",                                        //购买标识(0:未购买;1:已购买)
                "addressFull": "",                                     //联系人详细地址
                "layerCode": "",                                       //墓穴编号
                "businessNo": "",                                      //业务编号
                "userName": "李四",                                     //使用人
                "arriveTime": "2024-09-09",                            //来园时间
                "payStatus": "未付款",                                  //付款状态
                "payStatusId": "0"                                     //0:未付款;1:定金;3:全款 
            }
        ],
        "total": 1                                                     //总条数
    }   
}
```



