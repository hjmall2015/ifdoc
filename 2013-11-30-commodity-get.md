---
category: Stuff
path: '/app/commodity/getDetail'
title: '[B1]获得商品详情'
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

例1:
```{
    'success': true,
    'data': {
	    'code': 'I_6000000000002',	//商品编号
	    'name':'IPhone6土豪金',			//商品名称
	    'related':{	//相关商品信息,如果无相关商品，则hasitems属性为false, items里无商品
	    	hasitems: 'true',
	    	items: [
	    		{
	    		'code': 'I_6918000000001',	//商品编号
	    		'name': 'IPhone6白',		//商品名称
	    		'nameingroup': '白',		//选项名
	    		'discountprice': '229',		//售价
	    		'sellingprice': '230',			//原价
	    		'coverimg': 'http://company.com/images/NBKSR000000065.jpg',	//主图
	    		'detailimgs': ['http://company.com/detailimages/NBKSR000000065_1.jpg', 'http://company.com/detailimages/NBKSR000000065_2.jpg'],	//详情图
	    		'extradesc': [{'key': 'aaa', 'value': 'bbb'},{'key': 'ccc', 'value': 'ddd'}]	//额外描述
	    		},
	    		{
	    		'code': 'I_6918000000002',	//商品编号
	    		'name':'IPhone6土豪金',		//商品名称
	    		'nameingroup': '土豪金'		//选项名
	    		'discountprice': '229',		//售价
	    		'sellingprice': '230',		//原价	    		
	    		'coverimg': 'http://company.com/images/NBKSR000000065.jpg',	//主图
	    		'detailimgs': ['http://company.com/detailimages/NBKSR000000065_1.jpg', 'http://company.com/detailimages/NBKSR000000065_2.jpg'],	//详情图
	    		'extradesc': [{'key': 'aaa', 'value': 'bbb'},{'key': 'ccc', 'value': 'ddd'}]
	    		},
				{
	    		'code': 'I_6918000000003',	//商品编号
	    		'name':'IPhone6黑',		//商品名称
	    		'discountprice': '229',		//售价
	    		'sellingprice': '230',		//原价	    		
	    		'nameingroup': '黑'		//选项名	  
	    		'coverimg': 'http://company.com/images/NBKSR000000065.jpg',	//主图
	    		'detailimgs': ['http://company.com/detailimages/NBKSR000000065_1.jpg', 'http://company.com/detailimages/NBKSR000000065_2.jpg']	//详情图 
	    		'extradesc': [{'key': 'aaa', 'value': 'bbb'},{'key': 'ccc', 'value': 'ddd'}] 		    	
	    		}	    		
	    	],			//end groupinfo
	    'discountprice': '5000',		//售价
	    'sellingprice': '5001',			//原价
	    'vendor': '桔子',			//厂家
	    'unit': '捆',				//规格
	    'coverimg': 'http://company.com/images/NBKSR000000065.jpg',	//主图
	    'detailimgs': ['http://company.com/detailimages/NBKSR000000065_1.jpg', 'http://company.com/detailimages/NBKSR000000065_2.jpg'],	//详情图
    }
}```

例2:
```{
    'success': true,
    'data': {
	    'code': 'I_6000000001296',	//商品编号
	    'name':'ABC牌针织衫L号',			//商品名称
	    'related':{	//相关商品信息,如果无相关商品，则hasitems属性为false, items里无商品
	    	hasitems: 'true',
	    	items: [
	    		{
	    		'code': 'I_6000000001296',	//商品编号
	    		'name': 'ABC牌针织衫XL号',		//商品名称
	    		'nameingroup': 'XL'		//选项名
	    		'discountprice': '229',		//售价
	    		'sellingprice': '230',			//原价	    		
	    		'coverimg': 'http://company.com/images/NBKSR000000065.jpg',	//主图
	    		'detailimgs': ['http://company.com/detailimages/NBKSR000000065_1.jpg', 'http://company.com/detailimages/NBKSR000000065_2.jpg'],	//详情图
	    		'extradesc': [{'key': 'aaa', 'value': 'bbb'},{'key': 'ccc', 'value': 'ddd'}]	//额外描述
	    		},
	    		{
	    		'code': 'I_6000000001297',	//商品编号
	    		'name':'ABC牌针织衫L号',		//商品名称
	    		'nameingroup': 'L'		//选项名
	    		'discountprice': '229',		//售价
	    		'sellingprice': '230',			//原价	    		
	    		'coverimg': 'http://company.com/images/NBKSR000000065.jpg',	//主图
	    		'detailimgs': ['http://company.com/detailimages/NBKSR000000065_1.jpg', 'http://company.com/detailimages/NBKSR000000065_2.jpg'],	//详情图
	    		'extradesc': [{'key': 'aaa', 'value': 'bbb'},{'key': 'ccc', 'value': 'ddd'}]	//额外描述
	    		},
				{
	    		'code': 'I_6000000001298',	//商品编号
	    		'name':'ABC牌针织衫M号',		//商品名称
	    		'nameingroup': 'M'		//选项名	   
	    		'discountprice': '229',		//售价
	    		'sellingprice': '230',			//原价	    		
	    		'coverimg': 'http://company.com/images/NBKSR000000065.jpg',	//主图
	    		'detailimgs': ['http://company.com/detailimages/NBKSR000000065_1.jpg', 'http://company.com/detailimages/NBKSR000000065_2.jpg'],	//详情图
	    		'extradesc': [{'key': 'aaa', 'value': 'bbb'},{'key': 'ccc', 'value': 'ddd'}]	//额外描述 		    		
	    		}	    		
	    	],			//end groupinfo
	    'discountprice': '229',		//售价
	    'sellingprice': '230',			//原价
	    'vendor': 'ABC',			//厂家
	    'unit': '捆',				//规格
	    'coverimg': 'http://company.com/images/NBKSR000000065.jpg',	//主图
	    'detailimgs': ['http://company.com/detailimages/NBKSR000000065_1.jpg', 'http://company.com/detailimages/NBKSR000000065_2.jpg'],	//详情图
    }
}```