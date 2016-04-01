# 用户登录验证
```
Http请求方式：POST
接口地址：
http://api.1code.cc/User/login_confirm
```

##参数说明：
| 参数 | 是否必须 | 说明 |
| -- | -- | -- |
| appid | 是 | 第三方用户唯一凭证 |
| access_token | 是 | 授权Access_token，通过通用接口获取 | 
| user_name | 是 | 用户名称 |
| password | 是 | 用户密码经MD5加密 |

##返回说明：
| 参数 | 类型 | 说明 |
| -- | -- | -- |
| status | int | 用户验证成功时为1，小于0时为错误码 |
| message | string | 当status<0时返回，错误提示内容 |