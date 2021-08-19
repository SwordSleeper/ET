# [English](https://github.com/egametang/Egametang/blob/master/README-EN.md) 

__讨论QQ群 : 474643097__  

[ET论坛](https://et-framework.cn)  

# 本项目是ET6.0接入ILRuntime热更新的示例，后续将保持维护状态，与ET同步更新。

接入ILRtuntime教程地址：[https://www.lfzxb.top/et-6-with-ilruntime/](https://www.lfzxb.top/et-6-with-ilruntime/) (完全仿照ET 5.0接入ILRuntime的思路进行开发的) 但已过时，出于学习的目的，可以前往：[et6以5.0思路接入ilrt里程碑](https://github.com/wqaetly/ET/releases/tag/ilrt-change) 进行查看

**当前master采用了一种与上述博客不同的，全新的思路**

- 热更层：当前master会把Model, ModelView，Hotfix，HotfixView打成一个程序集，然后以全热更的方式进行，最大限度保留了ET的结构，方便后续跟进更新
- 非热更层：Unity.Mono，整个框架的底层驱动，网络协议的收发与序列化都在这里

# ET的介绍：

ET是一个开源的游戏客户端（基于unity3d）服务端双端框架，服务端是使用C# .net core开发的分布式游戏服务端，其特点是开发效率高，性能强，双端共享逻辑代码，客户端服务端热更机制完善，同时支持可靠udp tcp websocket协议，支持服务端3D recast寻路等等

# TODO && Features

- [x] 接入ILRuntime
- [ ] 接入xAsset作为资源管理方案（必要，因为当前非热更层直接从Resources目录加载的Hotfix Dll和配置数据，而这些数据理应是热更的）

# 引用

[ET学习笔记](https://www.lfzxb.top/)

[状态帧同步Moba，包含基于双端行为树技能系统](https://gitee.com/NKG_admin/NKGMobaBasedOnET)

[ET框架视频教程-6.0版本](https://space.bilibili.com/33595745/favlist?fid=759596845&ftype=create)

[91焦先生ET-ILRuntime](https://github.com/mister91jiao/ET_ILRuntime/)
