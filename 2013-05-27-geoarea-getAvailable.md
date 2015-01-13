---
category: Stuff
path: '/app/geoarea/getAvailableCommunities'
title: '[G5]获得被覆盖的小区信息'
type: 'POST'

layout: nil
---

获得验证码．

### Request


```
无```

### Response

**如果成功**,　返回被覆盖的小区以及这些小区的省、市、区信息．


```{
    'success': true,
    'data':
	{
	province:	[
	{
	    'areaid': 25,
	    'parentid': 1,
	    'type': 1
	    'name': 'X省',,
	},
	{
	    'areaid': 31,
	    'parentid': 1,
	    'type': 1	    
	    'name': 'Y省'
	},
	{
	    'areaid': 39,
	    'parentid': 1,
	    'type': 1	    
	    'name': 'Z省'
	}
	],	//end province
	city:	[
	{
	    'areaid': 192,
	    'parentid': 25,
	    'type': 2,	    
	    'name': 'X1市'
	},
	{
	    'areaid': 203,
	    'parentid': 25,
	    'type': 2,
	    'name': 'X2市'
	},
	{
	    'areaid': 351,
	    'parentid': 31,
	    'type': 2,
	    'name': 'Y1市'
	} ...
	],	//end city
	district:	[
	{
	    'areaid': 1760,
	    'parentid': 192,
	    'type': 3,	    
	    'name': 'X1a区'	
	}, ...
	],	//end district
	community:	[
	{
	    'areaid': , 1760
	    'parentid': 3598,
	    'type': 4,	    
	    'name': 'X1a1小区'	
	}, ...
	]	//end community
	}	//end data
}```


