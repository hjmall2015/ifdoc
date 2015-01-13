---
category: Stuff
path: '/app/cartitem/getAll'
title: '[C2]购物车获取'
type: 'POST'

layout: nil
---

获取购物车中的所有商品．

### Request


```{
    'sessionid': '10760362195'
}```

### Response

**如果成功**, 返回购物车中的商品．

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
	    'amount': 2
	},
	{
	    'serial':'6903148091531',
	    'amount': 1
	},
	...
	]
}```


