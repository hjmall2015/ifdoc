---
category: Stuff
path: '/app/geoarea/lv2Read'
title: '[G2]获得市列表'
type: 'POST'

layout: nil
---

获得市列表．

### Request


```{
    'data': {
	'parentid': '2'
    }
}```

### Response

**如果成功**,　返回如下消息．


```{
    'success': true,
    'data':
	[
	{
	    'areaid': 53,
	    'parentid': 4,
	    'name': '福州'
	},
	{
	    'areaid': 54,
	    'parentid': 4,
	    'name': '龙岩'
	},
	{
	    'areaid': 55,
	    'parentid': 4,
	    'name': '南平'
	},
	...
	]
}```

For errors responses, see the [response status codes documentation](#response-status-codes).
