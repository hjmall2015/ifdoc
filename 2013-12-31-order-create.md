---
category: Stuff
path: '/app/order/create'
title: '[O1]创建订单'
type: 'POST'

layout: nil
---

创建订单．注意：请求中无价格信息(此处待确认)．若成功，则返回订单编号，若失败，则返回失败响应，失败情况包括任意商品无库存丶其他失败．(错误码待定)

### Request

```{
    'sessionid': '10760362195',
    'data': {
	'communityareaid': 6019,
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
	'serial':'6902088111927',
	'amount':2
	},
	{
	'serial':'6903148091531',
	'amount':1
	}]
    }
}```

### Response

**如果成功**, 返回订单编号


```{
    'success': true,
    'data': {'serial': 15}	//注意是数字
}```


