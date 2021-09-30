### DNS接入

1.在dns平台解析域名，并获得如下信息：

DNS主域名：输入需要解析的域名(一个主控只用输入一个国际域名)

2.在帐户设置中生成API_KEY

UID: 这个uid是dns平台自动生成的
API_KEY： API_KEY需要点击生成key,然后点保存。看下图

3.进入cdn的系统设置，点击DNS接入。如下图打开高级设置选择DNS提供者，输入接入方域名(DNS平台域名)
![image](https://user-images.githubusercontent.com/90588289/135214704-264ef469-7bb6-4795-953f-3573a6fc7961.png)

把相关信息输入系统设置-dns接入，然后点测试连接，可测试是否对接成功

默认TTL：600

UID与API_KEY可在DNS平台中找到

备注：点击dns修复可以重新同步因网络原因没有及时更新同步的配置信息到dns解析
