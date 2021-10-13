Cdn三种添加ssl证书的方法

一、第一种在站点设置中添加：

点击CDN管理--站点列表--需要添加ssl证书的站点名--站点设置--https设置--打开

![image](https://user-images.githubusercontent.com/90588289/135225142-e272930e-3cc1-4aad-82ac-7e096f6d093a.png)

加入证书后点提交

![image](https://user-images.githubusercontent.com/90588289/135227442-d45e53b2-4601-4b4a-a87c-a817b765aaec.png)

可以点检测功能检查证书是否有效，打勾说明证书是有效的，打叉说明证书无效

二. 第二种是在域名记录里添加：

1.在站点里[添加域名](/SharkCdnDoc/CDN管理/站点列表/添加域名.md)，并做好解析到cname或者直接解析到cdn节点ip,否则申请证书不会通过，然后勾选该条记录，并点击自动证书，如下图:

![image](https://user-images.githubusercontent.com/90959714/137085798-e7d38f7c-2f61-4bc9-b43d-5e815560815d.png)

2.选择好域名厂商和填写好从域名商那边获取的api_key，再点击获取，就会开始自动申请证书

![image](https://user-images.githubusercontent.com/90959714/137088175-b8a59da4-c2fb-4db2-b146-6edc82c51966.png)

三. 第三种是用sharkcdn自动获取证书功能：

开启申请ssl证书前域名要做好cname解析记录，或者域名直接解析到了节点的ip也行

如下图点击开启自动申请ssl证书的功能

![image](https://user-images.githubusercontent.com/90588289/133751382-f5222a12-ab59-420f-9eaa-14b4f81a60d6.png)

如下图显示就申请成功了，到期后会自动续期，（注：独立主控用户开通这个功能需联系客服开通）

自动申请证书也有可能失败，失败可先检查下解析是否做好，然后重新申请

![image](https://user-images.githubusercontent.com/90588289/133751396-6df1d446-a0c0-4576-b5d1-99e866a5c390.png)

[SSL管理](zh-cn/SharkCdnDoc/CDN管理/SSL管理/SSL管理.md)

以上就是三种添加证书的方式

备注：无
