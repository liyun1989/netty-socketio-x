# netty-socketio-x：SocketIO插件集合

Netty-SocketIO是Redisson作者mrniko基于nodeJS版本开发的基于java语言的socketio websocket协议的socket服务器端，基于高性能的netty实现。

https://github.com/mrniko/netty-socketio

本项目使用netty-socketio 最新版本v1.7.17开发和测试

## 插件集合

1. 高效（替换原生基于反射）的事件触发器
2. 通信和事件解耦的同步和异步任务处理器
3. 连接和自定义认证反馈的协议支持
4. 基于原生事件和消息处理器的自定义拦截器和过滤器
5. 完整的监控（采集、输出）支持

## 场景支持

netty-socketio是基于websocket协议的双工实时通信协议，环境上支持多客户端，能够在web和native app上具备良好的兼容特性。

1. 游戏实时交互
2. IM、推送
3. 其他实时通信场景

## Netty-SocketIO客户端

支持socketio的所有客户端均可兼容，具体版本见netty-socketio介绍

## 为何有这些插件

netty-socketio基本上可以理解为已经停止维护的项目，但是在稳定性兼容性上已经有比较好的沉淀，在基于netty-socketio进行某些复杂的通信场景时，现有功能无法满足特定的场景覆盖。

## 如何使用

基于Spring-boot-starter方式，集成即可启用上述提到的功能，按需开启

## 功能介绍

TODO

## 不支持的场景

1. 分布式的连接管理场景，原生使用memoryStore,官方提供了Redis支持
2. 常规websocket和ssl websocket同时启用规则,需要使用特定的netty-socketio fork版本
https://github.com/socketside/netty-socketio
