---
category: Stuff
path: '/app/cartitem/sync'
title: '[C1]购物车同步'
type: 'POST'

layout: nil
---

同步购物车．同步规则为：只增加商品、更新商品数目，不删除商品．

### Request


```{
    'sessionid': '10760362195',
    'data':
	[{
	    'code':'I_6902088111927',
	    'amount': 2
	},
	{
	    'code':'I_6903148091531',
	    'amount': 1
	},
	...
	]
}```

### Response

**如果成功**, 返回同步后的购物车．

```Status: 200```
```{
    'success': true,
    'data':
	[{
	    'code':'I_6903148082140',
	    'amount': 1
	},
	{
	    'code':'I_6902088111927',
	    'amount': 2
	},
	{
	    'code':'I_6903148091531',
	    'amount': 1
	},
	...
	]
}```

失败响应见 [响应格式及错误码](#/response-status-codes)中的631号错误.
