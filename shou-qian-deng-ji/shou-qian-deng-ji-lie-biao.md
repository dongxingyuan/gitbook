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
        "rows": [
            {
                "linkman": "张三",
                "linkmanPhone": "**没有权限**",
                "linkmanSex": "1",
                "sellerName": "刘艳",
                "sellplace": "陵园",
                "registerUser": "管理员9",
                "registerDate": "2017-07-07",
                "linkmanId": 6,
                "linkmanDetailId": 6,
                "receiveUser": "",
                "buyFlag": "0",
                "addressFull": "",
                "layerCode": "",
                "businessNo": "",
                "userName": "李四",
                "arriveTime": "2024-09-09",
                "payStatus": "未付款",
                "payStatusId": ""
            }
        ],
        "total": 1
    }   
}
```



