Cdn三种添加ssl证书的方法

一、第一种在站点设置中添加：

点击CDN管理--站点列表--需要添加ssl证书的站点名--站点设置--https设置--打开

![image](https://user-images.githubusercontent.com/90588289/135225142-e272930e-3cc1-4aad-82ac-7e096f6d093a.png)

加入证书后点提交

![image](https://user-images.githubusercontent.com/90588289/135227442-d45e53b2-4601-4b4a-a87c-a817b765aaec.png)

可以点检测功能检查证书是否有效，打勾说明证书是有效的，打叉说明证书无效

二. 第二种是在域名记录里添加：

点击CDN管理--站点列表--需要添加ssl证书的站点名--记录管理--选择要添加ssl证书的域名--修改--填写好ssl证书和密钥

如下图点击，添加证书后点确定即可

![image](https://user-images.githubusercontent.com/90959714/137092749-c057c96b-3805-4cfd-b10c-5e4905eecad5.png)

三. 第三种是用sharkcdn自动获取证书功能：

1.在站点里[添加域名](/SharkCdnDoc/CDN管理/站点列表/添加域名.md)，然后勾选该条记录，并点击修改，如下图:

![image](https://user-images.githubusercontent.com/90959714/159394757-3861a8a7-4b7b-4f41-8c63-300107633323.png)

如下图显示就申请成功了

2.自动申请证书也有可能失败，失败可先检查下解析是否做好，然后重新申请

![image](https://user-images.githubusercontent.com/90588289/133751396-6df1d446-a0c0-4576-b5d1-99e866a5c390.png)

[SSL管理](/SharkCdnDoc/CDN管理/SSL管理/SSL管理.md)

以上就是三种添加证书的方式

备注：无
