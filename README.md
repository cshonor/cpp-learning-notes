# 学习笔记目录

按推荐阅读顺序整理，笔记与代码对应根目录下各书籍子目录。

| 顺序 | 目录 | 书籍 | 侧重 |
|------|------|------|------|
| 1 | [01-C++Primer](./01-C++Primer/) | 《C++ Primer 第5版》 | 语法、标准库基础 |
| 2 | [02-Effective-C++](./02-Effective-C++/) | 《Effective C++ 第三版》 | 基础编码规范 |
| 3 | [03-More-Effective-C++](./03-More-Effective-C++/) | 《More Effective C++》 | 进阶语法、设计技巧 |
| 4 | [04-Effective-Modern-C++](./04-Effective-Modern-C++/) | 《Effective Modern C++》 | 移动语义、lambda、类型推导等现代特性 |
| 5 | [05-Effective-STL](./05-Effective-STL/) | 《Effective STL》 | STL 最佳实践 |
| 6 | [06-STL-Source-Analysis](./06-STL-Source-Analysis/) | 《STL源码剖析》 | STL 底层原理 |
| 7 | [07-Cpp-Object-Model](./07-Cpp-Object-Model/) | 《深度探索C++对象模型》 | 对象内存布局、多态底层 |
| 8 | [08-Cpp-Concurrency](./08-Cpp-Concurrency/) | 《C++并发编程实战》 | 线程、同步、内存模型 |

## 学习提示

- **经典与现代的衔接**：前序 Effective 系列打好编码基本功后，用《Effective Modern C++》集中补齐 C++11/14；不必因书偏老而跳过底层书，**原理 > 语法版本**。
- **Modern C++ 重点**：优先掌握移动语义、模板新特性、lambda、类型推导；在 `04-Effective-Modern-C++/` 写示例，理解用法与坑点即可，不必啃得特别慢。
- **对象模型**：在 `07-Cpp-Object-Model/` 打印类内存大小、成员偏移、虚表结构，直观理解底层布局。
- **并发编程**：在 `08-Cpp-Concurrency/` 动手写多线程、互斥锁、条件变量、异步代码，纯看书很难吃透。
- **全程保持**：笔记与代码都写在对应书籍目录下，方便按书复盘。
