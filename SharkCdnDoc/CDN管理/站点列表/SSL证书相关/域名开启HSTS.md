### 域名开启HSTS

HSTS介绍：

国际互联网工程组织IETE正在推行一种新的Web安全协议HTTP Strict Transport Security（HSTS）

采用HSTS协议的网站将保证浏览器始终连接到该网站的HTTPS加密版本，不需要用户手动在URL地址栏中输入加密地址。

该协议将帮助网站采用全局加密，用户看到的就是该网站的安全版本。

HSTS的作用是强制客户端（如浏览器）使用HTTPS与服务器创建连接。服务器开启HSTS的方法是，当客户端通过HTTPS发出请求时，在服务器返回的超文本传输协议响应头中包含Strict-Transport-Security字段。非加密传输时设置的HSTS字段无效。

比如，```https://xxx``` 的响应头含有Strict-Transport-Security: max-age=31536000; includeSubDomains。这意味着两点：

在接下来的一年（即31536000秒）中，浏览器只要向xxx或其子域名发送HTTP请求时，必须采用HTTPS来发起连接。比如，用户点击超链接或在地址栏输入 ```http://xxx/``` ，浏览器应当自动将 http 转写成 https，然后直接向 ```https://xxx/``` 发送请求。

在接下来的一年中，如果 xxx 服务器发送的TLS证书无效，用户不能忽略浏览器警告继续访问网站

在cdnbest站点里面添加一条域名记录，如图

![image](https://user-images.githubusercontent.com/90588289/135227802-add4dbdf-a39e-4555-8923-e6b515621da0.png)

点击上图修改图标增加ssl证书，如下图所示ssl证书增加成功，可参考自动获取ssl证书教程：[一键自动申请部署好ssl证书](/SharkCdnDoc/CDN管理/站点列表/SSL证书相关/一键自动申请部署好ssl证书.md)

![image](https://user-images.githubusercontent.com/90588289/133751796-5b1c7238-c1f2-42f9-8daa-299b1a68817d.png)

最后开启HSTS功能，也是点击修改图标进入，如下图

![image](https://user-images.githubusercontent.com/90588289/133751809-d530c272-42d7-4f83-a674-ba6a4c65ea74.png)

开启HSTS后，检查是否成功，我们访问域名，按F12查看，响应头出现Strict-Transport-Security：max-age=2592000（表示HSTS有效期，单位秒），则表示设置成功。
如下图

![image](https://user-images.githubusercontent.com/90588289/133751823-022818ac-8145-4946-ad24-788a07f926af.png)

HSTS有效期可以自定义
进入站点设置，选择https设置，HSTS有效期，单位为月，点击提交，如下图

![image](https://user-images.githubusercontent.com/90588289/133751848-41ef6b72-3db9-423b-9d6a-eaccfdd3e184.png)

设置自定义有效期后，可以访问域名，按F12查看是否自定义成功，如下图

![20200427112253a04ecfec361d1f474940b2473e06d04f](https://user-images.githubusercontent.com/90588289/134650004-f7244497-1ca7-4857-9aff-ec1874c88182.png)

备注：无
