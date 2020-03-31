# redis 发布订阅

## 订阅
- 订阅频道
```redshift
subscribe hello_redis
```
- 订阅模式
```redshift
psubscribe 'hello_*'
```

## 退出订阅
- 订阅频道
```redshift
unsubscribe hello_redis
```

- 订阅模式
```redshift
punsubscribe  hello_*
```

## 发布消息
```redshift
publish  hello_redis  "niu bi"
```


## 查看订阅
- 查看所有的订阅频道
```redshift
pubsub channels
```

- 查看频道的订阅数量
```redshift
pubsub numsub hello_redis
```
- 查看订阅的模式数量
```redshift
pubsub numpat hello_redis
```









