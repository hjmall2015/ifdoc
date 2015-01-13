---
category: Stuff
path: '/app/order/getDetail'
title: '[O3]获取某订单详情'
type: 'POST'

layout: nil
---

获取某订单的详情．

### Request

```{
    'sessionid': '10760362195',
    'data': {
	'serial': 665	//订单编号
    }
}```

### Response

**如果成功**, 返回订单详情．
```{
'success': true,
    'data':{
	'serial':665	//订单编号
	'address': {
	    	'provinceareaid':5,	//省
	    	'cityareaid':27,	//市
	    	'districtareaid':391,	//区
	    	'communityareaid':1659,	//小区
	    	'contactname': '张三',	//联系人
	    	'contactnumber': '1300012135',	//联系电话
	    	'detail': 'ABCDEF'	//详细地址
	},	//end address
	'createtime': '2014-10-15 23:10:12',
	'finishtime': '2014-10-17 16:32:25',
	'status': '正在出货'
	'items':[
	{
	    'seriescover': "/hjmall/management/commodity/6901010119116.jpg",	//系列主图
	    'seriesname':'健力宝香草冰淇淋汽水（瓶）560ml',		//系列名称
	    'serial':'6901010119116',	//条码
	    'sellingprice':4.2,
	    'amount':3,
	},
	...
	],
	count:63		//订单中总项数
    }
}```



