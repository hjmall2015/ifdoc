---
category: Stuff
path: '/app/classifiedswanted/getAll'
title: '[L2]获取所有需求'
type: 'POST'

layout: nil
---

获取所有需求,带分页,按发布时间由近至远排序.

### Request


```{
    'data':
	{
	'start': 0,			//分页信息
	'limit': 25,		//分页信息
  	}
}```

### Response

**如果成功**, 返回如下消息．

```{
    'success': true,
    'data':{
	items:[
	{
		'customerid': '13011112222';	//用户id
		'customernickname': 'zhangsan';	//用户昵称
		'customeravatar': 'http://cache.soso.com/wenwen/sg/i/logo.png';	//用户头像
		'title':'SD卡',		//标题
	    'userprice':'100',	//用户提供的价格
	    'approvedprice':'150',	//核定价格
	    'intro':'体积越小越好',	//简介
	    'comments':['要2个','最好金士顿的'],	//客服补充
	    'expiretime': '2015-10-15 23:10:12'	//截止时间
	},
	{
		'customerid': '13011112222';	//用户id
		'customernickname': 'zhangsan';	//用户昵称
		'customeravatar': 'http://cache.soso.com/wenwen/sg/i/logo.png';	//用户头像	
		'title':'移动电源',		//标题
	    'userprice':'200',	//用户提供的价格
	    'approvedprice':'210',	//核定价格
	    'intro':'容量大点的',	//简介
	    'comments':['要知名品牌的'],	//客服补充
	    'expiretime': '2015-10-17 16:25:03'	//截止时间
	},
	...
	]
    }
}```
