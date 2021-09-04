
# [Kubernetes面试知识点](https://github.com/stevenli91748/Big-Data/blob/master/Kubernetes/Kubernetes%E9%9D%A2%E8%AF%95%E7%9F%A5%E8%AF%86%E7%82%B9/README.md)

<a href="https://ibb.co/mqHJ8Fc"><img src="https://i.ibb.co/wWKysrz/kubernetes.png" alt="kubernetes" border="0"></a>

<a href="https://ibb.co/d4W0MVT"><img src="https://i.ibb.co/tpmMKvG/kubernetes1.png" alt="kubernetes1" border="0"></a>


[精尽 Kubernetes 学习指南](http://svip.iocoder.cn/Kubernetes/tutorials/)|[在程序中调用Kubernetes API操作Kubernetes](https://github.com/stevenli91748/Big-Data/blob/master/Kubernetes/Kubernetes%20API/README.md)|[Kubernetes 中文指南/云原生应用架构实践手册](https://jimmysong.io/kubernetes-handbook/)|
---|---|---|

[Kubernetes中文社区](https://www.kubernetes.org.cn/)|[周志明 如何部署 Kubernetes 集群](https://icyfenix.cn/appendix/deployment-env-setup/setup-kubernetes/)|
---|---|


[如何基于K8s(Kubernetes)部署成PaaS/DevOps(一套完整的软件研发和部署平台)](https://github.com/ben1234560/k8s_PaaS)|
---|


[阿里巴巴 云原生技术实践公开课---从零开始实践 Kubernetes](https://developer.aliyun.com/lesson_2174_21484#_21484)|[Service Mesher社区---istio资料](https://www.servicemesher.com/)|
---|---|

[阿里巴巴 知行动手实验室](https://start.aliyun.com/)|[Spring on Kubernetes](https://spring.io/guides/topicals/spring-on-kubernetes/)|
---|---|

[SpringCloud 应用在 Kubernetes 上的最佳实践 — 部署篇(工具部署)](https://www.kubernetes.org.cn/8078.html)|[SpringCloud 应用在 Kubernetes 上的最佳实践 —— 开发篇](https://mp.weixin.qq.com/s?__biz=MzUzNzYxNjAzMg==&mid=2247491668&idx=1&sn=c9839f78ff31d6f5da285a259d804f53&chksm=fae6eb9bcd91628d28b0db9b53a091132df7535d320aee9c85fea241dc4e964e746b83a69dc8&scene=21#wechat_redirect)|[SpringCloud 应用在 Kubernetes 上的最佳实践 — 部署篇（开发部署）](https://mp.weixin.qq.com/s?__biz=MzUzNzYxNjAzMg==&mid=2247492052&idx=1&sn=8ff93e6f7b398e6a509239910b61b975&scene=21#wechat_redirect)|
---|---|---|

[使用 Java 操作 Kubernetes API](https://www.kubernetes.org.cn/8984.html)|
---|

# Mybird

* [Kubernetes服务发现总结](https://mrbird.cc/Kubernetes-Service-Discovery-Summary.html)
* [Kubernetes Ingress](https://mrbird.cc/Kubernetes-Ingress.html)
* [Kubernetes StatefulSet](https://mrbird.cc/Kubernetes-StatefulSet.html)
* [Kubernetes StorageClass实践](https://mrbird.cc/Kubernetes-StorageClass-Practice.html)
* [Kubernetes PV/PVC](https://mrbird.cc/Kubernetes-PV-PVC.html)
* [Kubernetes资源管理](https://mrbird.cc/Kubernetes-Resource-Management.html)
* [Kubernetes Namespace&Context](https://mrbird.cc/Kubernetes-Namespaces-Context.html)
* [Kubernetes Service基础](https://mrbird.cc/Kubernetes-Service-Basic.html)
* [Kubernetes Pod扩容与缩容](https://mrbird.cc/Kubernetes-Pod-Expansion-Contraction.html)
* [Kubernetes Pod升级与回滚](https://mrbird.cc/Kubernetes-Pod-Upgrade-And-Rollback.html)
* [Kubernetes Pod管理对象与调度策略](https://mrbird.cc/Kubernetes-Pod-Mananger.html)
* [Kubernetes Pod基础](https://mrbird.cc/Kubernetes-Pod-Basic.html)
* [Kubernetes基础](https://mrbird.cc/Kubernetes-Basic.html)
* [Kubernetes1.16.2安装Dashboard](https://mrbird.cc/Kubernetes1-16-2-install-Dashboard.html)
* [Kubeadm安装Kubernetes1.16.2集群](https://mrbird.cc/Kubeadm-install-Kubernetes1-16-2-cluster.html)


# 目录
* [kubertes命令]()
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
      * [进击的 Kubernetes 调度系统（一）：Kubernetes scheduling framework](https://www.kubernetes.org.cn/7983.html)
    * [ETCD---集群中配置等信息存储](https://github.com/stevenli91748/Big-Data/blob/master/Kubernetes/Kubernetes%E7%BB%84%E4%BB%B6/master%E8%8A%82%E7%82%B9/ETCD.md)
  * [Worker Node](https://github.com/stevenli91748/Big-Data/blob/master/Kubernetes/Kubernetes%E7%BB%84%E4%BB%B6/%E5%B7%A5%E4%BD%9C%E8%8A%82%E7%82%B9/README.md)
    * [kubelet---调用Docker Engine创建对应的pod]()
    * [Kube-proxy---维护节点上的网络规则。这些网络规则允许从集群内部或外部的网络会话与 Pod 进行网络通信]()
    * [Pod](https://github.com/stevenli91748/Big-Data/blob/master/Kubernetes/Kubernetes%E7%BB%84%E4%BB%B6/%E5%B7%A5%E4%BD%9C%E8%8A%82%E7%82%B9/Pod.md)
       * [Pause容器]()
         * [Pod内数据的存储管理](https://github.com/stevenli91748/Big-Data/blob/master/Kubernetes/Kubernetes%E7%BB%84%E4%BB%B6/%E5%B7%A5%E4%BD%9C%E8%8A%82%E7%82%B9/Pod%E5%86%85%E6%95%B0%E6%8D%AE%E7%9A%84%E5%AD%98%E5%82%A8%E7%AE%A1%E7%90%86.md)
       * [业务容器]()
    * [容器引擎]()   
  * [Addons]()     
    * [DNS]()
    * [Web UI(Dashboard)]()
    * [ContainerResource Monitoring]()
    * [Cluster-level Logging]()
* [集群安全机制]()
  * [Kubernetes最佳安全实践](https://www.kubernetes.org.cn/8630.html)
  * [API Server认证管理---Authentication]()
    * [使用 KubeSphere 在 Kubernetes 安装 cert-manager 为网站启用 HTTPS](https://www.kubernetes.org.cn/8289.html)
  * [API Server授权管理---Authorization]()
  * [Admission Control---准入控制]()
  * [Service Account]()
  * [Secret]()
* [Kubernetes存储]()
  * [云原生存储详解：容器存储与 K8s 存储卷](https://www.kubernetes.org.cn/7866.html)
* [Kubernetes网络原理](https://github.com/stevenli91748/Big-Data/blob/master/Kubernetes/Kubernetes%E7%BD%91%E7%BB%9C%E5%8E%9F%E7%90%86/README.md)
  * [Kubernetes选择CNI插件的11个注意事项](https://www.kubernetes.org.cn/8570.html)
  * [1. 容器到容器通信]()
  * [2. Pod到Pod通信]()
  * [3. Pod到Service通信]()
  * [4. Kubernetes的三种外部网络访问方式]()
    * [LoadBalancer](https://github.com/stevenli91748/Big-Data/blob/master/Kubernetes/Kubernetes%E7%BD%91%E7%BB%9C%E5%8E%9F%E7%90%86/LoadBalancer.md)
    * [NodePort](https://github.com/stevenli91748/Big-Data/blob/master/Kubernetes/Kubernetes%E7%BD%91%E7%BB%9C%E5%8E%9F%E7%90%86/NodePort.md)
    * [Ingress](https://github.com/stevenli91748/Big-Data/blob/master/Kubernetes/Kubernetes%E7%BD%91%E7%BB%9C%E5%8E%9F%E7%90%86/Ingress.md)
* [Kubernetes管理工具]()
  * [Kubernetes中优秀的开发或运维工具](https://www.kubernetes.org.cn/7937.html)
  * [日志管理工具]()
    * [2020年Kubernetes中7个最佳日志管理工具](https://www.kubernetes.org.cn/8595.html)
    * [使用 docker-compose 安装 filebeat+redis](http://www.dev-share.top/2019/06/27/%e4%bd%bf%e7%94%a8-docker-compose-%e5%ae%89%e8%a3%85-filebeatredis/)
    * [ELK+logtrail 显示filebeat抓取的日志](http://www.dev-share.top/2019/07/01/elklogtrail-%e6%98%be%e7%a4%bafilebeat%e6%8a%93%e5%8f%96%e7%9a%84%e6%97%a5%e5%bf%97/)
    * [Kubernetes中日志记录和监控模式](https://www.kubernetes.org.cn/7840.html)
  * [k8s网络工具]()
    * [K8S 网络工具](http://www.dev-share.top/2019/12/12/k8s-%e7%bd%91%e7%bb%9c%e5%b7%a5%e5%85%b7/)
  * [开发工具]()
    * [如何基于 K8s 构建下一代 DevOps 平台？](https://www.kubernetes.org.cn/8351.html)
    * [基于开源 KubeSphere 构建跨多集群的云原生 DevOps 平台](https://www.kubernetes.org.cn/8619.html)
    * [深入玩转K8S之Kubernetes1.10中部署dashboard以及常见问题解析](https://blog.51cto.com/devingeng/2096639?source=drt)
    * [kubernetes之Ingress部署](https://blog.51cto.com/newfly/2060587?source=drt)
    * [分布式消息队列RocketMQ部署与监控](https://blog.51cto.com/sofar/1540874?source=drt)
  * 部署 Kubernetes 集群
    * 主流的部署方式
      * [使用 Kubeadm 部署 Kubernetes 集群](https://icyfenix.cn/appendix/deployment-env-setup/setup-kubernetes/setup-kubeadm.html)
      * [使用 Rancher 部署、管理 Kubernetes 集群（其他如 KubeSphere 等在 Kubernetes 基础上构建的工具均归入此类）](https://icyfenix.cn/appendix/deployment-env-setup/setup-kubernetes/setup-rancher.html)
      * [使用 Minikube 在本地单节点部署 Kubernetes 集群（其他如 Microk8s 等本地环境的工具均归入此类）](https://icyfenix.cn/appendix/deployment-env-setup/setup-kubernetes/setup-minikube.html)
    * [调试集群](https://kubernetes.io/zh/docs/tasks/debug-application-cluster/debug-cluster/)
    * [调试那些部署到 Kubernetes 上后没有正常运行的应用](https://kubernetes.io/zh/docs/tasks/debug-application-cluster/debug-application/)
  * [运维监控工具]()
     * [如何以优雅的姿势监控kubernetes](https://www.kancloud.cn/huyipow/prometheus#/catalog)
     * Prometheus
       * [用容器轻松搭建Prometheus运行环境](http://qinghua.github.io/prometheus/)
       * [Prometheus监控Kubernetes的3个配置挑战](https://www.kubernetes.org.cn/8533.html)
       * [Prometheus 配置文件详解](http://www.dev-share.top/2020/09/04/prometheus-%e9%85%8d%e7%bd%ae%e6%96%87%e4%bb%b6%e8%af%a6%e8%a7%a3/)
       * [使用Prometheus+grafana打造高逼格监控平台](https://blog.51cto.com/youerning/2050543?source=drt)
       * [使用 docker-compose 安装 Prometheus+Alertmanager+Grafana](http://www.dev-share.top/2019/06/25/%e4%bd%bf%e7%94%a8-docker-compose-%e5%ae%89%e8%a3%85-prometheusalertmanagergrafana/)
       * [监控实战Prometheus+Grafana](https://cloud.tencent.com/developer/article/1513063?from=article.detail.1751679)
       * [Kubernetes之利用prometheus监控K8S集群](https://blog.51cto.com/newfly/2061135?source=drt)
       * [用Prometheus细化Nginx监控](https://blog.51cto.com/xujpxm/2080146?source=drt)
       * [Kubernetes+Prometheus+Grafana部署笔记](https://blog.51cto.com/kaliarch/2160569?source=drt)
       * [Prometheus应用 blackbox_exporter 监控程序网络状态](http://www.dev-share.top/2020/05/18/prometheus%e5%ba%94%e7%94%a8-blackbox_exporter-%e7%9b%91%e6%8e%a7%e7%a8%8b%e5%ba%8f%e7%bd%91%e7%bb%9c%e7%8a%b6%e6%80%81/)
       * [Prometheus应用 node_exporter 监控机器状态](http://www.dev-share.top/2019/06/21/prometheus%e5%ba%94%e7%94%a8-node_exporter-%e7%9b%91%e6%8e%a7%e6%9c%ba%e5%99%a8%e7%8a%b6%e6%80%81/)
       * [Prometheus应用 mysqld_exporter 监控Mysql](http://www.dev-share.top/2019/06/21/prometheus%e5%ba%94%e7%94%a8-mysqld_exporter-%e7%9b%91%e6%8e%a7mysql/)
     * [Kubernetes集群监控方案](https://blog.51cto.com/ylw6006/2084403?source=drt)
     * [Grafana的使用感受](https://blog.51cto.com/13728665/2114392?source=drt)
       * [Grafana全网最佳实战视频教程合集](https://www.bilibili.com/video/BV1PV411k7Rz/?spm_id_from=333.788.videocard.12)
     * [Kubernetes高可用性监控：Thanos的部署](https://www.kubernetes.org.cn/8308.html)
* [Kubernetes运维]()  
  * 集群升级
    * [如何为 Kubernetes 实现原地升级](https://www.kubernetes.org.cn/7839.html)
    * [Kubernetes 集群升级指南：从理论到实践](https://www.kubernetes.org.cn/8504.html)
    * [更新应用时，如何实现 K8s 零中断滚动更新？](https://www.kubernetes.org.cn/7714.html)
    * [K8S 升级](http://www.dev-share.top/2020/05/01/k8s-%e5%8d%87%e7%ba%a7/)
  * 通过负载均衡访问服务
    * [通过负载均衡访问服务](https://help.aliyun.com/document_detail/86531.html)
  * 容器服务 kubernetes中应用上下线
    * [容器服务 kubernetes（ACK）中应用优雅上下线]()
  * 多集群管理
    * [K8S 多集群切换](http://www.dev-share.top/2020/09/29/k8s-%e5%a4%9a%e9%9b%86%e7%be%a4%e5%88%87%e6%8d%a2/)
    * [Kubernetes 多集群在开源项目 KubeSphere 的应用](https://www.kubernetes.org.cn/8284.html)
    * [灵活、高效的云原生集群管理经验：用 K8s 管理 K8s](https://www.kubernetes.org.cn/7476.html)
  * 集群容器性能指标
    * [K8S 容器性能指标 metrics-server](http://www.dev-share.top/2020/10/25/k8s-%e5%ae%b9%e5%99%a8%e6%80%a7%e8%83%bd%e6%8c%87%e6%a0%87-metrics-server/)
    
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

* [k8s学习笔记-发布一个Pod](https://www.coollf.com/archives/k8s-note-pod-learn)
* [5分钟让你理解K8S必备架构概念，以及网络模型](https://developer.51cto.com/art/202103/649700.htm)
* [架构解密从分布式到微服务：深入Kubernetes微服务平台](https://news.51cto.com/art/202103/650439.htm)
* [重新初始化k8s master节点](https://cloud.tencent.com/developer/article/1706820)
* [使用 KubeSphere 在 Kubernetes 安装 cert-manager 为网站启用 HTTPS](https://www.kubernetes.org.cn/8289.html)
* [Kubernetes 集群搭建 v1.19.3](https://blog.csdn.net/Liing0/article/details/111060199)
* [使用Kuboard界面在k8s上部署SpringCloud项目](https://www.cnblogs.com/sanduzxcvbnm/p/13207317.html)
* [云原生存储详解：容器存储与 K8s 存储卷](https://www.kubernetes.org.cn/7866.html)
* [kubectl技巧之查看资源列表,资源版本和资源schema配置](https://www.cnblogs.com/tylerzhou/p/11043285.html)
* [KubeOperator 是一个开源的轻量级 Kubernetes 发行版](https://github.com/KubeOperator/KubeOperator)
* [kubernetes中文社区](https://www.kubernetes.org.cn/)
* [Kubernetes教程之新手安装必看（快速浏览少走弯路）](https://segmentfault.com/a/1190000022809164)
* [手摸手教你从开发到部署(CI/CD)GO微服务系列](https://learnku.com/docs/go-micro-build/1.0/kubernetes-1804-cluster-installation-tutorial-based-on-centos7/8877)
* [k8S 搭建集群](https://www.shuzhiduo.com/A/Ae5RKvVYdQ/)
* [Kubernetes 是什么？](https://kubernetes.io/zh/docs/concepts/overview/what-is-kubernetes/)
* [分享我的k8s学习过程](https://zhuanlan.zhihu.com/p/262181124?utm_source=wechat_session&utm_medium=social&utm_oi=991812777480134656)
* [一文带你彻底厘清 Kubernetes 中的证书工作机制](https://zhuanlan.zhihu.com/p/142990931)
* [Ingress文件实例](https://blog.csdn.net/qq_39680564/article/details/106220130)
* [Kubernetes持续部署方案](https://blog.csdn.net/qq_39680564/article/details/106081751)
* [Kubernetes研发环境搭建方案](https://blog.csdn.net/qq_39680564/article/details/106022212)
* [Deployment部署实例](https://blog.csdn.net/qq_39680564/article/details/106002185)
* [Service文件实例](https://blog.csdn.net/qq_39680564/article/details/106232120)
* [Kubernetes](https://blog.csdn.net/qq_39680564/category_9985180.html)
* [CKA 学习笔记(一)](http://www.dev-share.top/2020/10/23/cka-%e5%ad%a6%e4%b9%a0%e7%ac%94%e8%ae%b0%e4%b8%80/)
* [CKA 学习笔记(二)](http://www.dev-share.top/2020/10/26/cka-%e5%ad%a6%e4%b9%a0%e7%ac%94%e8%ae%b0%e4%ba%8c/)
* [Kubernetes 新玩法：在 yaml 中编程](https://www.kubernetes.org.cn/8445.html)
* [Kubernetes 忘记token解决方案](https://blog.csdn.net/qq_19734597/article/details/97674360)
* [CI/CD Kubernetes | Setting up CI/CD Jenkins pipeline for kubernetes](https://jhooq.com/ci-cd-jenkins-kubernetes/)
* [Setting up Ingress controller NGINX along with HAproxy for Microservice deployed inside Kubernetes cluster](https://jhooq.com/ingress-controller-nginx/)
* [Deploy spring boot microservice on Google Cloud Platform (GCP)](https://jhooq.com/deploy-spring-boot-microservices-on-kubernetes/#part-2)
* [Deploy Spring Boot microservices on kubernetes](https://jhooq.com/deploy-spring-boot-microservices-on-kubernetes/)
* [How to use Persistent Volume and Persistent Claims | Kubernetes](https://jhooq.com/how-to-use-persistent-volume-and-persistent-claims-kubernetes/)
* [Setting Up kubernetes Dashboard on GKE(Google Kubernetes Engine) on GCP(Google Cloud Platform)](https://jhooq.com/setting-up-kubernetes-dashboard/#gke-kubernetes-dashboard)
* [Setting Up kubernetes Dashboard on On Kubernetes Local cluster](https://jhooq.com/setting-up-kubernetes-dashboard/)
* [Install Kubernetes with Minikube](https://jhooq.com/kubernets-and-minikube/)
* [阿里PB级Kubernetes日志平台建设实践](https://zhuanlan.zhihu.com/p/67497026?utm_source=wechat_session&utm_medium=social&utm_oi=991812777480134656)
* [Kubernetes Deployment 终极指南！](https://zhuanlan.zhihu.com/p/103973666?utm_source=wechat_session&utm_medium=social&utm_oi=991812777480134656)


# Mybird的博客

* [Kubernetes服务发现总结](https://mrbird.cc/Kubernetes-Service-Discovery-Summary.html)
* [Kubernetes Ingress](https://mrbird.cc/Kubernetes-Ingress.html)
* [Kubernetes StatefulSet](https://mrbird.cc/Kubernetes-StatefulSet.html)
* [Kubernetes StorageClass实践](https://mrbird.cc/Kubernetes-StorageClass-Practice.html)
* [Kubernetes PV/PVC](https://mrbird.cc/Kubernetes-PV-PVC.html)
* [Kubernetes资源管理](https://mrbird.cc/Kubernetes-Resource-Management.html)
* [Kubernetes Namespace&Context](https://mrbird.cc/Kubernetes-Namespaces-Context.html)
* [Kubernetes Service基础](https://mrbird.cc/Kubernetes-Service-Basic.html)
* [Kubernetes Pod扩容与缩容](https://mrbird.cc/Kubernetes-Pod-Expansion-Contraction.html)
* [Kubernetes Pod升级与回滚](https://mrbird.cc/Kubernetes-Pod-Upgrade-And-Rollback.html)
* [Kubernetes Pod管理对象与调度策略](https://mrbird.cc/Kubernetes-Pod-Mananger.html)
* [Kubernetes Pod基础](https://mrbird.cc/Kubernetes-Pod-Basic.html)
* [Kubernetes基础](https://mrbird.cc/Kubernetes-Basic.html)
* [Kubernetes1.16.2安装Dashboard](https://mrbird.cc/Kubernetes1-16-2-install-Dashboard.html)
* [Kubeadm安装Kubernetes1.16.2集群](https://mrbird.cc/Kubeadm-install-Kubernetes1-16-2-cluster.html)





---

# online gitbook

* [阿里巴巴 容器服务Kubernetes版教程](https://help.aliyun.com/document_detail/86737.html?spm=a2c4g.11186623.4.1.60ee6ea3yhNq5I)
* [Kubernetes 中文指南/云原生应用架构实践手册](https://jimmysong.io/kubernetes-handbook/)
* [Kuboard v3.0 ---支持多 Kubernetes 集群管理](https://kuboard.cn/install/install-dashboard.html)
* [Kubernetes实践指南](https://k8s.imroc.io/configuration/helm/install-helm/)
* [Serverless Handbook——无服务架构实践手册](https://jimmysong.io/serverless-handbook/)
* [云原生基础架构](https://jimmysong.io/cloud-native-infra/)
* [Istio Handbook——Istio 服务网格进阶实战](https://www.servicemesher.com/istio-handbook/)
* [移到云原生应用架构](https://jimmysong.io/migrating-to-cloud-native-application-architectures/)
* [Hugo 静态网站构建手册--如何使用Hugo构建静态网站用于个人博客或者项目展示](https://jimmysong.io/hugo-handbook/)
