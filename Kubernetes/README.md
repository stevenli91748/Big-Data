
# [Kubernetes面试知识点](https://github.com/stevenli91748/Big-Data/blob/master/Kubernetes/Kubernetes%E9%9D%A2%E8%AF%95%E7%9F%A5%E8%AF%86%E7%82%B9/README.md)

<a href="https://ibb.co/mqHJ8Fc"><img src="https://i.ibb.co/wWKysrz/kubernetes.png" alt="kubernetes" border="0"></a>

<a href="https://ibb.co/d4W0MVT"><img src="https://i.ibb.co/tpmMKvG/kubernetes1.png" alt="kubernetes1" border="0"></a>


[精尽 Kubernetes 学习指南](http://svip.iocoder.cn/Kubernetes/tutorials/)|[在程序中调用Kubernetes API操作Kubernetes](https://github.com/stevenli91748/Big-Data/blob/master/Kubernetes/Kubernetes%20API/README.md)|[Kubernetes 中文指南/云原生应用架构实践手册](https://jimmysong.io/kubernetes-handbook/)|
---|---|---|

[阿里巴巴 云原生技术实践公开课---从零开始实践 Kubernetes](https://developer.aliyun.com/lesson_2174_21484#_21484)|
---|

[阿里巴巴 知行动手实验室](https://start.aliyun.com/)|
---|

# 目录

* [Kubernetes实验](https://github.com/stevenli91748/Big-Data/blob/master/Kubernetes/Kubernetes%E5%AE%9E%E9%AA%8C/README.md)
* [Kubernetes例子](https://github.com/stevenli91748/Big-Data/blob/master/Kubernetes/Kubernetes%E4%BE%8B%E5%AD%90/README.md)
* [Kubernetes 特性](#Kubernetes-特性)
* [Kubernetes组件]()
  * [Master Node](https://github.com/stevenli91748/Big-Data/blob/master/Kubernetes/Kubernetes%E7%BB%84%E4%BB%B6/master%E8%8A%82%E7%82%B9/README.md)
    * [kubectl---与Kubernetes集群打交道的客户端]()
    * [API Server---接收kubectl客户端的请求]()
    * [Controller-Manaager---APIServer接收到请求后具体分配Worker Node进行内容创建]()
      * [Replication controller](https://github.com/stevenli91748/Big-Data/blob/master/Kubernetes/Kubernetes%E7%BB%84%E4%BB%B6/master%E8%8A%82%E7%82%B9/Controller-Manaager/Replication%20Controller.md)
      * [Namespace Controller]()
      * [Service Controller---是分布式集群架构的核心](https://github.com/stevenli91748/Big-Data/blob/master/Kubernetes/Kubernetes%E7%BB%84%E4%BB%B6/master%E8%8A%82%E7%82%B9/Controller-Manaager/Service.md)
      * [Node Controller]()
      * [ResourceQuota Controller]()
      * [Endpoint Controller]()
    * [Cloud-controller-manager]()
    * [Scheduler---APIServer接收到请求后通过Scheduler的调度策略选择对应的Worker node]()
    * [ETCD---集群中配置等信息存储](https://github.com/stevenli91748/Big-Data/blob/master/Kubernetes/Kubernetes%E7%BB%84%E4%BB%B6/master%E8%8A%82%E7%82%B9/ETCD.md)
  * [Worker Node](https://github.com/stevenli91748/Big-Data/blob/master/Kubernetes/Kubernetes%E7%BB%84%E4%BB%B6/%E5%B7%A5%E4%BD%9C%E8%8A%82%E7%82%B9/README.md)
    * [kubelet---调用Docker Engine创建对应的pod]()
    * [Kube-proxy---维护节点上的网络规则。这些网络规则允许从集群内部或外部的网络会话与 Pod 进行网络通信]()
    * [Pod](https://github.com/stevenli91748/Big-Data/blob/master/Kubernetes/Kubernetes%E7%BB%84%E4%BB%B6/%E5%B7%A5%E4%BD%9C%E8%8A%82%E7%82%B9/Pod.md)
       * [Pause容器]()
       * [业务容器]()
    * [容器引擎]()   
  * [Addons]()     
    * [DNS]()
    * [Web UI(Dashboard)]()
    * [ContainerResource Monitoring]()
    * [Cluster-level Logging]()
* [集群安全机制]()
  * [API Server认证管理---Authentication]()
  * [API Server授权管理---Authorization]()
  * [Admission Control---准入控制]()
  * [Service Account]()
  * [Secret]()
* [Kubernetes网络原理](https://github.com/stevenli91748/Big-Data/blob/master/Kubernetes/Kubernetes%E7%BD%91%E7%BB%9C%E5%8E%9F%E7%90%86/README.md)
* [Kubernetes管理工具]()       
  * [开发工具]()
    * [如何基于 K8s 构建下一代 DevOps 平台？](https://www.kubernetes.org.cn/8351.html)
    * [深入玩转K8S之Kubernetes1.10中部署dashboard以及常见问题解析](https://blog.51cto.com/devingeng/2096639?source=drt)
    * [kubernetes之Ingress部署](https://blog.51cto.com/newfly/2060587?source=drt)
    * [分布式消息队列RocketMQ部署与监控](https://blog.51cto.com/sofar/1540874?source=drt)
  * [部署测试工具]()
    * [调试集群](https://kubernetes.io/zh/docs/tasks/debug-application-cluster/debug-cluster/)
    * [调试那些部署到 Kubernetes 上后没有正常运行的应用](https://kubernetes.io/zh/docs/tasks/debug-application-cluster/debug-application/)
  * [运维监控工具]()
     * [使用Prometheus+grafana打造高逼格监控平台](https://blog.51cto.com/youerning/2050543?source=drt)
     * [Kubernetes之利用prometheus监控K8S集群](https://blog.51cto.com/newfly/2061135?source=drt)
     * [用Prometheus细化Nginx监控](https://blog.51cto.com/xujpxm/2080146?source=drt)
     * [Kubernetes集群监控方案](https://blog.51cto.com/ylw6006/2084403?source=drt)
     * [Grafana的使用感受](https://blog.51cto.com/13728665/2114392?source=drt)
     * [Kubernetes+Prometheus+Grafana部署笔记](https://blog.51cto.com/kaliarch/2160569?source=drt)
  
---

# Kubernetes 特性

      kubernetes优势:

     （1）可移动：公有云、私有云、混合云、多态云
     （2）可扩展：模块化、插件化、可挂载、可组合
     （3）自修复：自动部署、自动重启、自动复制、自动伸缩




[k8s安装-上](https://www.bilibili.com/video/av67180400)|[k8s安装—中](https://www.bilibili.com/video/av67202797)|[k8s安装-下](https://www.bilibili.com/video/av67203001)|
---|---|---|

[k8s-2-几个概念](https://www.bilibili.com/video/av67318105)|[k8s-3-几个组建的工作理解](https://www.bilibili.com/video/av67318156)|[k8s-4-deployment命令部署](https://www.bilibili.com/video/av67318193)|
---|---|---|

[k8s-5-deployment脚本创建](https://www.bilibili.com/video/av67318250)|[k8s-6-yaml简单解读](https://www.bilibili.com/video/av67318272)|[k8s-7-failover](https://www.bilibili.com/video/av67319027)|
---|---|---|


[k8s-8-用label控制pod位置](https://www.bilibili.com/video/av67387104)|[k8s-9-deamonset的应用和案例](https://www.bilibili.com/video/av67394882)|[k8s-10-运行一个daemonSet](https://www.bilibili.com/video/av67394965)|
---|---|---|

[k8s-11-job运行一次性任务](https://www.bilibili.com/video/av67395073)|[k8s-12-job运行失败怎么办](https://www.bilibili.com/video/av67395135)|[k8s-13-并行执行job](https://www.bilibili.com/video/av67395198)|
---|---|---|

[k8s-14-定时执行job](https://www.bilibili.com/video/av67395290)|
---|

[为Kubernetes集群中服务部署Nginx入口服务](https://tonybai.com/2016/11/22/deploy-nginx-service-for-the-services-in-kubernetes-cluster/)|[Kubernetes集群中的Nginx配置热更新方案](https://tonybai.com/2016/11/17/nginx-config-hot-reloading-approach-for-kubernetes-cluster/)|[Kubernetes集群DNS插件安装](https://tonybai.com/2016/10/23/install-dns-addon-for-k8s/)|[Kubernetes从Private Registry中拉取容器镜像的方法](https://tonybai.com/2016/11/16/how-to-pull-images-from-private-registry-on-kubernetes-cluster/)|
---|---|---|---|

[在kubernetes中部署tomcat与mysql集群](https://yq.aliyun.com/articles/506908)|[k8s 部署tomcat完整版](https://blog.csdn.net/weixin_34120274/article/details/92600879?utm_medium=distribute.pc_relevant.none-task-blog-searchFromBaidu-9.not_use_machine_learn_pai&depth_1-utm_source=distribute.pc_relevant.none-task-blog-searchFromBaidu-9.not_use_machine_learn_pai)|
---|---|

# Kubernetes 视频



* [尚硅谷Kubernetes](https://www.bilibili.com/video/av66617940/?spm_id_from=333.788.videocard.9)
* [Kubernetes/K8S 集群环境搭建](https://www.bilibili.com/video/av76793551?from=search&seid=18371074308858678491)
* [Jenkins+K8s实现持续集成](https://www.imooc.com/learn/1112)
* [Manage Your Kubernetes Clusters with Built-in Best Practices---以 Azure Kubernetes Service 为例介绍了如何在托管 Kubernetes 集群上面实现高可用、高扩展、高安全、可观测的应用架构，是运行和维护 Kubernetes 应用最好的参考资料之一](https://info.microsoft.com/ww-thankyou-manage-your-kubernetes-clusters-with-built-in-best-practices-vdeo?LCID=EN-US)

# 有用的参考
* [如何为 Kubernetes 实现原地升级](https://www.kubernetes.org.cn/7839.html)
* [Kubernetes 集群升级指南：从理论到实践](https://www.kubernetes.org.cn/8504.html)
* [Kubernetes 集群搭建 v1.19.3](https://blog.csdn.net/Liing0/article/details/111060199)
* [使用Kuboard界面在k8s上部署SpringCloud项目](https://www.cnblogs.com/sanduzxcvbnm/p/13207317.html)

* [kubectl技巧之查看资源列表,资源版本和资源schema配置](https://www.cnblogs.com/tylerzhou/p/11043285.html)
* [KubeOperator 是一个开源的轻量级 Kubernetes 发行版](https://github.com/KubeOperator/KubeOperator)
* [kubernetes中文社区](https://www.kubernetes.org.cn/)
* [Kubernetes教程之新手安装必看（快速浏览少走弯路）](https://segmentfault.com/a/1190000022809164)
* [ Kubernetes 18.04集群安装教程(基于Centos7)](https://learnku.com/docs/go-micro-build/1.0/kubernetes-1804-cluster-installation-tutorial-based-on-centos7/8877)
* [k8S 搭建集群](https://www.shuzhiduo.com/A/Ae5RKvVYdQ/)
* [Kubernetes 是什么？](https://kubernetes.io/zh/docs/concepts/overview/what-is-kubernetes/)
* [分享我的k8s学习过程](https://zhuanlan.zhihu.com/p/262181124?utm_source=wechat_session&utm_medium=social&utm_oi=991812777480134656)
* [一文带你彻底厘清 Kubernetes 中的证书工作机制](https://zhuanlan.zhihu.com/p/142990931)

---

# online gitbook

* [Kubernetes 中文指南/云原生应用架构实践手册](https://jimmysong.io/kubernetes-handbook/)
* [Kuboard v3.0 ---支持多 Kubernetes 集群管理](https://kuboard.cn/install/install-dashboard.html)
* [Kubernetes实践指南](https://k8s.imroc.io/configuration/helm/install-helm/)
