# Database of tracing systems

## 项目背景

[AP](http://www.cs.cmu.edu/~pavlo/) 在 2014 年建立了网站 [dbdb.io](https://dbdb.io/)，即 Database of Databases，从一些固定的维度来分析市面上琳琅满目的数据库系统。受它启发，我们是否也可以找到一些相对固定的维度，来分析市面上的调用链追踪系统，从而获得更加系统化的理解，并将分析调研的结果沉淀下来？

在调研的过程中，恰好阅读到 [So, you want to trace your distributed system?](https://www.pdl.cmu.edu/PDL-FTP/SelfStar/CMU-PDL-14-102.pdf) 这篇论文，文章中介绍了调用链追踪系统的四个重要设计维度：**因果关系**、**追踪方式**、**采样策略** 以及 **数据可视化**，我们不妨就以它为起点，来尝试解构实践中的调用链追踪系统，将它们收录到这个数据库中来。

## 分析维度

针对每个现存的解决方案，我们通过「**事实维度**」 和 「**设计维度**」 来分别考量。

### 事实维度

* [基本信息](./dimensions/facts/basics/README.md)
* [项目历史](./dimensions/facts/history/README.md)
* [使用场景](./dimensions/facts/use-cases/README.md)

### 设计维度

* [基本架构](/dimensions/design/architecture/README.md)
* [调用链数据模型](./dimensions/design/tracing-model/README.md)
* [元数据结构](./dimensions/design/metadata/README.md)
* [因果关系](./dimensions/design/causality/README.md)
* [采样策略](./dimensions/design/sampling/README.md)
* [数据可视化](./dimensions/design/visualization/README.md)

由于各个维度之间并不正交，而是存在一定的关联关系，每个案例分析根据实际情况有选择性地介绍部分设计维度即可。

## 案例分析

* [Canopy](./Canopy/README.md)
* [Jaeger](./Jaeger/README.md)

注：按字母顺序排列

## 视频

* [微服务时代的调用链追踪系统设计 | InfoQ 公开课](https://www.infoq.cn/video/Kf4DaZ1C862juiMS84J8)

## 文章

* [调用链追踪系统在伴鱼：理论偏 (调用链追踪系统的设计维度)](https://zhenghe-md.github.io/blog/2020/12/20/design-dimensions-of-tracing-systems/)
* [调用链追踪系统在伴鱼：实践篇](https://zhenghe-md.github.io/blog/2021/03/04/implementing-tail-based-sampling/)

## 贡献

[如何贡献？](./CONTRIBUTING.md)

