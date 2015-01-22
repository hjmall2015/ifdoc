---
category: Stuff
path: '/app/commodity/checkStorage'
title: '[B8]检测库存'
type: 'POST'

layout: nil
---

检测库存．

### Request


```{
    'sessionid': '10760362195',
	'data':	{
	    'communityareaid': 3999,	//小区的areaid
	    'items': [
	    	{
		    'code':'I_6903148082140',
		    'amount': 2
		},
		{
		    'code':'I_6902088111927',
		    'amount': 4
		},
		{
		    'code':'I_6903148091531',
		    'amount': 1
		},
		...
		]//end items
	}//end data
}```

### Response

**如果成功**, 返回商品列表．


```{
    'success': true,
    'data': [{
	    'code':'I_6903148082140',
	    'result':'sufficient'	//库存足够
	},
	{
	    'code':'I_6902088111927',
	    'result':'insufficient',	//库存不够, 但有货
	    'stock': 3
	},
	{
	    'code':'I_6903148091531',
	    'result':'empty'	//无货
	},
	...
	]
}```


