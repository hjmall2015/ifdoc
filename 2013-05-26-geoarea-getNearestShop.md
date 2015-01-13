---
category: Stuff
path: '/app/geoarea/getNearestShop'
title: '[G6]获得最近的商店'
type: 'POST'

layout: nil
---

获得最近的一个商店．返回经纬度和配货范围取在范围内的最近的一个商店.

### Request

```{
    'data': {
	'latitude': 39.2		//维度
	'longitude': 47.1		//经度
    }
}```


### Response

**如果成功**,　返回商店信息．


```{
    'success': true,
    'data':
	{
	    'code': 'SHOP_TTY',
	    'name': '天通苑',
	    'communityareaid': 503,	//小区id
	    'districtareaid': 29			//区id(如海淀区)
	},
}```


