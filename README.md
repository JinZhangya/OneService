# OneService

## 简介
------------

### 目录
------------
```
.
├── README.md
├── pom.xml
├── service-claim
│   ├── README.md
│   ├── pom.xml
│   └── src
│       ├── main
│       │   ├── java
│       │   │   └── com
│       │   │       └── fulan
│       │   │           └── claim
│       │   │               ├── application ((应用层):它主要存放应用层服务组合和编排相关的代 码)
│       │   │               │   ├── event ((事件):这层目录主要存放事件相关的代码)
│       │   │               │   │   ├── publish (事件发布相关代码)
│       │   │               │   │   └── subscribe (事件订阅相关代码)
│       │   │               │   └── service (应用服务):这层的服务是应用服务
│       │   │               ├── domain ((领域层):它主要存放领域层核心业务逻辑相关的代码)
│       │   │               │   ├── demoAggregate01 ((聚合):它是聚合软件包的根目录，可以根据实际项目的 聚合名称命名，比如权限聚合)
│       │   │               │   │   ├── entity ((实体):它存放聚合根、实体、值对象以及工厂模式 (Factory)相关代码)
│       │   │               │   │   ├── event ((事件):它存放事件实体以及与事件活动相关的业务逻辑代码)
│       │   │               │   │   ├── repository ((仓储):它存放所在聚合的查询或持久化领域对象的代 码，通常包括仓储接口和仓储实现方法)
│       │   │               │   │   └── service ((领域服务):它存放领域服务代码。一个领域服务是多个实体 组合出来的一段业务逻辑)
│       │   │               │   └── demoAggregate02
│       │   │               │       ├── entity
│       │   │               │       ├── event
│       │   │               │       ├── repository
│       │   │               │       └── service
│       │   │               ├── infrastructure ((基础层):它主要存放基础资源服务相关的代码，为其它各层提供的通用技术能力、三方软件包、数据库服务、配置和基础资源服务的代码)
│       │   │               │   ├── config (主要存放配置相关代码)
│       │   │               │   └── util (主要存放平台、开发框架、消息、数据库、缓存、文件、总线、网 关、第三方类库、通用算法等基础代码，你可以为不同的资源类别建立 不同的子目录)
│       │   │               │       ├── api
│       │   │               │       ├── driver
│       │   │               │       └── mq
│       │   │               └── interfaces ((用户接口层):它主要存放用户接口层与前端交互、展现 数据相关的代码)
│       │   │                   ├── assembler (实现DTO与领域对象之间的相互转换和数据交换)
│       │   │                   ├── dto (它是数据传输的载体，内部不存在任何业务逻辑，我们可以通过 DTO把内部的领域对象与外界隔离)
│       │   │                   └── facade (提供较粗粒度的调用接口，将用户请求委派给一个或多个应用 服务进行处理)
│       │   └── resources
│       └── test
│           └── java
├── service-policy
│   ├── README.md
│   ├── pom.xml
│   └── src
│       ├── main
│       │   ├── java
│       │   └── resources
│       └── test
│           └── java
├── service-preservation
│   ├── README.md
│   ├── pom.xml
│   └── src
│       ├── main
│       │   ├── java
│       │   └── resources
│       └── test
│           └── java
├── service-receipt-visit
│   ├── README.md
│   ├── pom.xml
│   └── src
│       ├── main
│       │   ├── java
│       │   └── resources
│       └── test
│           └── java
├── sevice-payment
│   ├── README.md
│   ├── pom.xml
│   └── src
│       ├── main
│       │   ├── java
│       │   └── resources
│       └── test
│           └── java
