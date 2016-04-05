# 获取品牌列表

```
Http请求方式：POST
接口地址：
http://api.1code.cc/Brand/brand_list
```

##参数说明：
| 参数 | 是否必须 | 类型 | 说明 |
| -- | -- | -- | -- |
| appid | 是 | string |第三方用户唯一凭证 |
| access_token | 是 | string | 授权Access_token，通过通用接口获取 | 

##返回说明：
| 参数 | 类型 | 说明 |
| -- | -- | -- |
| status | int | 调用成功时为1，小于0时为错误码 |
| message | string | 当status<0时返回，错误提示内容 |
| brand | array | 品牌列表 |


##品牌数组结构：

| 参数 | 类型 | 说明 |
| -- | -- | -- |
| id | int | 品牌编号 |
| name | string | 品牌名称 |
| value | array | 品牌全局唯一标识名 |
