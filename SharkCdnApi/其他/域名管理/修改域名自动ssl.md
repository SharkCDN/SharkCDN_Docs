

    
##### 简要描述

- 修改域名自动ssl

##### 请求URL
- ` /api/site/{vhost}/domain/ssl/{id}/{status} `
  
##### 请求方式
- POST 

##### 参数

|参数名|必选|类型|说明|
|:----    |:---|:----- |-----   |
|vhost |是  |string |站点   |
|id |是  |string | 域名id    |
|status     |否  |string | 自动ssl状态，0：关闭1:开启    |

##### 返回示例 

![image](https://user-images.githubusercontent.com/90588289/133868735-ba6eaada-ffb0-45f7-b443-30d7ff3cd8d9.png)

##### 返回参数说明 

无

##### 备注 

- 更多返回错误代码请看首页的错误代码描述



