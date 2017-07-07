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

#### 返回结果\(墓区\)：

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
        }
    ],
    "type": "1"                                                    //数据类型(1:墓区;2:墓穴)
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
    "type": "2"
}
```



