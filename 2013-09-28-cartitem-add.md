---
category: Stuff
path: '/app/cartitem/add'
title: '[C3]购物车添加商品'
type: 'POST'

layout: nil
---

添加商品．如果已有同种商品则增加数量.

### Request


```{
    'sessionid': '10760362195',
    'data':
	[{
	    'serial':'6902088111927',
	    'amount': 2
	},
	{
	    'serial':'6903148091531',
	    'amount': 1
	},
	...
	]
}```

### Response

**如果成功**, 返回添加后的购物车．

```Status: 200```
```{
    'success': true,
    'data':
	[{
	    'serial':'6903148082140',
	    'amount': 1
	},
	{
	    'serial':'6902088111927',
	    'amount': 3
	},
	{
	    'serial':'6903148091531',
	    'amount': 1
	},
	...
	]
}```

失败响应见 [响应格式及错误码](#/response-status-codes)中的631号错误.
