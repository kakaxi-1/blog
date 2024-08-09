**声明：项目来源youshandefeiyang，鸣谢大佬**

**PS：该程序运行同样需要docker环境，如没有可跳过本文或者安装docker后按教程运行，同样仅需要两步就能成功搭建，动手能力强的小伙伴网上自行搜索docker安装试玩。**

**_教程正文：_**
一、运行环境搭建：

> 1、
> docker run -d --restart unless-stopped --privileged=true -p 35455:35455 --name allinone youshandefeiyang/allinone
> 
> 2、
> docker run -d --name watchtower --restart unless-stopped -v /var/run/docker.sock:/var/run/docker.sock containrrr/watchtower allinone -c --schedule "0 0 2 * * *"

二、获取播放列表

> IPTV直播：http://你的IP:35455/tv.m3u
> 
> 虎牙一起看：http://你的IP:35455/huyayqk.m3u?url=http://你的IP:35455
> 
> 斗鱼一起看：http://你的IP:35455/douyuyqk.m3u?url=http://你的IP:35455
> 
> YY轮播：http://你的IP:35455/yylunbo.m3u?url=http://你的IP:35455
> 
> BiliBili生活：http://你的IP:35455/bililive.m3u?url=http://你的IP:35455

