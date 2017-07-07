## 接口**路径：**

[http:8080/fsyGroupApp/common/interface/appIndex](http:8080/fsyGroupApp/common/interface/appIndex)

---

## 接口参数：

| 参数 | 类型 | 是否必填 | 最大长度 | 描述 | 示例值 |
| :--- | :--- | :--- | :--- | :--- | :--- |
| tokenUUID | String | 是 | 32 | 令牌 | A97D1A1BAB0F4556B214F34B9699F827 |

#### 请求示例

```json
json = {
    "tokenUUID": "A82ADE66C0824A7F943C17EFEF46C35F"    //令牌
}
```

#### 返回结果

```json
{
    "msgs": [                                                        //用户消息
        {
            "id": "9",                                               //消息ID
            "title": "福寿园国际集团第一期",                           //标题
            "content": "福寿园国际集团第一期",                         //内容
            "createDate": "2017-07-03",                              //发送时间
            "acceptDate": "2017-06-30",                              //接收时间
            "userName": "管理员1",                                    //发送人
            "headUrl": "http://aliyuncs.com/2017-07/f58.jpg",        //头像
            "status": "1"                                            //消息状态 (0:未接收1:已接收)
        }
    ],
    "alertFlag": true,
    "notices": [
        {
            "id": "1",
            "title": "福寿园国际集团第一期“福寿人体验营”",
            "content": "6月26日，福寿园国际集团第一期“福寿人体验营”培训在上海举行。",
            "createDate": "2017-06-30",
            "createUser": "管理员1",
            "endDate": "2017-07-31",
            "headUrl": "http://aliyuncs.com/2017-07/f58.jpg"
        }
    ],
    "userBean": {
        "userId": "9",
        "userNo": "9999",
        "loginName": "9999",
        "userName": "管理员9",
        "unitName": "福寿园集团",
        "deptName": "销售部",
        "headImage": "2017-07/415.jpg",
        "headUrl": "http://aliyuncs.com/2017-07/415.jpg"
    },
    "images": [
        {
            "id": "2",
            "title": "dasdsad",
            "url": "http://aliyuncs.com/2017-07/fda.jpg"
            "content": "2"
        },
        {
            "id": "1",
            "title": "dasda",
            "url": "http://aliyuncs.com/2017-07/310.jpg",
            "content": "1"
        }
    ],
    "alertCode": "1"
}
```



