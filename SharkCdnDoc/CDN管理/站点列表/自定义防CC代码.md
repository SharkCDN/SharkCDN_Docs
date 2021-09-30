-  **自定义防CC代码**

防CC代码模式有以下几种： 注：复制代码时代码中间一定要空一行，如下格式：
1.http redirect（普通）
```
HTTP/1.1 302 FOUND  
Connection: keep-alive  
Location: {{url}}  

<html><body><a href="{{url}}">continue</a></body></html>  
```
2.html redirect
```
HTTP/1.1 200 OK  
Content-Type: text/html; charset=utf-8  
Connection: keep-alive  
Cache-Control: no-cache,no-store  

<html><head><meta http-equiv="refresh" content="0;url={{url}}"></head><body><a href="{{url}}">continue</a></body></html>
```
3.js plain
```
HTTP/1.1 200 OK  
Content-Type: text/html; charset=utf-8  
Connection: keep-alive  
Cache-Control: no-cache,no-store  

<html><body><script language="javascript">window.location="{{url}}";</script><a href="{{url}}">continue</a></body></html>
```
4.js concat
```
HTTP/1.1 200 OK  
Content-Type: text/html; charset=utf-8  
Connection: keep-alive  
Cache-Control: no-cache,no-store  

<html><body><script language="javascript">window.location="{{murl}}";</script></body></html>
```
5.js revert(复杂)
```
HTTP/1.1 200 OK  
Content-Type: text/html; charset=utf-8  
Connection: keep-alive  
Cache-Control: no-cache,no-store  

<html><body><script language="javascript">{{revert:url}};window.location=url;</script></body></html>
```
6.html manual
```
HTTP/1.1 200 OK  
Content-Type: text/html; charset=utf-8  
Connection: keep-alive  
Cache-Control: no-cache,no-store  

<html><body><a href="{{url}}">continue</a></body></html>  
```
7.deny
```
HTTP/1.1 200 OK  
Content-Type: text/html; charset=utf-8  
Connection: keep-alive  
Cache-Control: no-cache,no-store  

<html><body>try again later</body></html>
```
以上的模式都可以登陆节点的3311后台查看,如何登陆节点3311后台查看：
登陆后点击请求控制-->标记模块-->anti_cc模块
