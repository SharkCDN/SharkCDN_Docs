

    
##### 简要描述

- 修改域名，ip，权重信息

##### 请求URL
- ` /api/site/{vhost}/domain/{domain}/{host} `
  
##### 请求方式
- PUT

##### 参数

|参数名|必选|类型|说明|
|:----    |:---|:----- |-----   |
|vhost |是  |string |站点名   |
|domain |是  |string | 域名   |
|host     |是  |string | 地址   |
|weight |是  |int |权重 |

##### 返回示例 

![image](https://user-images.githubusercontent.com/90588289/133868392-5eebffd4-0c3b-41c6-9c5b-352540dd68ef.png)

##### 返回参数说明 

无

##### 备注 

- **响应码**：
 - 200 成功
 - 201 创建
 - 401 未授权
 - 403 防火墙限制
 - 404 没找到路径



