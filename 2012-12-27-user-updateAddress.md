---
category: Stuff
path: '/app/customeraddress/update'
title: '[Z7]修改我的地址'
type: 'POST'

layout: nil
---

修改我的地址．

### Request


```{
    'sessionid': '10760362195',
    'data': {
	'id': 2,				//序号
	'addressname': '办公室',	//地址名称
	'provinceareaid':5,	//省
	'cityareaid':27,	//市
	'districtareaid':391,	//区
	'communityareaid':1659,	//小区
	'contactname': '张三',	//联系人
	'contactnumber': '1300012135',	//联系电话
	'detail': 'X街Y号'	//详细地址
    }
}```

### Response

**如果成功**,　返回如下消息．


```{
    'success': true
}```
