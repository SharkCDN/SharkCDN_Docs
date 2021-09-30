### Cdn配置四层协议端口转发

Cdn配置四层协议端口转发就是将外网主机的IP地址的一个端口映射到内网中一台机器，提供相应的服务。当用户访问该IP的这个端口时，服务器自动将请求映射到对应局域网内部的机器上。

1.安装好节点后初始化节点要选择四层协议



2.增加四层分组：

![image](https://user-images.githubusercontent.com/90588289/135419732-74ecc527-2724-4fae-aa82-cf8fc7f391c5.png)

3.点击进入四层分组，添加四层节点ip，把44分组里的四层节点添加到右边启用

![image](https://user-images.githubusercontent.com/90588289/135420428-85e3d69d-4c48-4e77-9c67-abdefad188ce.png)

4.建立产品，选择四层协议



5.新增站点，选择四层产品

![image](https://user-images.githubusercontent.com/90588289/135421552-091be721-1f96-469e-ac03-63a4ade9026d.png)

6.点击进入站点，点端口映射，添加端口是要映射的端口，ip是写源机的ip

查看节点的ip可以点击显示节点

![image](https://user-images.githubusercontent.com/90588289/135421335-12a009a9-18b2-4808-b5d1-851b275acf64.png)

添加后，在节点3311会显示侦听了1980端口

![image](https://user-images.githubusercontent.com/90588289/135416774-6217d0fd-617e-4e3d-8bb2-a2bb6553a23d.png)

完成上面操作，就可以通过节点ip 1980端口ssh登陆到3.3.3.3这台机器了

注：如果登陆不上，用telnet测下端口是不是通的，格式：telnet ip 端口
