

    
##### 简要描述

- 获取下载的版本和url

##### 请求URL
- ` /api/sdk/{vhost}/download/info `
  
##### 请求方式
- GET

##### 参数

|参数名|必选|类型|说明|
|:----    |:---|:----- |-----   |
|vhost |是  |string |站点名   |


##### 返回示例 

![image](https://user-images.githubusercontent.com/90588289/133775220-d27777b8-bbd5-42a3-bf67-2e72e2a5e50d.png)

##### 返回参数说明 

|参数名|类型|说明|
|:-----  |:-----|-----                           |
|version |int   |版本号  |
|url |string   |链接  |

##### 备注 

- **响应码**：
 - 200 成功
 - 401 未授权
 - 403 防火墙限制
 - 404 没找到路径



