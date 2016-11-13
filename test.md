# TM 管理系统服务api文档

## 注意
	B端：表示前端（浏览器端）
	S端：表示后端（服务器端）
	
	本系统服务URL采用rest"风格"
	
	所有服务地址为 url=api/index.php
	
	浏览器通过post方式提交（json格式（method字段关键））
	
###1.用户验证
	B端：
	`````
	{
		method:"userVerify",
		data:[
			{
				username:"zhouchangsheng"
				password:"zhouchangsheng"
			}
		]
	}
	`````
	
	S端：
	S1成功：
	`````
	{
		data:[],
		errcode:"0",
		errmsg:"ok"
	}
	`````
	
	S2失败：
	`````
	{
		data:[],
		errocde:"...",
		errmsg:"..."
	}
	`````
