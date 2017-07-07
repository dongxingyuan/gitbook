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
    "page": {                                                        //分页数据
        "current": 1,                                                //当前页号
        "rowCount": 10,                                              //每页条数
        "rows": [                                                    //分页数据
            {
                "bookingId": "1",                                   //墓穴保留ID
                "tombPath": "大蜀山文化陵园归宁园1区GN4-3",            //墓穴位置
                "sellerplace": "陵园",                               //营销地点
                "seller": "韩洋",                                    //营销人
                "bookDay": "2",                                     //保留时间
                "startTime": "2017-07-07 20:45:01",                  //开始时间
                "endTime": "2017-07-07 22:45:01",                    //结束时间
                "linkMan": "张三",                                    //联系人
                "userName": "李四",                                   //使用人              
                "bookNo": "B20170707001",                             //墓穴保留编号
                "businessFlag": "0"                                   //洽谈标识(0:未洽谈;1:已洽谈)
            }
        ],
        "total": 1                                                     //总条数
    }   
}
```



