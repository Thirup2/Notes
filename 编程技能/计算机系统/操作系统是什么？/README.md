# 前言
可以说，操作系统经历了这么多年的演变，成了现在我们看到的层层包裹的系统，导致学习起来非常的费力。为了理清这个结构，于是写了这一篇总结。文中的内容基本上是我自己的理解，并非权威的内容，所以肯定有许许多多的错误，毕竟在写这篇文章的时候，我连一本操作系统的书都还没有看。文章的结构将从最底层的硬件说起，直到现在用户使用的操作系统。

# 一. 硬件
硬件是硬件设计者设计的，它的设计方法与这篇文章关系不大。每个硬件都可以一些具体的工作，如显卡可以将信息显示在屏幕上；网卡可以实现电脑的联网；声卡可以让电脑发出声音等等……

可是不同的硬件的往往其中的信息是不同的，如何才能操纵硬件实现用户想让它实现的功能呢？这个答案就是驱动程序。

# 二. 驱动程序
驱动程序的具体实现暂时不管。通过驱动程序就可以操控硬件实现一些功能。

假设现在还没有操作系统，我们日常使用的软件就是通过调用不同的驱动程序来实现调用硬件完成功能的。

可是几乎每个不同的硬件都有不同的驱动程序，如果一个软件想要兼容所有人的电脑，那这个软件就得针对每一个硬件的驱动程序编写不同的实现方法，或者驱动程序来匹配不同的应用程序，这个工作量毫无疑问是巨大的。

而解决这个问题的方法就是引入操作系统。

![软件适应每个驱动程序](https://user-images.githubusercontent.com/91216205/185748847-1e6175f8-f91e-4b1e-b0ea-b72de33a43dd.png)![驱动程序适应每个软件](https://user-images.githubusercontent.com/91216205/185748862-cb7bd146-daeb-4698-8bf5-a4beef6e453e.png)

# 三. 内核
操作系统的内核就是用来管理驱动程序及硬件的一个程序。内核首先向硬件开发商提供接口，通过一个统一的接口，硬件开发商只需要根据操作系统内核的不同来编写不同的驱动程序，而现在市面上的操作系统也没有几个，工作量可以说并不大。现在内核就成了操作驱动程序的中转站。

可是这还不够，对于软件制作者来说，还是需要通过内核操作不同的驱动程序，除了多了一层中介，实际的工作量并没有减轻多少。
于是就有了操作系统的出现。

# 四. 操作系统
操作系统将硬件驱动程序的接口抽象成了一个个的函数接口。这样就可以成功给软件制作者提供一个长期保持一致的系统接口，对于一个软件，他只需要对不同的操作系统提供不同版本的软件就行了。

![操作系统](https://user-images.githubusercontent.com/91216205/185748887-432136c8-de3a-42f2-9cce-38404102075c.png)

# 总结
通过操作系统，简化了驱动程序编写者或者应用软件编写者的工作。

现在所说的操作系统一般包括驱动程序在内，还有内核和提供给软件的编程接口。由于驱动程序是需要嵌入到操作系统里面，这就要求驱动程序的开发人员不仅需要熟悉手头硬件的工作原理，更重要的是它们要确保它们写的驱动能够嵌入到操作系统里面去。