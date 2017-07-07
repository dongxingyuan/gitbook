#### 接口**路径：**

[http//localhost:8080/fsyGroupApp/interment/interface/getTombInfo](http:8080/fsyGroupApp/common/interface/appIndex)

---

#### 接口参数：

| 参数 | 类型 | 是否必填 | 最大长度 | 描述 | 示例值 |
| :--- | :--- | :--- | :--- | :--- | :--- |
| tokenUUID | String | 是 | 32 | 令牌 | A97D1A1BAB0F4556B214F34B9699F827 |
| objId | String | 否 | 10 | 墓区ID | 1 |

#### 请求示例：

```json
json={
    "tokenUUID": "A82ADE66C0824A7F943C17EFEF46C35F",                 //令牌
}
&objId="1"                                                           //墓穴ID
```

#### 返回结果\(墓区\)：

```json
{
    "alertFlag": true,                                               //成功标识
    "alertCode": "1"                                                 //成功编码
    "bean": {
        "tombPath": "大蜀山文化陵园长青园1区CQ1_2",
        "layerCode": "长青047010102",
        "graveNo": 2,
        "baseSum": "46200.00",
        "displayNo": "CQ1-2",
        "mergeFlag": false,
        "mergeMainFlag": false,
        "rowLastFlag": false,
        "basicPrice": "45000.00",
        "id": "710416",
        "buryStyleName": "丰碑园",
        "tombStyleName": "商品艺术墓",
        "supplierName": "",
        "tombMaterial": "大理石",
        "useArea": "0.000",
        "sellArea": "4.500",
        "factArea": "0.000",
        "greenArea": "0.000",
        "roadArea": "0.000",
        "buildArea": "0.000",
        "shareArea": "0.000",
        "lowestPrice": "0.00",
        "innerHeight": "0.00",
        "innerLength": "0.00",
        "innerWidht": "0.00"
    },
    "files": [
           {
            "id": "大蜀山文化陵园长青园1区CQ1_2",
            "tombId": "长青047010102",
            "fileName": 2,
            "filePath": "46200.00"
        },
    ]                                                     //数据类型(1:墓区;2:墓穴)
}
```

#### 返回结果\(墓穴\)：

```json
{
    "alertFlag": true,                                              //成功标识
    "alertCode": "1",                                               //成功代码
    "columnNo": 9,                                                  //列
    "rowNo": 9,                                                     //行
    "onSiteFlag": "1"                                               //是否可划地墓区(1:可以;2:不可以)
    "list": [                                                       //墓穴信息
        {
            "gridId": 338800,                                       //各位ID
            "tombId": 710253,                                       //墓穴ID
            "rowNo": 0,                                             //行号
            "columnNo": 0,                                          //列号
            "path": "大蜀山文化陵园归宁园1区GN1-1",                   //墓穴位置
            "tombPath": "大蜀山文化陵园归宁园1区GN1-1",               //墓穴位置
            "status": 4,                                            //墓穴状态
            "layerCode": "归宁047010101",                           //墓穴编号
            "graveNo": 2,                                           //穴数
            "baseSum": "2100.00",                                   //墓穴售价
            "displayNo": "GN1-1",                                   //显示编号
            "buildFlag": "2",                                       //建墓状态(0:未建;1:再建;2:建成)
            "onSaleFlag": "2",                                      //上账状态(0:未上账;1:已上账;2:上账审批通过)
            "mergeFlag": false,                                     //合并标识(true:合并;false:不合并)
            "mergeMainFlag": false,                                 //合并格位中的主对象(true:是;false:否)
            "rowLastFlag": false,                                   //每行最后一个标志(true:是;false:否)
            "payStatus": "0",                                       //结算状态(0:未付;1:定金;3:全款)
            "payStatusHtml": "<br/>(未付)",                         //结算状态
            "sellArea": "3.700"                                     //销售面积  
        }
    ],
    "type": "2"                                                     //数据类型(1:墓区;2:墓穴)
}
```



