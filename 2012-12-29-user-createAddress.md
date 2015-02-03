---
category: Stuff
path: '/app/customeraddress/create'
title: '[Z5]增加我的地址'
type: 'POST'

layout: nil
---

增加我的地址．
地址名称＼姓名＼手机＼省ID＼市ID＼区ID＼小区ID＼详细

### Request


```{
    'sessionid': '10760362195',
    'data': {
	'caption': '办公室',	//地址名称
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

For errors responses, see the [response status codes documentation](#response-status-codes).
