---
author : "ArnoLiu"
title : "FirstExpansionHub"
date : "2020-01-16"
description : ""
---

目的：扩展单hub IO口的局限性。

注意：一个机器人最多只能有两个hub。

设备需求：
<blockquote>
两台手机	
	
micro数据线	
	
OTG	
	
REV Robotics Switch, Cable, and Bracket (REV-31-1387). 	
	
REV Robotics Tamiya to XT30 Adapter Cable (REV-31-1382). 	
	
12V电源	
	
两个HUB	
	
 3-Pin JST PH Cable 	
	
REV Robotics XT30 Extension Cable	
</blockquote>

	具体步骤：
		1. 检查hub Address
		原因：所有hub出厂都会有默认地址2，必须改变一个的地址来避免冲突
		2. 改变hub Address（注意此时不要连接两个hub）
		步骤：RC Advanced setting -》删除原配置文件-》创建新临时配置文件并保存
		成功标志：HUB LED闪烁为：GREEN (long) --> BLUE (short) --> BLUE (short) 
		3. 连接2个hub
			a. 断电
			b. 用XT30扩展电源线并电
c. <img src="https://github.com/arnoliudaxia/arnoliudaxia.github.io/blob/blog/content/img/exc1.png?raw=true"/>

	d. 用3针线连接2个hub上的RS-485接口
	f. 上电连接RC，创建新配置文件




	
