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
	'items':[{
			'code':'I_6902088111927',	//商品编号
			'sellingprice': 13.7,			//售价
			'coverimg': "/hjmall/management/commodity/6902088111921.jpg",	//主图
			'amount':2			//数量
			},
			{
			'code':'I_6903148091531',
			'sellingprice': 65.3,
			'coverimg': "/hjmall/management/commodity/6902088111921.jpg",	//主图
			'amount':1
		}],
	'createtime': '2014-10-15 23:10:12',
	'status': {'name': '正在出货', 'time': '2014-10-15 23:10:12'}		
    }
}```



