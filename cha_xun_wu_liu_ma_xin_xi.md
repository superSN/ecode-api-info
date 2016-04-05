# 查询物流码信息

```
Http请求方式：GET
接口地址：
http://api.1code.cc/FangWei/wlInfo
```

##参数说明：
| 参数 | 是否必须 | 类型 | 说明 |
| -- | -- | -- | -- |
| appid | 是 | string |第三方用户唯一凭证 |
| access_token | 是 | string | 授权Access_token，通过通用接口获取 | 
| wlCode | 是 | string | 防伪标签的18位物流码信息 |


##返回说明：
| 参数 | 类型 | 说明 |
| -- | -- | -- |
| status | int | 调用成功时为1，小于0时为错误码 |
| message | string | 当status<0时返回，错误提示内容 |
| ecid | int | 企业ID，使用E码互联返回的ID |
| brandId | string | 品牌ID，使用E码互联返回的ID |
| brand_name | string | 品牌名称 |
| brand_img | string | 品牌图片Url |
| productId | int | 产品ID，使用E码互联返回的ID |
| product_name | string | 产品名称 |
| product_img | string | 产品图片Url |
| dealerId | string | 客户ID，使用E码互联返回的ID |
| dealer_name | string | 客户名称 |
| wlCode | string | 18位物流码 |
| order_no | string | 防伪下单订单编号 |