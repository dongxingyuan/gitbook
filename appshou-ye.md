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
    "msgs": [
        {
            "id": "9",
            "title": "福寿园国际集团第一期",
            "content": "福寿园国际集团第一期",
            "createDate": "2017-07-03",
            "acceptDate": "2017-06-30",
            "userName": "管理员1",
            "headUrl": "http://aliyuncs.com/2017-07/f58.jpg",
            "status": "1"
        }
    ],
    "alertFlag": true,
    "notices": [
        {
            "id": "1",
            "title": "福寿园国际集团第一期“福寿人体验营”",
            "content": "6月26日，福寿园国际集团第一期“福寿人体验营”培训在上海举行。来自集团各地分公司的首期36名学员入营，在三天半的时间里开展教学培训。通过培训，员工们进一步对福寿园理念、思维方法进行槽刻，并与讲师、同学们充分交流互动，增进对公司和行业的整体认知。",
            "createDate": "2017-06-30",
            "createUser": "管理员1",
            "endDate": "2017-07-31",
            "headUrl": "http://fsygroup-bucket.oss-cn-shanghai.aliyuncs.com/2017-07/201707051435512017070545131a53ea69c-5dca-4315-bdf1-855c7a9d6f58.jpg?Expires=1499416110&OSSAccessKeyId=LTAIRzvB6DDs7SS5&Signature=cp5mvLUVm5NrvOFCvBbPa8nJTYA%3D"
        },
        {
            "id": "2",
            "title": "福寿园国际集团第一期“福寿人体验营”",
            "content": "6月26日，福寿园国际集团第一期“福寿人体验营”培训在上海举行。来自集团各地分公司的首期36名学员入营，在三天半的时间里开展教学培训。通过培训，员工们进一步对福寿园理念、思维方法进行槽刻，并与讲师、同学们充分交流互动，增进对公司和行业的整体认知。",
            "createDate": "2017-06-30",
            "createUser": "管理员1",
            "endDate": "2017-07-31",
            "headUrl": "http://fsygroup-bucket.oss-cn-shanghai.aliyuncs.com/2017-07/201707051435512017070545131a53ea69c-5dca-4315-bdf1-855c7a9d6f58.jpg?Expires=1499416110&OSSAccessKeyId=LTAIRzvB6DDs7SS5&Signature=cp5mvLUVm5NrvOFCvBbPa8nJTYA%3D"
        }
    ],
    "userBean": {
        "userId": "9",
        "userNo": "9999",
        "loginName": "9999",
        "userName": "管理员9",
        "unitName": "福寿园集团",
        "deptName": "销售部",
        "headImage": "2017-07/景观介绍31compress2017070339010adf27aeb-9163-4460-82ec-91fdaee17415.jpg",
        "headUrl": "http://fsygroup-bucket.oss-cn-shanghai.aliyuncs.com/2017-07/%E6%99%AF%E8%A7%82%E4%BB%8B%E7%BB%8D31compress2017070339010adf27aeb-9163-4460-82ec-91fdaee17415.jpg?Expires=1499416110&OSSAccessKeyId=LTAIRzvB6DDs7SS5&Signature=QFMaRRVV8vo79iO4un83l9qQdDI%3D"
    },
    "images": [
        {
            "id": "2",
            "title": "dasdsad",
            "url": "http://fsygroup-bucket.oss-cn-shanghai.aliyuncs.com/2017-07/jxplay20170703422025df03b97-ab08-41b9-b87c-48d65bf92fda.jpg?Expires=1499416110&OSSAccessKeyId=LTAIRzvB6DDs7SS5&Signature=VNI1IbqseFMbfzFT1qLejCmrVEI%3D",
            "content": "2"
        },
        {
            "id": "1",
            "title": "dasda",
            "url": "http://fsygroup-bucket.oss-cn-shanghai.aliyuncs.com/2017-07/22017070352390a0315b3e-9672-4b2e-9bae-42eacd5ec310.jpg?Expires=1499416110&OSSAccessKeyId=LTAIRzvB6DDs7SS5&Signature=6bTBkrgaH%2BJm%2FH5JZDhTUg9ZCfQ%3D",
            "content": "1"
        }
    ],
    "alertCode": "1"
}
```



