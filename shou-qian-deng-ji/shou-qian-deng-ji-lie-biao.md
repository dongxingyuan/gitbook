#### 接口**路径：**

[http//localhost:8080/fsyGroupApp/interment/interface/receptionList](http:8080/fsyGroupApp/common/interface/appIndex)

---

#### 接口参数：

| 参数 | 类型 | 是否必填 | 最大长度 | 描述 | 示例值 |
| :--- | :--- | :--- | :--- | :--- | :--- |
| tokenUUID | String | 是 | 32 | 令牌 | A97D1A1BAB0F4556B214F34B9699F827 |
| current | Int | 是 | 10 | 页数 | 1 |
| rowCount | Int | 是 | 10 | 每页条数 | 10 |
| queryMap | Array | 否 |  | 查询条件 | {"createUser":9} |

| 参数 | 类型 | 是否必填 | 最大长度 | 描述 | 示例值 |
| :--- | :--- | :--- | :--- | :--- | :--- |
| createUser | Int | 是 | 10 | 每页条数 | 10 |

#### 请求示例：

```json
{
    "tokenUUID": "A82ADE66C0824A7F943C17EFEF46C35F",                //令牌
    "current": 1,                                                   //页数
    "rowCount": 10,                                                 //每页条数
    "queryMap": {                                                   //查询条件
        "createUser": 9                                             //创建人ID
    }
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
                "linkman": "张三",                                    //联系人
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
                "arriveTime": "2024-09-09",                             //来园时间
                "payStatus": "未付款",                                  //付款状态
                "payStatusId": "0"                                     //0:未付款;1:定金;3:全款 
            }
        ],
        "total": 1
    }   
}
```



