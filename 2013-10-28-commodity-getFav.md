---
category: Stuff
path: '/app/commodity/getFav'
title: '[B7]获得我收藏的商品列表'
type: 'POST'

layout: nil
---

获得我收藏的商品列表，无库存信息，按收藏时间由近到远排序，带分页．

### Request


```{
    'sessionid': '10760362195',
    'data': {
	'start': 0,			//分页信息
	'limit': 25			//分页信息
    }
}```

### Response

**如果成功**, 返回商品列表．


```{
    'success': true,
    'data':{
	items:[
	{
	    'name':'多芬滋养水润洗发乳200ml',
	    'serial': '6902088111927',
	    'category': 2,
	    'unit': '瓶',
	    'sellingprice': 19.5,
	    'vendor': '联合利华',
	    'sales': 59			//销量
	},
	{
	    'name':'潘婷丝质顺滑精华素400ml',
	    'serial': '6903148091531',
	    'category': 2,
	    'unit': '瓶',
	    'sellingprice': 27.5,
	    'vendor': '宝洁',
	    'sales': 307,		//销量
	},
	...
	],
	count:15			//总数
    }
}```


