---
category: Stuff
path: '/app/classifiedswanted/createText'
title: '[L1]发布文本需求'
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
	'contactnumber': '1300012135'	//联系电话
  	}
}```

### Response

**如果成功**, 返回如下消息．

```Status: 200```
```{
    'success': true
}```
