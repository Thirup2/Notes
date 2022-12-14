# 一. [思维导图](https://isdhtn0nft.feishu.cn/mindnotes/bmncnMYlWGVErhYCr2G5GSAmh8b#mindmap)

# 二. 前言
## 1. 写作目的
学完C语言之后，大部分的语法已经基本会用了，但是学习时对于各个C标准之间的不同并未太过在意，这也导致了一些问题，比如看似大部分语法都会用了，但是其实大脑里的知识却是乱糟糟的，这一点在我开始学习C++之后就越发的明显。在学了一段时间C++之后，我发现自己对二者之间的区别已经变得模糊了，比如把C++的特性用在C程序中，导致一些错误；在C++程序中却大量使用C语言，导致编写的还是一个C程序。这一点让我觉得实在是爽快不起来，于是我便停下了C++的学习，决定先把已经学过的C语言总结一遍，以构建知识体系。

## 2. C语言标准
K&R C、ANSI C（C89、C90、ISO C、ANSI/ISO C）、C99、C11四个版本的C标准都将进行总结
其中以使用最广的ANSI C为默认版本，即总结中所有正常段落即为ANSI C标准，而其余三个标准采用引用标注的方法进行标注
其中K&R C并非官方版本，但也将其列出，仅进行了解

## 3. 一些概念
1. 由编译器定义的：由编译器设计者决定采取何种行动，并做好文档记录
2. 未确定的：在某些正确情况下的做法，标准并未明确规定应该怎样做。例如，参数求值的顺序
3. 未定义的：在某些不正确情况下的做法，但标准并未规定应该怎样做
4. 约束条件：这是一个必须遵守的限制或要求。如果不遵守，那么你的程序的行为就会编程上面所说的属于“未定义的”。

## 4. 参考书籍
- 《C Primer Plus 中文版》（第6版）
- 《C和指针》
- 《C专家编程》
- 《C陷阱与缺陷》

## 5. 读后感
突发奇想在这里添加了一栏读后感，当然，并非是这个总结的读后感，那也太羞耻了。所以，当然，是参考书籍的读后感。
### 1) 《C Primer Plus》
作为自学者，这本书确实是当之无愧的第一本书。虽然其中的内容互相有些交错在一起，读者很难形成对于一门编程语言的体系，但对于初学者来说，对于编程语言这类东西来说，最重要的不是一开始就构建体系，而是学会用，连使用都不会，谈何构建体系。而这本书的内容循序渐进，很好地让人学会了使用C语言来编程。书中对于初学者最容易碰到的问题基本上都有提到，可以说是很好地提醒着读者。另外，每一章后面的习题质量也都不错，除了一些与前面正文内容相关的题需要翻来翻去感到有些麻烦以外，没什么不满。
中文版的翻译也挺好的，读起来除了小部分段落，都能够很好的理解，当然也可能是我的实力问题。
最后就是整本书的格式，就一个字：清晰明了。

### 2) 《C和指针》
在作者自己的介绍里，这本书介于初学与非初学之间，而我认为它更应该归类在非初学这一类。
书的目录结构很整齐，很适合用来构建体系，我也确实主要是用的这一本书来写的总结。
整本书从第一章的代码开始就在劝退初学者了，毕竟上来就看不懂，谁还会继续看下去。但是对于已经有一点C语言基础的人来说，这本书就是宝藏了。整本书的主要内容也是以读者对C语言有了解的前提下进行的。
书里有些句子不是很好，或许是翻译的问题，总是要读好几遍才能读明白，在学上一本书的时候，遇到这类段落我都是直接放弃。好在，这次我一边做着总结，一边读着书，总是要把书里的内容看懂了才好写在总结里。于是我发现，这本书在细节的地方一点不缺，我碰到过的基本上所有的问题都在这里找到了答案，是真正从原理上来说的答案。
章节末尾的习题有些比较复杂，而且也只有部分有答案，这一点说实话不是很好，虽然强迫读者自己思考，但无论如何都完成不了的时候，答案也是学习的方法。
另外就是书的格式，读完了上一本书再来读这一本实在是感觉格式看不下去，书的格式还有作者的代码风格实在是跟我有很大出入，当然并不是说作者的风格不好，只是不太适合我而已。耐着性子看完了还是收获很大。
再就是这本书的缺点，内容来说确实无可挑剔，但是内容的老是有些小错误，特别是到了后面几章，有些函数原型返回类型都不对，不知道是作者的原因还是翻译的原因。
总的来说，瑕不掩瑜，值得一看。