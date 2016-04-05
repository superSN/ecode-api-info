# 产品添加或修改

```
Http请求方式：POST
接口地址：
http://api.1code.cc/Product/edit
```

##参数说明：
| 参数 | 是否必须 | 类型 | 说明 |
| -- | -- | -- | -- |
| appid | 是 | string |第三方用户唯一凭证 |
| access_token | 是 | string | 授权Access_token，通过通用接口获取 | 
| productId | 修改时必须，添加时不得带此参数 | string | E码互联分配的产品ID |
| name | 是 | string | 产品名称 |
| brandId | 是 | string | 品牌全局唯一标识名 |
| model | 否 | string | 产品型号 |
| Unit | 否 | string | 产品单位 |

##返回说明：
| 参数 | 类型 | 说明 |
| -- | -- | -- |
| status | int | 调用成功时为1，小于0时为错误码 |
| message | string | 当status<0时返回，错误提示内容 |
| productId | string | 当添加时返回，E码互联产品全局唯一标识ID |