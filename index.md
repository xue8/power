## 生产力

## 全文检索
- [bleve](https://github.com/blevesearch/bleve)：单机版全文检索

## api

### openapi
- [OpenAPI.Tools](https://openapi.tools/)：OpenAPI 工具集

## Golang

### 数据结构
- [emirpasic/gods](https://github.com/emirpasic/gods)：常用数据结构 Golang 实现

### 测试
- [golang/mock](https://github.com/golang/mock)：mock 框架（用于 interface mock）
- [smartystreets/goconvey](https://github.com/smartystreets/goconvey)：测试用例管理工具
- [prashantv/gostub](https://github.com/prashantv/gostub)：变量、过程、函数打桩


## 可观测性
一个好的观察系统最后要做到的形态:终态就是实现Metrics、Tracing、Logging的融合。
这三者在可观察性上缺一不可,基于Metrics的告警发现异常，通过Tracing定位问题(可疑)模块，根据模块具体的Logging定位到错误根源，最后再基于这次问题调查经验调整Metrics(增加或者调整报警阈值等)以便下次可以更早发现/预防此类问题。

### 协议
- [OpenTelemetry](https://opentelemetry.io/)：OpenTelemetry的终态就是实现Metrics、Tracing、Logging的融合，作为CNCF可观察性的终极解决方案。


### tracing
提供了一个请求从接收到处理完毕整个生命周期的跟踪路径，通常请求都是在分布式的系统中处理，所以也叫做分布式链路追踪。


### metric
提供量化的系统内/外部各个维度的指标，一般包括Counter、Gauge、Histogram等。

- [prometheus/prometheus](https://github.com/prometheus/prometheus)

### log
提供系统/进程最精细化的信息，例如某个关键变量、事件、访问记录等。

- [grafana/loki](https://github.com/grafana/loki)：是一个水平可扩展，高可用性，多租户的日志聚合系统。它的设计非常经济高效且易于操作，因为它不会为日志内容编制索引，而是为每个日志流编制一组标签
- ELK
- EFK

## 云原生
### 开发环境
- [gitpod-io/gitpod](https://github.com/gitpod-io/gitpod)：Gitpod 是一个基于 Chorom Cloud 平台的在线 IDE，它可以快速的启动一个基于大多数流行语言的开发环境，并且可以很顺畅的进行开发
- [OAM](https://oam.dev/)：开放应用模型定义（ Open Application Model Specification），为构建于云原生之上的应用构建了一套规范
- [KubeVela](https://kubevela.io/)：基于 OAM 模型构建的 PaaS 平台
- [服务目录 Service Catalog](https://kubernetes.io/zh/docs/concepts/extend-kubernetes/service-catalog/)：服务目录（Service Catalog），为部署在 K8s 之上的应用提供使用 K8s 外部服务的能力，提供了 Service Broker、Serivce Binding 等概念，其中 Service Broker 遵循 Open Service Broker 标准。服务目录可以检索、供应、和绑定由 服务代理人（Service Brokers） 提供的外部托管服务（Managed Services）
- [Open Service Broker](https://www.openservicebrokerapi.org/)：开放服务代理 API（Open Service Broker），为 Service Broker 构建了标准的 API。Service Broker 为服务的创建、销毁、管理等全生命周期构建了一套规范，方便服务提供商之外的平台使用服务，可以简单理解为服务代理构建了一套标准协议。Service Broker 并不是云原生提出的概念，它源自于Pivotal公司在2011年开源的PaaS(Platform-as-a-Service)项目Cloud Foundry。Service Broker 也并不一定运行在 K8s 上

### 开放标准
#### [开放容器标准OCI](https://opencontainers.org/)
##### 镜像标准
标准：
- [镜像标准image-spec](https://github.com/opencontainers/image-spec)：定义了镜像的标准，让标准镜像能够在不同的容器软件中打包、上传和下载

实现：
- moby/buildkit：从 docker build 拆分出来的项目，支持自动 GC，多种输入和输出格式，并发依赖解析，分布式 Worker 和 Rootless 执行等特性
- genuinetools/img：对 buildkit 的一层封装，单独的二进制，没有 daemon，支持 Rootless 执行，会自动创建 SUBUID，比 buildkit 使用起来更加容易
- uber/makisu：uber 开源的内部镜像构建工具，目标是在 Mesos 或 Kubernetes 上进行 Rootless 构建，支持的 Dockerfile 有些许不兼容，在非容器环境下运行会有问题，比如 Image failed to build without modifyfs
- GoogleContainerTools/kaniko：Google 出品，目标是 Daemon free build on Kubernetes，要求运行镜像 gcr.io/kaniko-project/executor 进行构建，直接在别的镜像中使用二进制可能会不工作，很蠢
- containers/buildah：开源组织 Containers 推出的项目，目标是构建 OCI 容器镜像，Daemon free，支持 Rootless 构建

##### 运行时标准


## 模板引擎
- [jinja2](http://docs.jinkan.org/docs/jinja2/)：功能强大的模板引擎

## 翻译工具
- [DeepL](https://www.deepl.com/translator)：翻译能力比 Google 强大

## 业务洞察
### 行业数据
- [发现报告](https://www.fxbaogao.com/?stop=1)：行业分析报告平台
- [topklout](http://www.topklout.com/#/home)：专业的行业分析服务商

#### 互联网
- [TooBigData](https://toobigdata.com/)：网红数据库
- [5118](https://www.5118.com/)：营销大数据 - 智能原创改写,长尾词挖掘,营销情报,站长工具
- [生财有术](https://www.shengcaiyoushu.com/)：一个谈钱不伤感情的社群 

## 微信行业解决方案
### 微信公众号
- [微擎](https://www.w7.cc/)：微信公众号管理系统


## 音视频工具
### 视屏
- [Open Broadcaster Software-OBS](https://obsproject.com/)：好用的推流、录屏软件
- [Final Cut Pro](https://www.apple.com/final-cut-pro/)：专业的视频剪辑软件

## 产品
### DevOps领域
- [优维科技官网-DevOps专家-EasyOps-应用CMDB-自动化运维-持续交付](https://www.uwintech.cn/)
