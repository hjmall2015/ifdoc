---
category: Stuff
path: '/app/geoarea/lv1Read'
title: '[G1]获得省列表'
type: 'POST'

layout: nil
---

获得省列表．

### Request


```
无```

### Response

**如果成功**,　返回如下消息．


```{
    'success': true,
    'data':
	[
	{
	    'areaid': 2,
	    'parentid': 1,
	    'name': '北京'
	},
	{
	    'areaid': 3,
	    'parentid': 1,
	    'name': '安徽'
	},
	{
	    'areaid': 4,
	    'parentid': 1,
	    'name': '福建'
	},
	...
	]
}```

For errors responses, see the [response status codes documentation](#response-status-codes).
