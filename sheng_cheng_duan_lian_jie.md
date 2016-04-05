# 生成短链接

```
Http请求方式：POST
接口地址：
http://api.1code.cc/ShortUrl/create
```

##参数说明：
| 参数 | 是否必须 | 类型 | 说明 |
| -- | -- | -- | -- |
| appid | 是 | string |第三方用户唯一凭证 |
| access_token | 是 | string | 授权Access_token，通过通用接口获取 | 
| url | 是 | string | 待生成的长链接，请使用http_encode编码后传入 |

##返回说明：
| 参数 | 类型 | 说明 |
| -- | -- | -- |
| status | int | 用户验证成功时为1，小于0时为错误码 |
| message | string | 当status<0时返回，错误提示内容 |
| url | string | 当 status=1时返回，对应的短链接地址 |