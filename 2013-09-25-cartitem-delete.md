---
category: Stuff
path: '/app/cartitem/delete'
title: '[C4]购物车删除商品'
type: 'POST'

layout: nil
---

删除购物车中的一种商品．

### Request


```{
    'sessionid': '10760362195',
    'data':
	{
	    'serial':'6902088111927'
	}
}```

### Response

**如果成功**, 返回删除后的购物车．

```Status: 200```
```{
    'success': true,
    'data':
	[{
	    'serial':'6903148082140',
	    'amount': 1
	},
	{
	    'serial':'6903148091531',
	    'amount': 1
	},
	...
	]
}```

失败响应见 [响应格式及错误码](#/response-status-codes)中的634号错误.
