### 一键自动申请部署好ssl证书

SSL（Secure Sockets Layer），中文名为“安全套接层协议层”，即 HTTPS 传输加密协议，是 HTTP 超文本传输协议的升级版，利用身份鉴证与高强度数据加密双重手段，为客户端(浏览器) 到服务器端之间搭建一条加密通道，保证数据在传输过程中不被窃取或篡改，确保机密信息的保密性、完整性和可信性

一键自动开通ssl证书。只需要一键操作就能自动帮您申请部署好ssl证书，有效期三个月，到期前三天会自动续期，如果申请失败会自动重试三次

1：在站点里[添加域名](/SharkCdnDoc/CDN管理/站点列表/添加域名.md)，并做好解析到cname或者直接解析到cdn节点ip,否则申请证书不会通过，然后点修改，如下图:

![image](https://user-images.githubusercontent.com/90588289/135227802-add4dbdf-a39e-4555-8923-e6b515621da0.png)

2.点击添加好的域名的右边的修改按钮--自动获取，就会开始自动申请证书

![image](https://user-images.githubusercontent.com/90588289/133742058-1f6a9513-ae1f-4138-9fba-1d9df0c95a9f.png)

3.然后过几分钟点开SSL管理可以查看证书状态，如下图就是申请成功

查看：[SSL管理](/SharkCdnDoc/CDN管理/SSL管理/SSL管理.md)

![image](https://user-images.githubusercontent.com/90588289/133742072-8292f24d-9de1-4e01-b00e-7673f74d2595.png)
