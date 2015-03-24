---
category: Stuff
path: '/app/classifiedsoffered/createOrder'
title: '[L9]创建供应订单'
type: 'POST'

layout: nil
---

创建供应订单．若成功，则返回订单编号，若失败，则返回失败响应，失败情况包括任意商品无库存丶其他失败．(错误码待定)

### Request

```{
    'sessionid': '10760362195',
    'data': {
    'communityareaid': 3999,
	'address': {
		'provinceareaid':5,	//省
		'cityareaid':27,	//市
		'districtareaid':391,	//区
		'communityareaid':1659,	//小区
		'contactname': '张三',	//联系人
		'contactnumber': '1300012135',	//联系电话
		'detail': 'X街Y号'	//详细地址
	},	//end address
	'items':
	[{
	'code':'I_6902088111927',	//商品编号
	'sellingprice': 13.7,			//售价
	'amount':2			//数量
	},
	{
	'code':'I_6903148091531',
	'sellingprice': 65.3,
	'amount':1
	}],
	'totalprice': 92.7	//总价 
    }
}```

### Response

**如果成功**, 返回成功提示.


```{
    'success': true,
    'data':{
		'serial': 665
	}
}```


