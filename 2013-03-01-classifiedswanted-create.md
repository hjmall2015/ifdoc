---
category: Stuff
path: '/app/classifiedswanted/create'
title: '[L1]发布需求'
type: 'POST'

layout: nil
---

发布需求.

### Request


```{
    'sessionid': '10760362195',
    'data':
	{
	    'title':'SD卡',		//标题
	    'userprice':'100',	//用户提供的价格
	    'approvedprice':'150',	//核定价格
	    'intro':'体积越小越好',	//简介
	    'comments':['要2个','最好金士顿的'],	//客服补充
	    'expiretime': '2015-10-15 23:10:12'	//截止时间
  	}
}```

### Response

**如果成功**, 返回添加后的购物车．

```Status: 200```
```{
    'success': true,
    'data':
	[{
	    'code':'I_6903148082140',
	    'amount': 1
	},
	{
	    'code':'I_6902088111927',
	    'amount': 3
	},
	{
	    'code':'I_6903148091531',
	    'amount': 1
	},
	...
	]
}```

失败响应见 [响应格式及错误码](#/response-status-codes)中的631号错误.
