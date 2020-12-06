
# [Kubernetes面试知识点](https://github.com/stevenli91748/Big-Data/blob/master/Kubernetes/Kubernetes%E9%9D%A2%E8%AF%95%E7%9F%A5%E8%AF%86%E7%82%B9/README.md)

<a href="https://ibb.co/mqHJ8Fc"><img src="https://i.ibb.co/wWKysrz/kubernetes.png" alt="kubernetes" border="0"></a>

[精尽 Kubernetes 学习指南](http://svip.iocoder.cn/Kubernetes/tutorials/)|[在程序中调用Kubernetes API操作Kubernetes](https://github.com/stevenli91748/Big-Data/blob/master/Kubernetes/Kubernetes%20API/README.md)|
---|---|

# 目录

* [Kubernetes实验](https://github.com/stevenli91748/Big-Data/blob/master/Kubernetes/Kubernetes%E5%AE%9E%E9%AA%8C/README.md)
* [Kubernetes 特性](#Kubernetes-特性)
* [Kubernetes组件]()
  * [Master Node]()
    * [kubectl---与Kubernetes集群打交道的客户端]()
    * [API Server---接收kubectl客户端的请求]()
    * [Controller-Manaager---APIServer接收到请求后具体分配Worker Node进行内容创建]()
      * [Replication]()
      * [Namespace]()
      * [Service]()
    * [Scheduler---APIServer接收到请求后通过Scheduler的调度策略选择对应的Worker node]()
    * [ETCD---集群中配置等信息存储]()
  * [Worker Node]()
     * [kubelet---调用Docker Engine创建对应的pod]()
     * [Kube-proxy---维护节点上的网络规则。这些网络规则允许从集群内部或外部的网络会话与 Pod 进行网络通信]()
     * [Pod]()
       * [Pause容器]()
       * [业务容器]()
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
* [k8S 搭建集群](https://www.shuzhiduo.com/A/Ae5RKvVYdQ/)
* [Kubernetes 是什么？](https://kubernetes.io/zh/docs/concepts/overview/what-is-kubernetes/)
* [分享我的k8s学习过程](https://zhuanlan.zhihu.com/p/262181124?utm_source=wechat_session&utm_medium=social&utm_oi=991812777480134656)
* [一文带你彻底厘清 Kubernetes 中的证书工作机制](https://zhuanlan.zhihu.com/p/142990931)
