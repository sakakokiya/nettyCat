# nettyCat基于netty的nio数据流的服务器网关，同时也是网管，承载容器，支持多种协议

网管级网关的思路历程
zuul处理Http请求依赖的是Web容器，性能不如Nginx；
Nginx缺乏更易用的管控、配置方式，加个lua，或者go这种协程级
kong自由扩展困难

然后。。。。
就准备自己写

网关管理平台

- 请求代理
    基本完成
- 服务配置
    - Consul: 未完成
    - Etcd: 未开始
    - Zookeeper: 未开始
- Filter
    jwt oauth2与spring容和
- 限流
    可配置
- 降级
    可手动
- 负载均衡
    未开始 从RestyPass中迁移改造
- 流量切换
    结合负载均衡设计
- 协议转换(http,rpc)
    -支持dubbo
- 动态调整
    - 配置手动方式
    - 配置存储方式
        zk
- 调用链路跟踪
    



