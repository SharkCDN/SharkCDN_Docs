

    
##### 简要描述

- 获取域名cname

##### 请求URL
- ` /api/site/{vhost}/domain/{domain}/{host}/cname `
  
##### 请求方式
- GET

##### 参数

|参数名|必选|类型|说明|
|:----    |:---|:----- |-----   |
|vhost |是  |string |站点   |
|domain |是  |string | 域名    |
|host     |是  |string | 地址    |

##### 返回示例 

![image](https://user-images.githubusercontent.com/90588289/133868417-036afa77-3174-4add-965f-80ce90b58458.png)

##### 返回参数说明 

无

##### 备注 

- **响应码**：
 - 200 成功
 - 401 未授权
 - 403 防火墙限制
 - 404 没找到路径



