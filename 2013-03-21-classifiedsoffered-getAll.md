---
category: Stuff
path: '/app/classifiedsoffered/getAll'
title: '[L7]获取所有供应'
type: 'POST'

layout: nil
---

获取所有供应,带分页,按发布时间由近至远排序.

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
		"title": "蜂蜜",		//标题
        "thumbnail": "http://cache.soso.com/wenwen/sg/i/logo.png"	//缩略图
	},
	{
		 "title": "快餐",	//标题
        "thumbnail": "http://cache.soso.com/wenwen/sg/i/logo.png"	//缩略图
	},
	...
	]
    }
}```
