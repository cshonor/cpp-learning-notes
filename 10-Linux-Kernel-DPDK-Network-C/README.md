# 10 · C 语言（Linux 内核 / DPDK / 网络服务）

> 学习 C 的目的：读懂并编写 **Linux 内核**、**DPDK**、**Linux 网络服务** 相关代码。共 5 本，内部分为 `01–05`。

## 为什么学 C

- Linux 内核、内核模块、网络协议栈以 C + GNU 扩展为主
- DPDK、高性能网卡旁路、用户态网络栈依赖 C 与底层内存模型
- 与 C++ 主线（01–09）配合：C++ 做业务与框架，C 啃内核与数据面

## 书单

| 阶段 | 目录 | 书籍 | 侧重 |
|------|------|------|------|
| 1 | [01-K-and-R-C](./01-K-and-R-C/) | 《C 程序设计语言（K&R 第2版）》 | 标准 C、`malloc`/指针/结构体 |
| 1 | [02-Pointers-on-C](./02-Pointers-on-C/) | 《C 和指针》 | 内存布局、联合体、ABI（读内核结构体基础） |
| 1 | [03-C-Traps-and-Pitfalls](./03-C-Traps-and-Pitfalls/) | 《C 陷阱与缺陷（第2版）》 | 宏、链接、库函数等常见陷阱 |
| 1 | [04-Expert-C-Programming](./04-Expert-C-Programming/) | 《C 专家编程》 | 链接器、深层指针规则、C 设计内幕 |
| 2 | [05-Embedded-C-Self-Cultivation](./05-Embedded-C-Self-Cultivation/) | 《嵌入式 C 语言自我修养》 | GNU-C 扩展（`__attribute__`、零长数组等），内核/DPDK 必读 |

## 学习顺序

1. **阶段 1**（C++ 思维 → 纯 C）：**01 → 02 → 03 → 04**
2. **阶段 2**（GNU-C / 内核 / DPDK）：**05** → 再读 LKD、虚拟内存、内核网络源码

## 学习进度

- [ ] 01 K&R
- [ ] 02 C 和指针
- [ ] 03 C 陷阱与缺陷
- [ ] 04 C 专家编程
- [ ] 05 嵌入式 C 语言自我修养
