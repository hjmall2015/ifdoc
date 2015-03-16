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
		'id':5,
		'title':'SD卡',		//最终标题
		'price':'100',		//价格
		'introtext': '体积越小越好',	//最终文本简介
		'contactnumber': '1300012135',	//联系电话
		'contactaddress': 'A区B楼',	//联系地址
	    'starttime':'2015-10-15 23:10:12', //开始时间(到秒)
	    'endtime': '2015-10-15 23:10:12'	//结束时间(到秒)
	},
	...
	]
    }
}```
