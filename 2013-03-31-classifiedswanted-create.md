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
	    'intro':'体积越小越好',	//简介
	    'expiretime': '2015-10-15 23:10:12'	//截止时间
  	}
}```

### Response

**如果成功**, 返回如下消息．

```Status: 200```
```{
    'success': true
}```
