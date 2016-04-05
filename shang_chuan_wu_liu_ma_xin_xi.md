# 上传物流码信息

```
Http请求方式：POST
接口地址：
http://api.1code.cc/FangWei/wlInfo
```

##参数说明：
| 参数 | 是否必须 | 类型 | 说明 |
| -- | -- | -- | -- |
| appid | 是 | string |第三方用户唯一凭证 |
| access_token | 是 | string | 授权Access_token，通过通用接口获取 | 
| wlCode | 是 | string | 防伪标签的18位物流码信息 |
| brandId | 否 | string | 品牌ID，使用E码互联返回的ID |
| productId | 否 | string | 产品ID，使用E码互联返回的ID |
| dealerId | 否 | string | 客户ID，使用E码互联返回的ID |
| order_no | 否 | string | 订单编号 |

##返回说明：
| 参数 | 类型 | 说明 |
| -- | -- | -- |
| status | int | 调用成功时为1，小于0时为错误码 |
| message | string | 当status<0时返回，错误提示内容 |