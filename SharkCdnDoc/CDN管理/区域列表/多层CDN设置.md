### 多层CDN设置

点击CDN管理--区域列表--配置--多层CDN设置

![image](https://user-images.githubusercontent.com/90588289/135242521-eb523fd7-4eca-4b2e-81d1-f53f7c60a6a2.png)

![image](https://user-images.githubusercontent.com/90588289/133736086-4b1c0c0a-cbd3-41d1-bdda-c149a26017af.png)

备注：这个签名主要是认证的作用，多层cdn在传送真实ip时，黑客如果通过中间层cdn节点发送假ip，源就不能得到真实的ip。这个签名认证可以让中间层cdn节点认证上层cdn节点ip的来源
