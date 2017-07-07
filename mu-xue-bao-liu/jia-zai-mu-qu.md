#### 接口**路径：**

[http//localhost:8080/fsyGroupApp/interment/interface/getTombArea](http:8080/fsyGroupApp/common/interface/appIndex)

---

#### 接口参数：

| 参数 | 类型 | 是否必填 | 最大长度 | 描述 | 示例值 |
| :--- | :--- | :--- | :--- | :--- | :--- |
| tokenUUID | String | 是 | 32 | 令牌 | A97D1A1BAB0F4556B214F34B9699F827 |
| objId | String | 否 | 10 | 墓区ID | 1 |
| filterType | String | 否 | 1 | 过滤类型 | 1:查询可售;2:查询可划地 |

#### 请求示例：

```json
json={
    "tokenUUID": "A82ADE66C0824A7F943C17EFEF46C35F",                 //令牌
}
&objId="1"                                                           //墓区ID
&filterType="1"                                                      //过滤类型
```

#### 返回结果：

```json
{
    "alertFlag": true,                                               //成功标识
    "alertCode": "1"                                                 //成功编码
    "list": [                                                        //墓区信息
        {
            "id": "149",                                             //墓区ID
            "name": "归宁园",                                         //墓区名称
            "rowNo": "",                                             //行数
            "columnNo": "",                                          //列数
            "isBottom": "0"                                          //是否底级
        },
        {
            "id": "152",
            "name": "长青园",
            "rowNo": "",
            "columnNo": "",
            "isBottom": "0"
        }
    ],
    "type": "1"
}
```

```json
{
    "alertFlag": true,
    "alertCode": "1",
    "columnNo": 9,
    "rowNo": 9,
    "onSiteFlag": "1"
    "list": [
        {
            "gridId": 338800,
            "tombId": 710253,
            "rowNo": 0,
            "columnNo": 0,
            "path": "大蜀山文化陵园归宁园1区GN1-1",
            "tombPath": "大蜀山文化陵园归宁园1区GN1-1",
            "status": 4,
            "layerCode": "归宁047010101",
            "graveNo": 2,
            "baseSum": "2100.00",
            "displayNo": "GN1-1",
            "buildFlag": "2",
            "onSaleFlag": "2",
            "mergeFlag": false,
            "mergeMainFlag": false,
            "rowLastFlag": false,
            "payStatus": "0",
            "payStatusHtml": "<br/>(未付)",
            "sellArea": "3.700"
        }
    ],
    "type": "2"
}
```



