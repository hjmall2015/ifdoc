---
category: Stuff
path: '/app/commodity/getDetail'
title: '[B1临时]获得商品详情'
type: 'POST'

layout: nil
---

根据商品编号获得详情信息, 包含相关商品信息. 注: 可根据code属性判断相关商品中哪个为当前商品.


### Request

例1:
```{
    'data': {
		'code': 'I_6000000000002',	//商品编号
    }
}```

例2:
```{
    'data': {
		'code': 'S_0002',	//商品编号
    }
}```

### Response

**如果成功**, 返回商品信息．

例:
```{
    'success': true,
    'data': {
	    'seriesname':'IPhone6',		//系列名称
		'pricerange': '5000~6000',		//系列价格区间,注意是字符串
	    'name':'IPhone6白',		//系列名称
	    'vendor': '桔子',			//系列厂家
	    'unit': '捆',				//系列单位
	    'coverimg': 'http://company.com/images/NBKSR000000065.jpg',	//系列主图
	    'hasoptions': true,			//是否有选项  
	    'optionname': '颜色',		//系列选项名称   
	    'itemcount': 3,				//系列内商品数目，至少为1
	    'items':［
	    		{
	    		'code': 'I_6918000000001',	//商品编号
	    		'name': 'IPhone6白',		//商品名称
	    		'option': '白',		//选项名
	    		'default': true,	//是否为系列内默认商品
	    		'discountprice': '229',		//售价,注意是字符串
	    		'sellingprice': '230',		//原价,注意是字符串
	    		'coverimg': 'http://company.com/images/NBKSR000000065.jpg',	//主图
	    		'detailimgs': ['http://company.com/detailimages/NBKSR000000065_1.jpg', 'http://company.com/detailimages/NBKSR000000065_2.jpg'],	//详情图
	    		'profile': [{'key': 'aaa', 'value': 'bbb'},{'key': 'ccc', 'value': 'ddd'}]	//简介
	    		},
	    		{
	    		'code': 'I_6918000000002',	//商品编号
	    		'name':'IPhone6土豪金',		//商品名称
	    		'option': '土豪金'		//选项名
				'default': false,	//是否为系列内默认商品	    		
	    		'discountprice': '229',		//售价
	    		'sellingprice': '230',		//原价	    		
	    		'coverimg': 'http://company.com/images/NBKSR000000065.jpg',	//主图
	    		'detailimgs': ['http://company.com/detailimages/NBKSR000000065_1.jpg', 'http://company.com/detailimages/NBKSR000000065_2.jpg'],	//详情图
	    		'profile': [{'key': 'aaa', 'value': 'bbb'},{'key': 'ccc', 'value': 'ddd'}]	//简介
	    		},
			{
	    		'code': 'I_6918000000003',	//商品编号
	    		'name':'IPhone6黑',		//商品名称
	    		'option': '黑'				//选项名	
	    		'discountprice': '229',		//售价
	    		'sellingprice': '230',		//原价	    		
	    		'default': false,	//是否为系列内默认商品
	    		'coverimg': 'http://company.com/images/NBKSR000000065.jpg',	//主图
	    		'detailimgs': ['http://company.com/detailimages/NBKSR000000065_1.jpg', 'http://company.com/detailimages/NBKSR000000065_2.jpg']	//详情图 
	    		'profile': [{'key': 'aaa', 'value': 'bbb'},{'key': 'ccc', 'value': 'ddd'}]	//简介		    	
	    		}	    		
	    	]			//end items
    }	//end data
}```

有范围，那售价在哪？有系列时价格售价双显示？