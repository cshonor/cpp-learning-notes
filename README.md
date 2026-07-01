# 学习笔记目录

按推荐阅读顺序整理，笔记与代码对应根目录下各书籍子目录。

## C++ 主线（01–10）

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
| 9 | [09-C++17-The-Complete-Guide](./09-C++17-The-Complete-Guide/) | 《C++17 - The Complete Guide》（Josuttis） | 结构化绑定、折叠表达式、并行 STL、`string_view` 等 C++17 过渡特性 |
| 10 | [10-C++20-The-Complete-Guide](./10-C++20-The-Complete-Guide/) | 《C++20 - The Complete Guide》（Josuttis） | Concepts、Modules、Coroutines、Ranges 等 C++20 标准 |

## C 语言 · Linux 内核 / DPDK / 网络服务（11）

| 顺序 | 目录 | 说明 |
|------|------|------|
| 11 | [11-Linux-Kernel-DPDK-Network-C](./11-Linux-Kernel-DPDK-Network-C/) | 5 本 C 书（内部分 `01–05`），面向内核、DPDK、Linux 网络服务 |

详见 [11-Linux-Kernel-DPDK-Network-C/README.md](./11-Linux-Kernel-DPDK-Network-C/README.md)。

## C++ 学习顺序

1. 先吃透 **04-Effective-Modern-C++**（C++11/14/17），建立现代 C++ 基础认知
2. 完成 STL、对象模型、并发等底层章节（05–08）
3. 读 **09-C++17-The-Complete-Guide**：结构化绑定、折叠表达式、并行 STL、`string_view` 等——HFT 技术栈里 17→20 的过渡基线
4. 最后切入 **10-C++20-The-Complete-Guide**，理解 C++20 是对 C++17 的升级拓展（Concepts、Ranges、Coroutines 等）

## C 语言学习顺序

见 **11-Linux-Kernel-DPDK-Network-C**：阶段 1（01–04）→ 阶段 2（05 GNU-C）→ 内核 / DPDK / 网络源码

## 学习提示

- **C++ 经典与现代**：Effective 系列 + Modern C++ 衔接；**原理 > 语法版本**
- **C 的定位**：为 Linux 内核、DPDK、网络数据面服务；有 C++ 基础后再学 C 更高效
- **对象模型**：`07-Cpp-Object-Model/` 与 `11-.../02-Pointers-on-C/` 对照理解内存布局
- **全程保持**：笔记与代码写在对应书籍目录下，方便按书复盘

## 可选拓展（量化 / 低延迟方向）

| 目录（按需追加） | 书籍 | 侧重 |
|------------------|------|------|
| `12-Practical-C++20-Financial-Programming` | 《Practical C++20 Financial Programming》 | 金融量化 C++20 实战 |
| `13-Modern-C++-Performance-Engineering` | 《Modern C++ Performance Engineering》 | C++17/20 低延迟、无锁、CPU 优化 |
