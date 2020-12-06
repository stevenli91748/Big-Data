**Service （服务）是分布式集群架构的核心， 一个Service 对象拥有如下关键特征。**

* 拥有一个唯一指定的名字（比如mysq l-server ）。
* 拥有一个虚拟E (Cluster E 、Service IP 或VIP ）和端口号。
* 能够提供某种远程服务能力。
* 被映射到了提供这种服务能力的一组容器应用上。

**Service 的服务进程目前都基于Socket 通信方式对外提供服务，比如Redis 、Memcache 、MySQL 、Web Server ，或者是实现了某个具体业务的一个特定
的TCP K凹er 进程。虽然一个Service 通常由多个相关的服务进程来提供服务，每个服务进程都有一个独立的EndpointCIP+Port ）访问点，但Kubemetes 
能够让我们通过Service （虚拟Cluster IP +Service p。此〉连接到指定的Service 上。有了Kubemetes 内建的透明负载均衡和故障恢复机制，不管后端有
多少服务进程，也不管某个服务进程是否会由于发生故障而重新部署到其他机器，都不会影响到我们对服务的正常调用。更重要的是这个Service 本身一旦创建就
不再变化，这意味着在Kubernetes集群中，我们再也不用为了服务的E 地址变来变去的问题而头疼了。**
