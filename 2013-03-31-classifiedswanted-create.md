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
	'initialtitle': 'SD卡',		//原始标题
	'initialintrotext': '体积越小越好',	//原始文本简介
	'initialintrovoiceid': '60532907',	//原始语音简介ID
	'contactnumber': '1300012135',	//联系电话
	'createtime':'2015-10-15 23:10:12' //发布时间
  	}
}```

### Response

**如果成功**, 返回如下消息．

```Status: 200```
```{
    'success': true
}```
