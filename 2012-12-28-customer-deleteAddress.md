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
    'data': {
	'ids': [2,4,5]				
    }
}```

### Response

**如果成功**, 返回删除后的地址列表．


```{
    'success': true,
    'data':{
	items:[
	{
	    'id': 1,					//地址id,　用于修改丶删除等操作
	    'name': '张三',				//姓名
	    'mobile': '13611113333',			//手机
	    'postcode': '100190',			//邮编
	    'city': '北京',				//市
	    'district': '海淀区',			//区
	    'address': 'X街Y号',			//详细
	},
	{
	    'id': 3,					//地址id,　用于修改丶删除等操作
	    'mobile': '13611112222',			//手机
	    'postcode': '100230',			//邮编
	    'city': '天津',				//市
	    'district': '南开区',			//区
	    'address': 'P街Q号',			//详细
	},
	...
	]
    }
}```


