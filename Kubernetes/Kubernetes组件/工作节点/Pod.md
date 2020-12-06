**Pod 运行在一个我们称之为节点（ Node)的环境中，这个节点既可以是物理机，也可以是私有云或者公有云中的一个虚拟机，通常在一个节点上运行几百个Pod 
：其次，每个Pod 里运行着一个特殊的被称之为Pause 的容器，其他容器则为业务容器，这些业务容器共享Pause 容器的网络械和Volume 挂载卷，因此它们之
间的通信和数据交换更为高效，在设计时我们可以充分利用这一特性将一组密切相关的服务进程放入同一个Pod 中；最后，需要注意的是，并不是每个Pod 和它
里面运行的容器都能“映射”到一个Service 上，只有那些提供服务（无论是对内还是对外）的一组Pod 才会被“映射”成一个服务。**

**将每个服务进程包装到相应的Pod 中，使其成为Pod中运行的一个容器（ Container ）。为了建立Service 和Pod 间的关联关系， Kubemetes 首先给每
个Pod 贴上一个标签（ Label) ，给运行MySQL 的Pod 贴上name=mysql 标签，给运行Pod 贴上name=php 标签，然后给相应的Service 定义标签选择器（ Label Selector ），比如MySQLService 的标签选择器的选择条件为name=mysql ，意为该Service 要作用于所有包含name=mysql Label 的Pod 上。这样一来，就巧妙地解决了Service 与Pod 的关联问题。**
