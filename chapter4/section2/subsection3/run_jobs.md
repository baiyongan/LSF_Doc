# 运行作业

使用 **bsub** 和 **lsrun** 命令通过 LSF 运行作业。 使用 **bjobs** 命令查看您的作业状态。 使用 **bstop**，**bresume** 和 **bkill** 命令控制作业执行。

## 使用 bsub 和 lsrun 运行 LSF 作业

使用两个基本命令通过 LSF 运行作业：

- **bsub** 将作业提交给 LSF 批处理调度程序。 LSF 根据您在 LSF 队列中配置的调度策略，将作业调度并调度到最佳可用主机。
- **lsrun** 命令根据 lim 守护程序，收集的当前系统负载信息在最佳主机上运行交互式任务。

对于大多数作业，您需要做的就是在通常使用的作业命令之前添加 **lsrun** 或 **bsub** 命令。 通常，您不需要修改可执行应用程序或执行脚本。

- ##### 使用bsub提交批处理作业

  **bsub** 命令将作业提交到 LSF 批处理调度队列。

- ##### 通过bjobs显示工作状态

  使用 **bjobs** 命令查看作业 ID 和有关您的作业的其他信息。

- ##### 使用 bstop，bresume 和 bkill 控制作业执行

  使用 LSF 命令来暂停（**bstop**），恢复（**bresume**）和杀死（**bkill**）作业。

- ##### 使用 lsrun 和 lsgrun 运行交互式任务

  如果可以找到所需的资源和适当的主机类型，则 **lsrun** 命令可以在当前本地主机或最佳可用主机上远程运行任务。 **lsgrun** 命令与 **lsrun** 命令类似，但是它在一组主机上运行任务。

- ##### 将您的应用程序与LSF集成

  通过将应用程序与 LSF 集成，可以确保用户可以使用正确而完整的作业提交选项来提交和运行其作业，而无需使他们学习 LSF 命令。