### 设置token签名防盗链

Token 防盗链是通过对时间有关的字符串进行签名，将时间、签名信息通过一定的方式传递给 CDN 节点服务器作为判定依据，CDN 边缘节点依据约定的算法判断来访的 URL 是否有访问权限。如果通过，执行下一步；如果不通过，响应 HTTP 403 状态码或者通过 302 跳转到其他 URL。

下面我们介绍下cdn的设置部骤：

进入cdn站点后，点击应用防火墙—>高级设置—>选择path_sign模块

输入下面的配置：

sign: _KS expire: _KE (过期时间戳 php中用time()获取 (这个时间是： Unix时间戳) key: test (key是自定义写的)

![image](https://user-images.githubusercontent.com/90588289/133750449-f9950c37-d0f7-4c7b-ab1e-6f07136cb33f.png)

图中file框框的意思是，是否带文件名

比如 /test/aaa.html

不勾path只算到目录 /test/

勾选后path算目录+文件名 /test/aaa.html

算法1不带IP验证：

md5(path+key+expire)

举个例子：

md5(/11.jpgtest1469951574)

```http://www.test.com/11.jpg?_KS=1678c4fd82b762ab304a40dab1e181ae&_KE=1469951574```

算法2带IP验证：

md5(path+key+expire+ip)

举个例子：

计算md5：md5(/11.jpgtest1469953787ip127.0.0.1) （注意计算md5是带ip的格式是： ip127.0.0.1 ,如果访问报403，注意查看自已的公网ip是什么）

访问的url: ```http://www.test.com/11.jpg?_KS=71b9c17ed08dda14d8402a78e4bc9342&_KE=1469953787ip``` (注意结尾的unix时间后面是写ip两个字符不是写ip地址)

以上两种算法也写了示例，cdn部分按上图设置就可以，接下来就是您的网站程序部分配合了。
