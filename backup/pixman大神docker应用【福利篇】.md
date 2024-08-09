****声明：**本文仅抄作业完成pixman搭建运行，相关程序及详细教程见：

原文教程：https://pixman.io/topics/17

**PS：**该程序运行需要docker环境，如没有可跳过本文或者安装docker后按教程运行。**

### _教程正文：_

一、运行环境搭建，整个搭建只有两步：

> _1、拉取镜像_
> 
> 安装运行命令：
> 
> docker pull pixman/pixman
> 
> _2、运行docker_
> 
> docker run -d --name=pixman -p 5000:5000 pixman/pixman
> 
> 如果需要在搭建主机重启的时候该docker可以自动启动建议增加运行参数restart=always：
> 
> docker run -d --name=pixman -p 5000:5000 --restart=always pixman/pixman
> 
> 可以修改 -p 5000:5000 中第一个 5000 为自定义端口号，如我修改为8201，则按以下代码运行：
> 
> docker run -d --name=pixman -p 8201:5000 --restart=always pixman/pixman

二、获取播放列表

原文有说明各个直播节目源的地址，可以直接http://ip:port/加文件即可，如我搭建的ip为192.168.100.1，设定端口为8201，则可以http://192.168.100.1:8201/ysp.m3u，http://192.168.100.1:8201/4gtv.m3u，http://192.168.100.1:8201/tptv.m3u，http://192.168.100.1:8201/itv.m3u，即可分别播放对应的节目


