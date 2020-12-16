# Database of tracing systems

## 项目背景

[AP](http://www.cs.cmu.edu/~pavlo/) 在 2014 年建立了网站 [dbdb.io](https://dbdb.io/)，即 Database of Databases，从一些固定的设计维度来分析市面上琳琅满目的数据库系统。受它启发，我们是否也可以找到一些相对固定的设计维度，来分析市面上的调用链追踪系统，从而获得更加系统化的理解？

恰好在调研的过程中，在多方引荐下阅读了 [So, you want to trace your distributed system?](https://www.pdl.cmu.edu/PDL-FTP/SelfStar/CMU-PDL-14-102.pdf) 这篇论文，文章中介绍了四个重要的设计维度：**因果关系**、**追踪方式**、**采样策略** 以及 **数据可视化** (详情可参考我的[分享: 调用链追踪的设计决定及伴鱼的实践经验](./shares/design-decisions-of-tracing-systems-and-practical-experiences-in-palfish.md))，我们不妨就以它为起点，来尝试解构市面上的调用链追踪系统。

## 案例分析

* [Jaeger](./Jaeger.md)
* [Canopy](./Canopy.md)

## 分析维度

针对每个现存的解决方案，我们通过 **事实维度** 和 **设计维度** 来分别考量。

### 事实维度

* [基本信息](./dimensions/facts/basics.md)
* [项目历史](./dimensions/facts/history.md)
* [使用场景](./dimensions/facts/use-cases.md)

### 设计维度

* [因果关系](./dimensions/design/causality.md)
* [追踪方式](./dimensions/design/tracking.md)
* [采样策略](./dimensions/design/sampling.md)
* [数据可视化](./dimensions/design/visualization.md)

## 贡献

### 流程

* 在贡献之前，请务必在项目中新建或认领一个 issue，避免重复劳动
* 完成你的贡献内容，并通过 PR 提交

### 内容

本项目中的任意文档都可以修改。此外，任意开发者都至少可以从以下 3 个角度贡献你的见解或调研成果：

1. 维度
2. 使用场景
3. 案例分析

##### 维度

你可以新增分析维度，也可以修改或补充某分析维度的说明。如果是新增维度请务必同时修改本文件。

##### 使用场景

你可以新增使用场景，也可以修改或补充某使用场景的说明。如果是新增使用场景请务必同时修改本文件。

##### 案例分析

你可以新增感兴趣的系统名称，等待他人调研或自己认领调研，也可以新增你对某追踪系统的调研结果。如果是新增调研结果请务必同时修改本文件。

案例分析文件中需要注意以下几点：

* 一级标题：项目名称
* 二级标题：维度名称

