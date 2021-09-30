### cdn配置部骤流程图:

![image](https://user-images.githubusercontent.com/90588289/134606462-0cc3014d-b8c1-416d-8f88-291e4753e271.png)

### 第一步： 配置DNS接入

![image](https://user-images.githubusercontent.com/90588289/135219128-0307d63b-1f19-4586-b4b8-774fb313c0c0.png)

接入文档：[DNS接入](/SharkCdnDoc/系统管理/系统设置/DNS接入.md)

### 第二步：增加区域和增加节点

(1).新增一个区域

![image](https://user-images.githubusercontent.com/90588289/135218995-96147a55-f335-437c-af71-cec54f698b5c.png)

立即配置：[添加区域](/SharkCdnDoc/CDN管理/区域列表/添加区域.md)

(2). 点击CDN管理---节点列表---新增节点 会弹出节点的安装程序

![image](https://user-images.githubusercontent.com/90588289/135219488-b6c450d5-b9b4-4be7-871d-b7db669123cc.png)

立即配置：[添加节点](/SharkCdnDoc/CDN管理/节点列表/添加节点.md)

(3).linux服务器，直接复制下图脚本命令运行。

![image](https://user-images.githubusercontent.com/90588289/135222152-5aaae70a-5f88-4c03-9983-93d79d1ab661.png)

(4).安装成功后,节点会出现在待初始化列表,点击初始化

![image](https://user-images.githubusercontent.com/90588289/135227694-03701cfb-a3d4-4856-95fa-1c232976ba0f.png)

区域：选择要初始化节点到哪个区域

名称：设置节点的名字，只能用英文和数字。

节点类型：选择默认的边缘节点就行了。 中间节点是多层CDN功能。

备注：可留空

![image](https://user-images.githubusercontent.com/90588289/135226750-4bccdf78-5c75-403d-bc17-4091fb64abd8.png)

(5). 初始化成功后，节点会显示在对应的区域中，显示版本号则表示节点连接主控后台正常

![image](https://user-images.githubusercontent.com/90588289/135227937-f16e33ac-af04-4de7-83f6-7f0417383703.png)

### 第三步：分组解析

在分组解析中启用相应的节点ip(分组可自行新增，同一区域下的节点可在不同分组中共用)，

立即配置：[新建分组](/SharkCdnDoc/CDN管理/分组解析/新建分组.md)

(1). 点击分组解析，进入分组，点击分组名称，进入启用节点界面

![image](https://user-images.githubusercontent.com/90588289/135223752-a601ca5a-7c68-405a-8dc2-550a5196e880.png)

(2). 如下图操作选择启用节点，添加到右边的为启用的ip

![image](https://user-images.githubusercontent.com/90588289/135224008-c0594306-90fc-4d06-a5ed-ecc792322590.png)

### 第四步：新增产品

如下图点击新增产品，根据自已需求设置产品

端口类型中混合端口，可同时支持四层端口和七层端口

注：七层主分组和副分组如果有多个是可以多选的，在新增站点时会随机指定一个主分组和副分组

![image](https://user-images.githubusercontent.com/90588289/135224447-0567b920-3fd5-4736-a3b1-10a0916d2431.png)

立即配置：[添加产品](/SharkCdnDoc/CDN管理/产品列表/添加产品.md)

### 第五步：新增站点

如下图点击站点列表--添加站点--输入站点名称、密码（选填），增加站点

![image](https://user-images.githubusercontent.com/90588289/135225221-6ad9d4dc-af1f-4409-9b4b-1154a607778a.png)

### 第六步：登陆站点

点击站点列表，点击站点名登录

![image](https://user-images.githubusercontent.com/90588289/135225444-3d5af350-c946-4cc5-8fb4-e0954cca1ac0.png)

### 第七步：添加域名

记录管理--添加域名，域名是要做cdn的域名，IP是源服务器IP, CNAME系统会自动生成

![image](https://user-images.githubusercontent.com/90588289/135228544-486d8490-351e-4b14-a1fc-583b30690e49.png)

到这里就配置完成了
