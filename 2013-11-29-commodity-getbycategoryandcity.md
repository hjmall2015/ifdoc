---
category: Stuff
path: '/app/commodity/getCommunityStorage'
title: '[B2]按小区和类别获得商品列表'
type: 'POST'

layout: nil
---

获得某类别及其子类别下所有商品(零售店仓库)的列表, 带库存有无信息, 带分页．其中类别属性可为空, 等级任意, 默认所有类别; 排序标准可为空, 可选价格、总销量、收藏量,  默认按总销量排序; 排序方向可为空, 默认降序.

### Request


```{
    'data': {
	'categorycode': 'all.daily',		//类别代码
	'communityareaid': 3999,	//小区的areaid
	'orderby': 'price',		//排序标准 -- 价格:price; 总销量:sales;收藏量: fav(暂不可用);
	'orderbydirection': 'asc'	//排序方向 -- 升序:asc; 降序:desc
	'start': 0,			//分页信息
	'limit': 25			//分页信息
    }
}```

### Response

**如果成功**, 返回所有区域的商品列表．每个商品包括编号、名称、售价、原价、本区域库存有无、总销量. 注:为了防止后台属性名使用混淆, 现价属性名暂定为discountprice, 原价属性名暂定为sellingprice, 如这样命名有问题再讨论. 

例1:
```{
    'success': true,
    'data':{
	items:[
	{
	    'code':'I_6000000000002',		//商品编号
	    'name':'IPhone6土豪金',			//商品名称
	    'vendor': '桔子',				//商品厂家
	    'price': '5000',			//商品现价, 注意是字符串类型(如'5000','5000-5500')
	    'sales': 3209,				//总销量	    
	    'hasstock': true,			//区域是否有货
	    'coverimg': 'http://company.com/images/NBKSR000000065.jpg'	//主图	    
	},
	...
	],
	count:273			//总数
    }
}```

例2:
```{
    'success': true,
    'data':{
	items:[
	{
	    'code':'S_0002',			//商品编号
	    'name':'ABC牌针织衫',		//商品名称
	    'discountprice': '229',		//商品现价, 注意是字符串类型(如'5000','5000-5500')
	    'sellingprice': '230',		//商品原价, 注意是字符串类型(如'5000','5000-5500')
	    'sales': 506,			//总销量	    
	    'hasstock': true,			//区域是否有货
	    'coverimg': 'http://company.com/images/NBKSR000000065.jpg'	//主图
	},
	...
	],
	count:273			//总数
    }
}```
