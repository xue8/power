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
- [gitpod-io/gitpod](https://github.com/gitpod-io/gitpod)：Gitpod是一个基于Chorom Cloud平台的在线IDE，它可以快速的启动一个基于大多数流行语言的开发环境，并且可以很顺畅的进行开发

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

## 微信行业解决方案
### 微信公众号
- [微擎](https://www.w7.cc/)：微信公众号管理系统
