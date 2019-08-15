# C语言常识

## 基本概念

> C语言主要是由贝尔电话实验室的丹尼斯·M·里奇（Dennis M.Ritchie）开发的，从1969年开始设计并于1973年开发完成。……它是一种早期的程序设计语言B语言的后继者。B是BCPL（Basic CPL）语言的一种精简版本，而BCPL来源于CPL（Combined Programming Language）。
>
> 参见[《编码》](../books/history/《编码：隐匿在计算机软硬件背后的语言》.md)396页

- 源文件拓展名 `h`, `c`

### `main()`函数

使用`int main(void){ ... }`形式的`main()`函数。

- `void main(){}` 不符合C语言标准。
- `main(){}` 不符合C99标准。
- `int main(){}` 能编译运行，但它不是标准的C语言形式。

参见[CPP Reference网站中关于main()函数的内容](http://en.cppreference.com/w/c/language/main_function)。