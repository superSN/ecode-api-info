# 获取企业用户列表

##调用方式：
* Http请求方式：POST
* 接口地址：
* http://api.1code.cc/User/user_list

##参数说明：
| 参数 | 是否必须 | 说明 |
| -- | -- | -- |
| appid | 是 | 第三方用户唯一凭证 |
| access_token | 是 | 授权Access_token，通过通用接口获取 | 
| type | 是 | 用户类型标识 |

##返回说明：
| 参数 | 类型 | 说明 |
| -- | -- | -- |
| status | int | 接口调用成功时为1，小于0时为错误码 |
| message | string | 当status<0时返回，错误提示内容 |
| user_list | array | 当调用成功时返回，用户信息数组列表 |

*用户信息数组字段说明：

| 参数 | 类型 | 说明 |
| -- | -- | -- |
| id | int | 用户ID |
| user_name | string | 用户名 |
| nickname | string | 用户昵称 |

