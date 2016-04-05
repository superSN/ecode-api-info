# 品牌添加或修改

```
Http请求方式：POST
接口地址：
http://api.1code.cc/Brand/edit
```

##参数说明：
| 参数 | 是否必须 | 类型 | 说明 |
| -- | -- | -- | -- |
| appid | 是 | string |第三方用户唯一凭证 |
| access_token | 是 | string | 授权Access_token，通过通用接口获取 | 
| name | 是 | string | 品牌名称 |
| value | 修改信息时必须 | string | 品牌的标识编号，带此参数则为更新操作，不带则为添加操作 |

##返回说明：
| 参数 | 类型 | 说明 |
| -- | -- | -- |
| status | int | 调用成功时为1，小于0时为错误码 |
| message | string | 当status<0时返回，错误提示内容 |
| value | string | 当添加时返回，品牌全局唯一标识名原样返回 |


