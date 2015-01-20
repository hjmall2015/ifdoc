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
	    'code':'I_6903148082140',
	    'name': 'A牌BB霜',
	    'price': '12.7',	//售价，注意是字符串
	    'coverimg': 'http://company.com/images/NBKSR000000065.jpg',
	    'amount': 1
	},
	{
	    'code':'I_6902088111927',
		'name': 'A牌BB霜',
	    'price': '12.7',	//售价，注意是字符串
	    'coverimg': 'http://company.com/images/NBKSR000000065.jpg',	    
	    'amount': 2
	},
	{
	    'code':'I_6903148091531',
		'name': 'A牌BB霜',
	    'price': '12.7',	//售价，注意是字符串
	    'coverimg': 'http://company.com/images/NBKSR000000065.jpg',	    
	    'amount': 1
	},
	...
	]
}```


