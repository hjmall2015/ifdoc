---
category: Stuff
path: '/app/commodity/getDetail'
title: '[B1]获得商品详情'
type: 'POST'

layout: nil
---

根据商品编号获得详情信息, 包含相关商品信息.


### Request

例1:
```{
    'data': {
		'code': 'I_6000000000002',	//商品编号
		'communityareaid': 6019		//小区的areaid
    }
}```

例2:
```{
    'data': {
		'code': 'S_0002',	//商品编号
		'communityareaid': 6019		//小区的areaid
    }
}```

### Response

**如果成功**, 返回商品信息．

例:
```{
    'success': true,
    'data': {
    	'hasgroup': true,			//是否有组, 如无则无组信息
    	'groupinfo': {				//组信息
    		'name':'IPhone6',			//组名称
		'price': '5000~6000',		//组价格,注意是字符串,如'5000-6000','5688'
		'optiondesc': '颜色',		//选项描述   
	    	'itemcount': 3				//组内商品数目，至少为1
    	},
	'items':［
	    		{
	    		'code': 'I_6918000000001',	//商品编号
	    		'name': 'IPhone6白',		//商品名称
			'vendor': '桔子',		//商品厂家
			'origin': '美国',		//商品产地
			'unit': '捆',			//商品单位	    		
	    		'groupoption': '白',			//组内选项名
	    		'groupdefault': true,		//是否为组内默认商品
	    		'discountprice': '229',		//售价,注意是字符串
	    		'sellingprice': '230',		//原价,注意是字符串
	    		'hasstock': true,		//小区是否有货	 
	    		'coverimg': 'http://company.com/images/NBKSR000000065.jpg',	//主图
	    		'detailimgs': ['http://company.com/detailimages/NBKSR000000065_1.jpg', 'http://company.com/detailimages/NBKSR000000065_2.jpg'],	//详情图
	    		'profile': [{'key': 'aaa', 'value': 'bbb'},{'key': 'ccc', 'value': 'ddd'}]	//简介
	    		},
	    		{
	    		'code': 'I_6918000000002',	//商品编号
	    		'name':'IPhone6土豪金',		//商品名称
			'vendor': '桔子',		//商品厂家
			'origin': '美国',		//商品产地
			'unit': '捆',			//商品单位	   	    		
	    		'groupoption': '土豪金'		//###组内选项名
			'groupdefault': false,		//###是否为组内默认商品    		
	    		'discountprice': '229',		//售价
	    		'sellingprice': '230',		//原价
	    		'hasstock': true,		//小区是否有货	    		
	    		'coverimg': 'http://company.com/images/NBKSR000000065.jpg',	//主图
	    		'detailimgs': ['http://company.com/detailimages/NBKSR000000065_1.jpg', 'http://company.com/detailimages/NBKSR000000065_2.jpg'],	//详情图
	    		'profile': [{'key': 'aaa', 'value': 'bbb'},{'key': 'ccc', 'value': 'ddd'}]	//简介
	    		},
			{
	    		'code': 'I_6918000000003',	//商品编号
	    		'name':'IPhone6黑',		//商品名称
			'vendor': '桔子',		//商品厂家
			'origin': '美国',		//商品产地
			'unit': '捆',			//商品单位	 	    		
	    		'groupoption': '黑'			//选项名
			'groupdefault': false,		//是否为组内默认商品	    		
	    		'discountprice': '229',		//售价
	    		'sellingprice': '230',		//原价	  
	    		'hasstock': true,		//小区是否有货	   		
	    		'default': false,	//是否为系列内默认商品
	    		'coverimg': 'http://company.com/images/NBKSR000000065.jpg',	//主图
	    		'detailimgs': ['http://company.com/detailimages/NBKSR000000065_1.jpg', 'http://company.com/detailimages/NBKSR000000065_2.jpg']	//详情图 
	    		'profile': [{'key': 'aaa', 'value': 'bbb'},{'key': 'ccc', 'value': 'ddd'}]	//简介		    	
	    		}	    		
	    	]			//end items
    }	//end data
}```