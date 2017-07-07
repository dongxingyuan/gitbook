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
    "bean": {                                                        //墓穴信息
        "tombPath": "大蜀山文化陵园长青园1区CQ1_2",                    //墓穴位置
        "layerCode": "长青047010102",                                //墓穴编号  
        "graveNo": 2,                                                //穴数
        "baseSum": "46200.00",                                       //墓穴售价
        "displayNo": "CQ1-2",                                        //显示编号
        "mergeFlag": false,                                        
        "mergeMainFlag": false,                                    
        "rowLastFlag": false,                                        //是否最后一行
        "basicPrice": "45000.00",                                    //基价
        "id": "710416",                                              //墓穴ID
        "buryStyleName": "丰碑园",                                    //墓型名称
        "tombStyleName": "商品艺术墓",                                //葬式
        "supplierName": "",                                          //供应商
        "tombMaterial": "大理石",                                     //石材料
        "useArea": "0.000",                                          //使用面积
        "sellArea": "4.500",                                         //销售面积
        "factArea": "0.000",                                         //净墓面积
        "greenArea": "0.000",                                        //绿化面积
        "roadArea": "0.000",                                         //道路面积
        "buildArea": "0.000",                                        //建造面积
        "shareArea": "0.000",                                        //公摊面积
        "lowestPrice": "0.00",                                       //最低价格
        "innerHeight": "0.00",                                       //内经高度
        "innerLength": "0.00",                                       //内经长度
        "innerWidht": "0.00"                                         //内经宽度
    },
    "files": [                                                        //墓穴照片
           {
            "id": "1",                                                //照片ID
            "tombId": "1",                                            //墓穴ID
            "fileName": "墓穴照片",                                    //照片名称                     
            "filePath": "http://aliyuncs.com/2017-07/f58.jpg"         //照片路径
        }
    ]                                                    
}
```



