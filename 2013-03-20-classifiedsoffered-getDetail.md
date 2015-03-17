---
category: Stuff
path: '/app/classifiedswanted/getDetail'
title: '[L3]获取需求详情'
type: 'POST'

layout: nil
---

获取某需求详情.

### Request


```{
    'data':
	{
	'id': 5			//需求id
  	}
}```

### Response

**如果成功**, 返回如下消息．

```{
    'success': true,
    'data':{
    	'id': 5,	//需求id
		'title':'SD卡',		//最终标题
		'price':'100',		//价格
		'introtext': '体积越小越好',	//最终文本简介
		'contactnumber': '1300012135',	//联系电话
		'contactaddress': 'A区B楼',	//联系地址
	    'createtime':'2015-10-15 23:10:12', //发布时间
	    'starttime': '2015-10-15 23:10:12',	//开始时间
	    'endtime': '2015-10-15 23:10:12'	//结束时间
    }
}```
