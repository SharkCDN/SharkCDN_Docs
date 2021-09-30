

    
##### 简要描述

- getDomainCname

##### 请求URL
- ` /api/site/{vhost}/domain/{domain}/cname `
  
##### 请求方式
- GET

##### 参数

|参数名|必选|类型|说明|
|:----    |:---|:----- |-----   |
|vhost |是  |string |站点   |
|domain |是  |string | 域名    |

##### 返回示例 

![image](https://user-images.githubusercontent.com/90588289/133868455-b8c66a84-e6cb-4c05-8ac7-7ae8de5fc999.png)

##### 返回参数说明 

无

##### 备注 

- **响应码**：
 - 200 成功
 - 401 未授权
 - 403 防火墙限制
 - 404 没找到路径



