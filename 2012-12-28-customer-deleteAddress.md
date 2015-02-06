---
category: Stuff
path: '/app/customeraddress/delete'
title: '[Z6]删除我的地址'
type: 'POST'

layout: nil
---

删除我的地址．

### Request


```{
    'sessionid': '10760362195',
    'data': [2,4,5]				
}```

### Response

**如果成功**, 返回删除后的地址列表．


```{
    'success': true,
    'data':{
	items:[
	{
	'id': 1,					//地址id,　用于修改丶删除等操作
	'caption': '办公室',	//地址名称
	'provinceareaid':5,	//省
	'cityareaid':27,	//市
	'districtareaid':391,	//区
	'communityareaid':1659,	//小区
	'provincename':'北京',	//省名
	'cityname':'北京',	//市名
	'districtname':'海淀',	//区名
	'communityname': '五道口',	//小区名
	'contactname': '张三',	//联系人
	'contactnumber': '1300012135',	//联系电话
	'detail': 'X街Y号'	//详细地址
	},
	{
	 'id': 3,					//地址id,　用于修改丶删除等操作
	'addressname': '家里',	//地址名称
	'provinceareaid':5,	//省
	'cityareaid':27,	//市
	'districtareaid':391,	//区
	'communityareaid':1659,	//小区
	'provincename':'北京',	//省名
	'cityname':'北京',	//市名
	'districtname':'海淀',	//区名
	'communityname': '五道口',	//小区名
	'contactname': '李四',	//联系人
	'contactnumber': '1311122233',	//联系电话
	'detail': 'S街T号'	//详细地址
	},
	...
	]
    }
}```


