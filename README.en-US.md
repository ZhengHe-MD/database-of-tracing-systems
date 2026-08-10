

# Database of tracing systems

## Project Background

In 2014, [AP](http://www.cs.cmu.edu/~pavlo/) launched the website [dbdb.io](https://dbdb.io/), the Database of Databases, to analyze the myriad database systems on the market across several fixed dimensions. Inspired by this, can we also identify a set of relatively fixed dimensions to analyze the distributed tracing systems available today? This would allow for a more systematic understanding and help us document our analysis and research findings.

During our research, we happened to read the paper [So, you want to trace your distributed system?](https://www.pdl.cmu.edu/PDL-FTP/SelfStar/CMU-PDL-14-102.pdf), which introduces four critical design dimensions for distributed tracing systems: **Causality**, **Tracing Approach**, **Sampling Strategy**, and **Data Visualization**. We will use this paper as a starting point to attempt to deconstruct real-world tracing systems and document them in this database.

## Analysis Dimensions

For each existing solution, we evaluate it across two categories: **Fact Dimensions** and **Design Dimensions**.

### Fact Dimensions

* [Basic Information](./dimensions/facts/basics/README.md)
* [Project History](./dimensions/facts/history/README.md)
* [Use Cases](./dimensions/facts/use-cases/README.md)

### Design Dimensions

* [Basic Architecture](/dimensions/design/architecture/README.md)
* [Tracing Data Model](./dimensions/design/tracing-model/README.md)
* [Metadata Schema](./dimensions/design/metadata/README.md)
* [Causality](./dimensions/design/causality/README.md)
* [Sampling Strategy](./dimensions/design/sampling/README.md)
* [Data Visualization](./dimensions/design/visualization/README.md)

Since these dimensions are not strictly orthogonal and have interrelationships, each case study will selectively cover only the relevant design dimensions based on the specific system.

## Case Studies

* [Canopy](./Canopy/README.md)
* [Jaeger](./Jaeger/README.md)

Note: Listed in alphabetical order.

## Videos

* [Design of Distributed Tracing Systems in the Microservices Era | InfoQ Open Course](https://www.infoq.cn/video/Kf4DaZ1C862juiMS84J8)

## Articles

* [Distributed Tracing Systems at Ban Yu: Theory (Design Dimensions of Tracing Systems)](https://zhenghe-md.github.io/blog/2020/12/20/design-dimensions-of-tracing-systems/)
* [Distributed Tracing Systems at Ban Yu: Practice](https://zhenghe-md.github.io/blog/2021/03/04/implementing-tail-based-sampling/)

## Contributing

[How to contribute?](./CONTRIBUTING.md)
