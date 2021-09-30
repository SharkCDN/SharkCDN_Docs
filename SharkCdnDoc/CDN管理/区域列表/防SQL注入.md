### 防SQL注入

点击CDN管理--区域列表--配置--防SQL注入

![image](https://user-images.githubusercontent.com/90588289/135242583-4a99ed36-7127-41fc-a9e0-e60b8d3a581b.png)

![image](https://user-images.githubusercontent.com/90588289/133735783-76c31b06-be24-42db-a41f-52c23df07958.png)

备注代码如下：

参数名称：param

参数值：'.*[; ]?((or)|(insert)|(select)|(union)|(update)|(delete)|(replace)|(create)|(drop)|(alter)|(grant)|(load)|(show)|(exec))[\s(]
