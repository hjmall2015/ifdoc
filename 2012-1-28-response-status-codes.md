---
title: '响应格式及错误码'

layout: nil
---
### 成功

* `GET` `POST ` 无论成功失败，响应消息头部的状态都为200，响应消息体如下


```{
    'success': true,
    'data': ...
}```

### 失败

* `GET` `POST ` 无论成功失败，响应消息头部的状态都为200，各种失败响应的消息体如下

####获取失败(404)
```{
    'success': false,
    'errcode': 404,	
    'message': 'xxx'	
}```

注:　所有接口都可能产生此响应

####认证失败(401)
```{
    'success': false,
    'errcode': 401,	
    'message': 'xxx'	
}```

注:　所有接口都可能产生此响应

####注册失败---验证码错误(601)
```{
    'success': false,
    'errcode': 601,	
    'message': 'xxx'	
}```

####注册失败---未知错误(604)
```{
    'success': false,
    'errcode': 604,
    'message': 'xxx'	
}```

####获取验证码失败(605)
```{
    'success': false,
    'errcode': 605,
    'message': 'xxx'	
}```

####购物车同步失败(631)
```{
    'success': false,
    'errcode': 631,
    'message': 'xxx'	
}```

####购物车删除商品失败(634)
```{
    'success': false,
    'errcode': 634,
    'message': 'xxx'	
}```
