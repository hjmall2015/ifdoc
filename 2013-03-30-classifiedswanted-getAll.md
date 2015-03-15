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
	'limit': 25			//分页信息
  	}
}```

### Response

**如果成功**, 返回如下消息．

```{
    'success': true,
    'data':{
	items:[
	{
		'title':'SD卡',		//最终标题
	    'createtime':'2015-10-15 23:10:12', //发布时间
	    'endtime': '2015-10-15 23:10:12'	//结束时间
	},
	...
	]
    }
}```
