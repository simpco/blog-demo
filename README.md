# blog-demo
blog相关代码实例
1、分析exchange类型
     direct交换器相对来说比较简单，匹配规则为：如果路由键匹配，消息就被投送到相关的队列
     fanout交换器中没有路由键的概念，他会把消息发送到所有绑定在此交换器上面的队列中。
     topic交换器采用模糊匹配路由键的原则进行转发消息到队列中
2、通过死信队列+ttl实现延迟队列	 
