# 福寿园公墓系统移动端APP接口文档

## 请求接口参数数名称：json

```json
json = {"objId":"1", "tokenUUID":"92DC677B77214DD0BA454A759FA7837C"}
```

## 错误代码：

| 编号 | 描述 |
| :--- | :--- |
| 40001 | 令牌失效 |
| 0 | 系统错误 |

## 错误示例：

```json
{
    "alertFlag": false,                    //出错标识
    "alertCode": "40001",                  //错误代码
    "alertMessage": "令牌失效！"            //错误信息
}
```

## 成功代码：

| 编号 | 描述 |
| :--- | :--- |
| 1 | 成功 |

## 成功示例：

```json
{
    "alertFlag": true,                     //成功标识
    "alertCode": "1",                  //成功代码
    "alertMessage": "保存成功！"            //成功信息
}
```



