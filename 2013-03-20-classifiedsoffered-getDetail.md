---
category: Stuff
path: '/app/classifiedsoffered/getDetail'
title: '[L8]获取供应详情'
type: 'POST'

layout: nil
---

获取某需求详情.

### Request


```{
    'data':
	{
	'code': 'I_6000000000002'			//供应id
  	}
}```

### Response

**如果成功**, 返回如下消息．

```{
    'success': true,
    'data':{
		"title": "蜂蜜",		//标题
		'code': 'I_6000000000002',	//供应编号
		'discountprice': '229',		//售价
        "thumbnail": "http://cache.soso.com/wenwen/sg/i/logo.png",	//缩略图
        'coverimg': 'http://company.com/images/NBKSR000000065.jpg',	//主图
        'detailimgs': ['http://company.com/detailimages/NBKSR000000065_1.jpg', 'http://company.com/detailimages/NBKSR000000065_2.jpg']	//详情图
    }
}```