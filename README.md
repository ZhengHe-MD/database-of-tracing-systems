# Database of tracing systems

## 项目背景

[AP](http://www.cs.cmu.edu/~pavlo/) 在 2014 年建立了网站 [dbdb.io](https://dbdb.io/)，即 Database of Databases，从一些固定的设计维度来分析市面上琳琅满目的数据库系统。受它启发，我们是否也可以找到一些相对固定的设计维度，来分析市面上的调用链追踪系统，从而获得更加系统的理解？

恰好在调研的过程中，在多方引荐下阅读了 [So, you want to trace your distributed system?](https://www.pdl.cmu.edu/PDL-FTP/SelfStar/CMU-PDL-14-102.pdf) 这篇论文，里头介绍了一些四个重要的设计维度：**因果关系**、**追踪方式**、**采样策略** 以及 **数据可视化** (详情可参考我的[分享: 调用链追踪的设计决定及伴鱼的实践经验](./shares/design-decisions-of-tracing-systems-and-practical-experiences-in-palfish.md))，我们不妨就以它为起点，来尝试解构市面上的调用链追踪系统。

## 追踪系统列表

* [Jaeger](./Jaeger.md)
* [Canopy](./Canopy.md)

## 标准维度

针对每个现存的解决方案，我们通过 **普通维度** 和 **设计维度** 来分别考量。

### 普通维度

* [基本信息](./dimensions/normal/basics.md)
* [项目历史](./dimensions/normal/history.md)
* [使用场景](./dimensions/normal/use-cases.md)

### 设计维度

* [因果关系](./dimentions/design/causality.md)
* [追踪方式](./dimentions/design/tracking.md)
* [采样策略](./dimentions/design/sampling.md)
* [数据可视化](./dimentions/design/visualization.md)

## 贡献

### 方式

任何一位开发者，都可以通过至少 3 种方式贡献你的见解：

1. 贡献维度：
   * 新增你认为遗漏的维度
   * 修改或补充某维度的说明
2. 贡献场景：
   * 新增你认为遗漏的场景
   * 修改或补充某场景的说明
3. 贡献追踪系统：
   * 新增你感兴趣的系统名称，等待他人调研
   * 新增你对某系统的调研结果
   * 修改或补充某追踪系统的文档

### 流程

* 在贡献之前，请务必在项目中开一个 issue
* 完成你的贡献内容，并通过 PR 提交

