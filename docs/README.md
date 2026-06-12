# 学习笔记目录

按阅读顺序整理，笔记对应 `docs/` 下各子目录。

| 顺序 | 目录 | 书籍 | 侧重 |
|------|------|------|------|
| 1 | [01-C++Primer](./01-C++Primer/) | 《C++ Primer 第5版》 | 语法、标准库基础 |
| 2 | [02-Effective-C++](./02-Effective-C++/) | 《Effective C++ 第三版》 | 基础编码规范 |
| 3 | [03-More-Effective-C++](./03-More-Effective-C++/) | 《More Effective C++》 | 进阶语法、设计技巧 |
| 4 | [04-Effective-STL](./04-Effective-STL/) | 《Effective STL》 | STL 最佳实践 |
| 5 | [05-STL-Source-Analysis](./05-STL-Source-Analysis/) | 《STL源码剖析》 | STL 底层原理 |
| 6 | [06-Cpp-Object-Model](./06-Cpp-Object-Model/) | 《深度探索C++对象模型》 | 对象内存布局、多态底层 |
| 7 | [07-Cpp-Concurrency](./07-Cpp-Concurrency/) | 《C++并发编程实战》 | 线程、同步、内存模型 |

## 学习提示

- **对象模型**：结合 `code/object-model-demo/` 打印类内存大小、成员偏移、虚表结构，直观理解底层布局。
- **并发编程**：在 `code/concurrency-demo/` 动手写多线程、互斥锁、条件变量、异步代码，纯看书很难吃透。
- **全程保持**：看书 → `docs/` 记笔记，写代码 → `code/`，综合练习 → `exercises/`。
