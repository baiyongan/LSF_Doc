# 3.2 LSF 细观

了解在 LSF 主机上运行的各种守护进程，LSF 集群通信路径，以及 LSF 如何容许集群中的主机故障。

- ##### LSF 守护程序和进程

  集群中的每个主机上都运行多个 LSF 进程。 正在运行的进程的类型和数量，取决于主机是主节点还是计算节点。

- ##### LSF 集群通信路径

  了解集群中 LSF daemon 之间的通信路径。

- ##### 容错和自动主控主机故障转移

  LSF 的强大体系结构在设计时考虑了容错能力。 系统中的每个组件，都有一个恢复操作。关键组件由另一个组件监视，并且可以自动从故障中恢复。

- ##### 安全性

  了解 LSF 安全模型，身份验证和用户角色。