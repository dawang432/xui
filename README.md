# V2ray--X-ui--教程合集
关于v2ray搭建和x-ui面板搭建两种教程

💻网上的教程很多  教程只是我个人总结

希望可以帮助到你🌏

🔈本教程只提供最简单的搭建方法  难点的可以看看我其他教程

教程脚本来源于：
-------------------
V2ray：https://github.com/233boy/v2ray/wiki/V2Ray

X-ui：https://github.com/vaxilu/x-ui

BBR加速：https://www.v2rayssr.com/bbr.html

需要用到的工具
-----------------------
一台VPS（主流系统最好Ubuntu  CentOS）

推荐vmshell家的香港VPS速度起飞解锁奈菲：https://vmshell.com/aff.php?aff=331

SSH连接工具（连接vps的   例如Termius    Finalshell等）

搭建V2ray教程
----------------------
首先连接好VPS看到开头root就行了没有的话输入：
`sudo -i`

**连接好后第 1 步**：
`bash <(curl -s -L https://git.io/v2ray.sh)`

![image](https://user-images.githubusercontent.com/94978556/145370208-7ebe3155-eb30-46fd-9802-828953077890.png)

**如果没有出现这个页面可能是你没有安装curl**

ubuntu/debian安装方法：
`apt-get update -y && apt-get install curl -y`

centos安装方法：
`yum update -y && yum install curl -y`

**然后再执行一次第 1 步**

**选择 1 安装然后基本上就可以一路回车键啦  等待安装完成就好了**

![image](https://user-images.githubusercontent.com/94978556/145371470-061cd5f6-2e7a-4577-95e7-41de54183375.png)

**搭建好后输入：
`v2ray qr`获取二维码链接  然后复制链接**

![image](https://user-images.githubusercontent.com/94978556/145372559-a315496f-b765-4fb9-ae63-76f08e8c85a3.png)

**然后用v2ray客户端扫码导入就好了**

![image](https://user-images.githubusercontent.com/94978556/145372904-d38dc4d7-c112-47a0-830f-2a2c85422d17.png)

**导入后节点名字可以自定义一个自己喜欢的❤**

**以后如果想调出v2ray面板直接连接ssh输入： `v2ray`

**至此整个V2ray搭建就完成了**

搭建X-ui面板教程
-------------------------------------
**连接ssh**

![image](https://user-images.githubusercontent.com/94978556/145374448-33efbce4-4a01-4441-82b4-f795853bd345.png)

**第 1 步直接输入**：
`bash <(curl -Ls https://raw.githubusercontent.com/vaxilu/x-ui/master/install.sh)`

![image](https://user-images.githubusercontent.com/94978556/145375231-25379ff2-e8ac-46cb-b822-9a326bcea744.png)

**搭建好后用你VPS `IP地址`加`:` 默认端口`54321`游览器访问**

**使用默认登陆账号密码登陆`admin`**

![image](https://user-images.githubusercontent.com/94978556/145376064-44cedb27-920b-4e94-948b-489ddf07fbee.png)

**登录后点击面板设置修改你默认面板监听端口&面板url根路径和登录账号**

![image](https://user-images.githubusercontent.com/94978556/145377323-9dc8e08c-349b-46c4-b5cd-ac9627474b3b.png)

![image](https://user-images.githubusercontent.com/94978556/145377241-d36a839b-a496-421c-9f4f-29979369c6c2.png)

**然后重启一下面板用你VPS `IP地址`加`:` 你修改的端口加/根路径游览器访问**

**然后点击面板入站列表添加节点  选择`+`**

![image](https://user-images.githubusercontent.com/94978556/145378123-d11c6d17-8081-49ac-9cc0-0d4076b41116.png)
---------------------------------------------------
备注就是你的节点名字

协议就选择vmess

监听IP不用填

端口你也可以自己设个 也可以默认无所谓

总流量可以自己规定多少（合租适合）无所谓的话可以不填

到期时间可以不填  合租可以试试

然后添加就好了

![image](https://user-images.githubusercontent.com/94978556/145378385-899d7964-2074-4c52-8051-83401f4ff51f.png)

**使用方法点击操作  选择二维码  然后v2ray客户端扫码就好了**

![image](https://user-images.githubusercontent.com/94978556/145379827-5e2ee9f0-c785-482a-8b1f-394fd977f2ba.png)

**X-ui面板的好处就是可以添加多个节点管理流量**

**至此整个X-ui就搭建好了**

BBR加速安装
---------------------------------
**输入**：`wget -N --no-check-certificate "https://raw.githubusercontent.com/chiakge/Linux-NetSpeed/master/tcp.sh" && chmod +x tcp.sh && ./tcp.sh`

![image](https://user-images.githubusercontent.com/94978556/145380739-3fbc2210-a1fa-4a8a-8096-e740152855cd.png)

**选择你需要的内核然后等待安装好后使用你安装的内核就好了**

**推荐安装**

**内核管理 1 安装 BBR/BBR魔改版内核**

**加速管理 4 使用BBR加速**

**加速就ok啦，快去看看你的网速有没有提升吧**

至此两种教程结束
----------------------------
##BBR2加速##

wget --no-check-certificate -q -O bbr2.sh "https://github.com/yeyingorg/bbr2.sh/raw/master/bbr2.sh" && chmod +x bbr2.sh && bash bbr2.sh auto
