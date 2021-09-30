

    
##### 简要描述

- 修改域名ssl，负载均衡等信息

##### 请求URL
- ` /api/site/{vhost}/domain/setting/{id} `
  
##### 请求方式
- PUT

##### 参数

|参数名|必选|类型|说明|
|:----    |:---|:----- |-----   |
|vhost |是  |string |站点   |
|id |是  |int | id号    |
|errorTryTime |否  |string |错误重试时间，单位s   |
|forceSsl |否  |int |开启强制,0:关闭1：开启    |
|hash |否  |string |负载均衡策略(ip_hash:ip哈希url_hash:url哈希random：随机)   |
|hsts |否  |int |开启HSTS,0:关闭1：开启    |
|maxErrorCount |否  |string |连续错误次数   |
|portMap |否  |int |端口映射,0:关闭1：开启|
|sslCsr |否  |string |ssl证书   |
|sslKey |否  |string |ssl 秘钥    |

##### 返回示例 

![image](https://user-images.githubusercontent.com/90588289/133868721-019ef466-3607-493e-b0b3-c91744985b86.png)

##### 返回参数说明 

无

##### 备注 

- 更多返回错误代码请看首页的错误代码描述



