# 学习笔记目录

按推荐阅读顺序整理，笔记与代码对应根目录下各书籍子目录。

## C++ 主线

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
| 9 | [09-C++20-The-Complete-Guide](./09-C++20-The-Complete-Guide/) | 《C++20 - The Complete Guide》（Josuttis） | Concepts、Modules、Coroutines、Ranges 等 C++20 标准 |

## C 语言（内核 / 底层前置）

全部 5 本书在 **[C/](./C/)** 目录下：

| 目录 | 说明 |
|------|------|
| [C/](./C/) | K&R、《C 和指针》、陷阱与缺陷、专家编程、嵌入式 C 自我修养 |

详见 [C/README.md](./C/README.md)。

## C++ 学习顺序

1. 先吃透 **04-Effective-Modern-C++**（C++11/14/17），建立现代 C++ 基础认知
2. 完成 STL、对象模型、并发等底层章节（05–08）
3. 最后切入 **09-C++20-The-Complete-Guide**，理解 C++20 是对现代 C++ 的升级拓展

## C 语言学习顺序

见 [C/README.md](./C/README.md)：阶段 1（10–13）→ 阶段 2（14 GNU-C）

## 学习提示

- **C++ 经典与现代**：Effective 系列 + Modern C++ 衔接；**原理 > 语法版本**
- **C 与 C++**：先有一定 C++ 基础再切 C 更高效；C 书在 `C/` 目录，服务内核/DPDK 路线
- **对象模型**：`07-Cpp-Object-Model/` 与 `C/11-Pointers-on-C/` 对照理解内存布局
- **全程保持**：笔记与代码写在对应书籍目录下，方便按书复盘

## 可选拓展（量化 / 低延迟方向）

| 目录（按需追加） | 书籍 | 侧重 |
|------------------|------|------|
| `15-Practical-C++20-Financial-Programming` | 《Practical C++20 Financial Programming》 | 金融量化 C++20 实战 |
| `16-Modern-C++-Performance-Engineering` | 《Modern C++ Performance Engineering》 | C++17/20 低延迟、无锁、CPU 优化 |
