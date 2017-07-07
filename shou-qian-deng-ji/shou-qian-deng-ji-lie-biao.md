#### 接口**路径：**

[http//localhost:8080/fsyGroupApp/interment/interface/receptionList](http:8080/fsyGroupApp/common/interface/appIndex)

---

#### 接口参数：

| 参数 | 类型 | 是否必填 | 最大长度 | 描述 | 示例值 |
| :--- | :--- | :--- | :--- | :--- | :--- |
| tokenUUID | String | 是 | 32 | 令牌 | A97D1A1BAB0F4556B214F34B9699F827 |
| current | Int |  |  |  |  |
| rowCount | Int |  |  |  |  |
| queryMap |  |  |  |  |  |

#### 请求示例：

```json
{
    "tokenUUID": "A82ADE66C0824A7F943C17EFEF46C35F"                 //令牌
}
```

#### 返回结果：

```json
{
    "alertFlag": true,                                               //成功标识
    "alertCode": "1"
    "msgs": [                                                        //用户消息
        {
            "id": "9",                                               //消息ID
            "title": "福寿园国际集团第一期",                           //消息标题
            "content": "福寿园国际集团第一期",                         //消息内容
            "createDate": "2017-07-03",                              //发送时间
            "acceptDate": "2017-06-30",                              //接收时间
            "userName": "管理员1",                                    //发送人
            "headUrl": "http://aliyuncs.com/2017-07/f58.jpg",        //头像
            "status": "1"                                            //消息状态 (0:未接收1:已接收)
        }
    ],
    "notices": [                                                     //通知
        {
            "id": "1",                                                //通知ID 
            "title": "福寿园国际集团第一期“福寿人体验营”",               //通知标题
            "content": "6月26日，福寿园国际集团第一期培训在上海举行",     //通知内容
            "createDate": "2017-06-30",                               //发送时间
            "createUser": "管理员1",                                   //发送人
            "endDate": "2017-07-31",                                  //截至时间
            "headUrl": "http://aliyuncs.com/2017-07/f58.jpg"          //头像
        }
    ],
    "userBean": {                                                     //用户信息
        "userId": "9",                                                //用户ID
        "userNo": "9999",                                             //用户工号
        "loginName": "9999",                                          //用户登录名称
        "userName": "管理员9",                                         //用户姓名
        "unitName": "福寿园集团",                                      //单位名称
        "deptName": "销售部",                                          //部门名称
        "headImage": "2017-07/415.jpg",                               //头像
        "headUrl": "http://aliyuncs.com/2017-07/415.jpg"              //头像显示路径
    },
    "images": [                                                       //首页图片
        {
            "id": "2",                                                //图片ID
            "title": "dasdsad",                                       //标题
            "url": "http://aliyuncs.com/2017-07/fda.jpg"              //图片路径
            "content": "2"                                            //内容
        }
    ],
}
```



