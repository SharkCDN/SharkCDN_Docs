

    
##### 简要描述

- 获取Token

##### 请求URL
- ` /api/user/login/token `
  
##### 请求方式
- POST

##### 参数

|参数名|必选|类型|说明|
|:----    |:---|:----- |-----   |
|sign |是  |string |签名验证，加密方式：MD5(MD5(uid+skey)+time)，长度32位   |
|time |是  |integer |秒级时间戳，注：请求到达时间相差不能超过5分钟   |
|uid |是  |integer |用户ID   |
|vhost |是  |string |站点名   |


##### 返回示例 

![image](https://user-images.githubusercontent.com/90588289/135231853-e74e61f5-61bf-4ae4-868a-0fdc5df3bc45.png)


##### 返回参数说明 

|参数名|类型|说明|
|:----    |:----- |-----   |
|sessionId |string |Token值   |
|account |integer |uid   |

##### 备注 
200 成功

201 创建

401 未授权

403 防火墙限制

404 没找到路径





