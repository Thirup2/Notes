# 前言

**计算机系统**在我看来应该分为三部分，一是**计算机硬件系统**，二是**操作系统**，三是**计算机体系结构**。

这三者之间的关系密不可分，一台计算机在这三者的协同作用下，才能进行正常的工作。以我现有的认识，我对这三者的理解暂时如下：

1. 计算机硬件系统是计算机的物理组成，其包含一些重要的组成部分：CPU、内存等，它们之间的组成方式往往决定了数据在这些硬件之间的传输速率
2. 操作系统是统筹管理硬件的一个软件，在操作系统和每个不同的硬件之间往往还需要一层接口，就是驱动程序，操作系统通过这些驱动程序管理硬件，来控制硬件的协同工作，它一般都提供了一些基础的系统管理应用，同时一般还会为软件开发者提供一层接口，来便于软件开发者开发能够使用操作系统各种功能的软件。
3. 计算机体系结构是硬件和操作系统的组织方式，一般而言决定了软件在计算机上运行的具体过程。

希望能在后续的学习中逐渐修正完善这三者的定义。

本次总结是基于《深入理解计算机系统》进行的，主要是上述三者的一个全局概览，所以在每一个具体的方面或许都不够细致，具体的总结会在后续逐步进行。



# 参考书籍

- 《深入理解计算机系统》
- 《计算机组成与设计：硬件/软件接口》（RISC-V版）
- 《计算机组成原理》
- 《现代操作系统》
