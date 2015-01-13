---
category: Stuff
path: '/app/geoarea/lv3Read'
title: '[G3]获得区列表'
type: 'POST'

layout: nil
---

获得区列表．

### Request


```{
    'data': {
	'parentid': '52'
    }
}```


### Response

**如果成功**,　返回如下消息．


```{
    'success': true,
    'data':
	[
	{
	    'areaid': 518,
	    'parentid': 53,
	    'name': '鼓楼区'
	},
	{
	    'areaid': 519,
	    'parentid': 53,
	    'name': '台江区'
	},
	...
	]
}```

For errors responses, see the [response status codes documentation](#response-status-codes).
