下面这条预处理指令用于移除一个宏定义：
```c
#undef name
```
如果一个现存的名字需要被重新定义，那么首先必须用`#undef`移除它的旧定义