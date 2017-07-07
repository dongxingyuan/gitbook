#### 接口**路径：**

[http//localhost:8080/fsyGroupApp/interment/interface/unsoldTombList](http:8080/fsyGroupApp/common/interface/appIndex)

---

#### 接口参数：

| 参数 | 类型 | 是否必填 | 最大长度 | 描述 | 示例值 |
| :--- | :--- | :--- | :--- | :--- | :--- |
| tokenUUID | String | 是 | 32 | 令牌 | A97D1A1BAB0F4556B214F34B9699F827 |
| current | Int | 是 | 10 | 页数 | 1 |
| rowCount | Int | 是 | 10 | 每页条数 | 10 |
| queryMap | Array | 否 |  | 查询条件 |  |

| 参数 | 类型 | 是否必填 | 最大长度 | 描述 | 示例值 |
| :--- | :--- | :--- | :--- | :--- | :--- |
| tombStyleName | String | 否 | 10 | 墓型 | 丰碑园 |
| buryStyleName | String | 否 | 10 | 葬式 | 艺术墓 |
| graveNo | Sting | 否 | 10 | 穴数 | 2 |
| layerCode | String | 否 | 20 | 墓穴编号 | 10001 |
| blockName | String | 否 | 20 | 墓区名称 | 归宁区 |
| sellAreaStart | String | 否 | 10 | 销售面积开始 | 1 |
| sellAreaEnd | String | 否 | 10 | 销售面积结束 | 5 |
| basePriceStart | String | 否 | 10 | 基价开始 | 1 |
| basePriceEnd | String | 否 | 10 | 基价结束 | 100000 |

#### 请求示例：

```json
{
    "tokenUUID": "A82ADE66C0824A7F943C17EFEF46C35F",
    "current": 1,
    "rowCount": 10,
    "queryMap": {
        "tokenUUID": "A82ADE66C0824A7F943C17EFEF46C35F",
        "tombStyleName": "丰碑园",
        "buryStyleName": "雕塑艺术墓",
        "graveNo": "2",
        "layerCode": "1",
        "blockName": "1",
        "sellAreaStart": "2",
        "sellAreaEnd": "5",
        "basePriceStart": "1",
        "basePriceEnd": "100000"
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



