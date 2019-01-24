# Orange Pi Zero Plus OpenWRT 刷入说明

准备工作：

 ·Orange Pi Zero Plus
 
 ·TF卡
 
 ·读卡器
 
 ·PC
 
所需软件：
 
 ·Win32DiskImager
 
 ·浏览器
 
 ·SSH客户端
 
 具体步骤：
 
 1.下载固件并解压。
 
 2.将TF卡插入读卡器并连接至PC端；
 
 3.开启 Win32DiskImager ,选择解压出来的文件，点击写入，即完成固件烧录步骤；
 
 4.将TF卡插入 Pi 的卡槽中，并使用网线连接至PC；
 
 5.打开SSH客户端，默认连接IP `root@192.168.1.1 -p 22 ` ，初始密码默认为 `password` ；
 
 6.进入SSH后，粘贴命令行 `echo 0xDEADBEEF > /etc/config/google_fu_mode ` （ 此步骤为开启 shadowsocks 插件 ）；
 
 7.打开浏览器，进入默认网关地址 http://192.168.1.1 进行各项设置；
 
 8.太监了。
