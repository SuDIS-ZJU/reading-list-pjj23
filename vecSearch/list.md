|paper|conference|remark|
|:---:|:---:|:---:|
|[Approximate Nearest Neighbor Search on High Dimensional Data — Experiments, Analyses, and Improvement](https://ieeexplore.ieee.org/abstract/document/8681160)|TKDE 2020|对目前一些主流ANN search的SOTA做了一个比较全面的实验价值评估（comprehensive experimental evaluation）|
|[Similarity Search Combining Query Relaxation and Diversification](https://browse.arxiv.org/pdf/1611.04689.pdf)|arxiv|找了个新目标函数来平衡similarity和diversity|
|[SPANN: Highly-efficient Billion-scale Approximate Nearest Neighborhood Search](https://arxiv.org/abs/2111.08566)|NEURIPS 2021||
|[CXL-ANNS: Software-Hardware Collaborative Memory Disaggregation and Computation for Billion-Scale Approximate Nearest Neighbor Search](https://www.usenix.org/system/files/atc23-jang.pdf)|ATC 2023|CXL(Computer eXpress Link)一种协议，用于计算机组件之间的互通。针对场景：多台设备在进行ANNS计算，但是有些设备内存比较紧迫，有些设备内存还有很多空的没用。文章用CXL协议最大程度利用了多台设备的内存。同时设计了一些提前cache、prefetch的规则|
|[VBASE: Unifying Online Vector Similarity Search and Relational Queries via Relaxed Monotonicity](https://www.usenix.org/conference/osdi23/presentation/zhang-qianxi)|OSDI 2023|提出了一种relaxed monotonicity的数学定义。作者团队发现ANNS下，对应每一种query存在一种两阶段的特点，向量索引遍历首先近似定位离目标矢量最近的区域，然后以近似方式逐步远离目标区域。据此他们提出一种Relaxed Monotonicity。作者团队根据这一特性进行提前剪枝、并利用单调性的特点将向量索引接洽到传统的火山模型数据库上。|
|[SPFresh: Incremental In-Place Update for Billion-Scale Vector Search](https://dl.acm.org/doi/abs/10.1145/3600006.3613166)|SOSP 2023|针对cluster-based进行索引更新的算法，提出了两种case，以及对应case是否应该更新centroid|
|[High-Throughput Vector Similarity Search in Knowledge Graphs](https://arxiv.org/pdf/2304.01926.pdf)|SIGMOD 2023|Knowledge Graph，Hybrid Query。作者发现workloads 中混合查询的过滤条件具备一定规律性，基于此可以在partition阶段做一定优化。文章设计了了HQI的模型。|
|Fast, Approximate Vector Queries on Very Large Unstructured Datasets|NSDI 2023|利用单个向量局部几何特性构建error-latency profile for each query。|
|Tagliabue, J., Greco, C.: (Vector) Space is not the final frontier: Product search as program synthesis. In: SIGIR(2023)||||


