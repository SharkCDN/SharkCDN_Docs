

    
##### 简要描述

- 修改源ip

##### 请求URL
- ` /api/site/{vhost}/srcip `
  
##### 请求方式
- PUT

##### 参数

|参数名|必选|类型|说明|
|:----    |:---|:----- |-----   |
|delPort |是  |true |不需要端口  |
|newIP |是  |string | 修改后ip   |
|oldIP     |是  |string | 原ip   |

##### 返回示例 

![image](https://user-images.githubusercontent.com/90588289/133867622-fcc1c8ad-7899-4fc7-a39b-383f5a8bad0e.png)

##### 返回参数说明 

无

##### 备注 

- **响应码**：
 - 200 成功
 - 201 创建
 - 401 未授权
 - 403 防火墙限制
 - 404 没找到路径



