### 自动申请部署好ssl证书

SSL（Secure Sockets Layer），中文名为“安全套接层协议层”，即 HTTPS 传输加密协议，是 HTTP 超文本传输协议的升级版，利用身份鉴证与高强度数据加密双重手段，为客户端(浏览器) 到服务器端之间搭建一条加密通道，保证数据在传输过程中不被窃取或篡改，确保机密信息的保密性、完整性和可信性

自动开通ssl证书。

1：在站点里[添加域名](/SharkCdnDoc/CDN管理/站点列表/添加域名.md)，并做好解析到cname或者直接解析到cdn节点ip,否则申请证书不会通过，然后勾选该条记录，并点击自动证书，如下图:

![image](https://user-images.githubusercontent.com/90959714/137085798-e7d38f7c-2f61-4bc9-b43d-5e815560815d.png)

2.选择好域名厂商和填写好从域名商那边获取的api_key，再点击获取，就会开始自动申请证书

![image](https://user-images.githubusercontent.com/90959714/137088175-b8a59da4-c2fb-4db2-b146-6edc82c51966.png)

3.然后过几分钟点开SSL管理可以查看证书状态，如下图就是申请成功

查看：[SSL管理](/SharkCdnDoc/CDN管理/SSL管理/SSL管理.md)

![image](https://user-images.githubusercontent.com/90588289/133742072-8292f24d-9de1-4e01-b00e-7673f74d2595.png)
