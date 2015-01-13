---
category: Stuff
path: '/app/geoarea/lv4Read'
title: '[G4]获得区域列表'
type: 'POST'

layout: nil
---

获得验证码．

### Request


```{
    'data': {
	'parentid': '501'
    }
}```
### Response

**如果成功**,　返回如下消息．


```{
    'success': true,
    'data':
	[
	{
	    'areaid': 3410,
	    'parentid': 541,
	    'name': '建瓯市小区1'
	},
	...
	]
}```


