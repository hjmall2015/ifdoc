---
category: Stuff
path: '/app/commoditycategory/getAll'
title: '[B4]获得所有商品类别'
type: 'POST'

layout: nil
---

获得所有商品类别．

### Request


```无
```

### Response

**如果成功**, 返回商品类别信息, 类别共两级, 一级也可能无下级．

```Status: 200```
```{
    'success': true,
    'data':
	[
	{
	    'name': '百货',			//名称
	    'code': 'all.misc',		//编号	
	    'level': 1,				//级数
	    'parentcode': null,	//上级编号
	    'hassub': false			//是否有下级
	},
	{
	    'name': '日化',
	    'code': 'all.daily',
	    'level': 1,	    
	    'parentcode': null,
	    'hassub': false	    
	},
	{
	    'name': '食品',
	    'code': 'all.food',
	    'level': 1,	    
	    'parentcode': null,
	    'hassub': true	    
	},
	{
	    'name': '休闲食品',
	    'code': 'all.food.snack',
	    'level': 2,	    
	    'parentcode': 'all.food',
	    'hassub': false
	},
	{
	    'name': '冷冻食品',
	    'code': 'all.food.frozen',
	    'level': 2,	    
	    'parentcode': 'all.food',
	    'hassub': true	 	    
	},
	...
	]
}```
