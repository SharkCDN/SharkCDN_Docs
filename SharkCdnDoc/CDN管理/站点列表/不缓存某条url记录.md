### 不缓存某条url记录

如果需要单独对一条url记录不缓存，配置方法如下：

在站点设置的缓存策略，添加规则，如下图输入，注意缓存的时间要设为0

![image](https://user-images.githubusercontent.com/90588289/133747127-d201b04e-6088-4881-9ae0-e3f07280d560.png)

2.配置好后，我们可以验证下X-Cache显示MISS就是没有缓存了

X-Cache：MISS from yn-190

![image](https://user-images.githubusercontent.com/90588289/135233456-26764dbb-cb31-4612-9d9e-8d4a5200739b.png)
