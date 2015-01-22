---
category: Stuff
path: '/app/order/notifyPayment'
title: '[O4]支付通知'
type: 'POST'

layout: nil
---

通知已支付.

### Request

```{
    'sessionid': '10760362195',
    'data': {
	'orderserial': 665		//订单编号
	'paymenttype': 'alipay'		//第三方支付类型--alipay:支付宝
    }
}```

### Response

**如果成功**, 返回成功响应．
```{
'success': true,
}```



