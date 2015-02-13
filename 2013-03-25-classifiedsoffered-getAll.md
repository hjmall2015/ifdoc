---
category: Stuff
path: '/app/classifiedsoffered/getAll'
title: '[L7]获取所有需求'
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
        "coverimg": "http://cache.soso.com/wenwen/sg/i/logo.png",	//主图
        "price": "1.23",	//价格
        "condition": "五环内",	//限制
        "intro": "质量可靠",	//简介
        "detailimgs":	//详情图 
        [
         "http://cache.soso.com/wenwen/sg/i/logo.png",
         "http://cache.soso.com/wenwen/sg/i/logo.png"
	     ]
	},
	{
		 "title": "快餐",	//标题
        "coverimg": "http://cache.soso.com/wenwen/sg/i/logo.png",	//主图
        "price": "4.56",	//价格
        "condition": "仅工作日送餐",	//限制
        "intro": "中式",	//简介
        "detailimgs":	//详情图 
        [
          "http://cache.soso.com/wenwen/sg/i/logo.png",
          "http://cache.soso.com/wenwen/sg/i/logo.png"
        ]
	},
	...
	]
    }
}```
