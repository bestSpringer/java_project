## java编写RabbitMQ
**五种工作模式**
* 简单模式
    * 点对点（没有交换机）
* 工作模式
    * 一对多（没有交换机）
    * 多个消费者平均去消费
    * 可以实现能者多劳的场景
* fanout广播模式
    * 引入交换机
    * 一对多，多个消费者都可以消费消息
* 路由模式（direct）
    * 根据routingKey去过滤消息到指定的队列
* 动态路由模式
    * routingKey复杂化
    * \* 代表匹配一个单词
    * \# 代表匹配多个单词
