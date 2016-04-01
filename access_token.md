# 获取access_token

access_token是公众号的全局唯一票据，调用各接口时都需使用access_token。开发者需要进行妥善保存。access_token的存储至少要保留512个字符空间。access_token的有效期目前为2个小时，需定时刷新，重复获取将导致上次获取的access_token失效。


### 接口调用说明：
* 接用方式：GET
* 接口地址：
* http://api.1code.cc/General/token?grant_type=client_credential&appid=APPID&secret=APPSECRET

### 参数说明：
| 参数| 是否必须 | 说明 |
| -- | -- | -- |
| grant_type | 必须 | 获取access_token填写client_credential |
| appid | 必须 | 第三方用户唯一凭证 |
| secret | 必须 | 第三方用户唯一凭证密钥，即appsecret |


### 接口返回说明
调用成功，会返回下述JSON数据包：
```json
{"access_token":"ACCESS_TOKEN","expires_in":7200}
```




