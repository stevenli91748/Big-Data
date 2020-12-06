
在Kubemetes 集群中，你只需为需要扩容的Service 关联的Pod 创建一个RC (Replication Conoiler ），则该Service 的扩容以至于后来的Service 升级等头疼问题都迎刃而解。在一个RC
定义文件中包括以下3 个关键信息。

* 目标Pod 的定义。
* 目标Pod 需要运行的副本数量（ Replicas ）。
* 要监控的目标Pod 的标签（ Label) 。

在创建好RC （系统将自动创建好Pod ）后， Kubemetes 会通过RC 中定义的Label 筛选出对应的Pod 实例井实时监控其状态和数量，如果实例数量少于定义的副本数量（ Replicas ），则会根据RC 中定义的Pod 
模板来创建一个新的Pod ，然后将此Pod 调度到合适的Node 上启动运行，直到Pod 实例的数量达到预定目标。这个过程完全是自动化的，无须人工干预。有了RC,服务的扩容就变成了一个纯粹的简单数字游戏了，只要
修改RC 中的副本数量即可。后续的Service 升级也将通过修改RC 来自动完成。
