

    
##### 简要描述

- 检测域名ssl是否生效

##### 请求URL
- ` /api/site/{vhost}/domain/{domain}/check `

##### 请求方式
- GET

##### 参数

|参数名|必选|类型|说明|
|:----    |:---|:----- |-----   |
|vhost |是  |string |站点名   |
|domain |是  |string | 域名    |

##### 返回示例 

![image](https://user-images.githubusercontent.com/90588289/133868435-f984559c-cd10-4c5c-a690-cc673724da16.png)

##### 返回参数说明 

无

##### 备注 

- **响应码**：
 - 200 成功
 - 401 未授权
 - 403 防火墙限制
 - 404 没找到路径



