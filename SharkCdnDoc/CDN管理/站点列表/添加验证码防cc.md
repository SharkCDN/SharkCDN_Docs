### 添加验证码防cc

登陆站点—>点应用防火墙—>防cc设置—>选择自定义，如图： 图中频率按自已的需求设置

![image](https://user-images.githubusercontent.com/90588289/133749864-de5a3a32-3afc-4994-b239-3e27bce4abc3.png)

内容添加如下代码 注：下面两段代码直接复制，代码中间的空行要保留，否则代码添加无效

```
  HTTP/1.1 200 OK
  Content-Type: text/html; charset=utf-8
  Connection: close
  Cache-Control: no-cache,no-store

  <html><body>
  <img src='/KANGLE_CCIMG.php?k={{session_key}}'>
  <form action='/KANGLE_CCIMG.php' method='get'>
  <input name='k' value='{{session_key}}' type='hidden'>
  <input name='v' value=/>
  <input type='submit'/>
  </form>
  </body></html>
```
