### Cdn配置强制ssl跳转

如何配置强制ssl跳转

点击CDN管理--站点列表--需要添加ssl证书的站点名--记录管理--选择要添加ssl证书的域名--修改--强制ssl

登陆用户站点，点击下图图标：

![image](https://user-images.githubusercontent.com/90588289/135227802-add4dbdf-a39e-4555-8923-e6b515621da0.png)

2.如下图添加证书和开启强制ssl即可

![image](https://user-images.githubusercontent.com/90588289/133751613-08af0c95-8110-4de7-a903-e9442f65f9bd.png)

hsts解释和作用：

国际互联网工程组织IETF正在推行一种新的Web安全协议HTTP Strict Transport Security（HSTS）

采用HSTS协议的网站将保证浏览器始终连接到该网站的HTTPS加密版本，不需要用户手动在URL地址栏中输入加密地址。

该协议将帮助网站采用全局加密，用户看到的就是该网站的安全版本。

HSTS的作用是强制客户端（如浏览器）使用HTTPS与服务器创建连接。服务器开启HSTS的方法是，当客户端通过HTTPS发出请求时，在服务器返回的超文本传输协议响应头中包含Strict-Transport-Security字段。非加密传输时设置的HSTS字段无效。

比如，```https://xxx``` 的响应头含有Strict-Transport-Security: max-age=2592000; includeSubDomains。这意味着两点：

在接下来的一个月（即2592000秒）中，浏览器只要向xxx或其子域名发送HTTP请求时，必须采用HTTPS来发起连接。比如，用户点击超链接或在地址栏输入 ```http://xxx/``` ，浏览器应当自动将 http 转写成 https，然后直接向 ```https://xxx/``` 发送请求。

简单一句话，开启hsts后，第一次访问通过http后，之后的访问都会自动跳转到https访问，所以hsts也有强制ssl的效果

在站点设置中设置301跳转到https的方法：[Cdn如何站点设置中添加301跳转](/SharkCdnDoc/CDN管理/站点列表/Cdn如何站点设置中添加301跳转.md)

备注：无
