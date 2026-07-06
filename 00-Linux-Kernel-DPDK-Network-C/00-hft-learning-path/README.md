# 00 · HFT / 低延迟学习路线（从这里开始）

> **本目录是 `00-Linux-Kernel-DPDK-Network-C` 的导读入口。** 仓库里排在 **01-C++Primer 之前**，HFT / 数据面请 **从这里开始**。

## 你要解决什么问题

| 目标 | 为什么先学 C |
|------|----------------|
| **DPDK** 用户态收发包 | mbuf、ring、零拷贝 —— 全是 C + 内存模型 |
| **Linux 网络栈 / 内核** | 协议栈、驱动、`sk_buff` —— C + GNU 扩展 |
| **低延迟交易数据面** | 热路径忌分配、忌虚函数；C 贴近硬件、可预测 |
| **与交易所 / 网卡对接** | 二进制协议、对齐、字节序 —— C 陷阱书里全覆盖 |

C++ 留给 **策略逻辑、回测框架、配置工具**；能读能写 **数据面 C** 是 HFT 底层门槛。

## 五本书怎么走（01 → 05）

```text
01 K&R          语法、指针、结构体、malloc —— 能写正确的小程序
    ↓
02 C和指针      内存布局、ABI、动态内存 —— 能读懂内核/DPDK 结构体
    ↓
03 陷阱与缺陷   词法/链接/库函数/宏/可移植 —— 少踩静默 bug
    ↓
04 专家编程     链接器、数组≠指针、表达式 UB —— 读懂「怪代码」
    ↓
05 GNU-C 修养   __attribute__、内联汇编、段布局 —— 内核/DPDK 必读
    ↓
实战            epoll/socket → DPDK l2fwd → 内核 net/ 源码选读
```

| 阶段 | 目录 | 建议用时（参考） | 过关标准 |
|------|------|------------------|----------|
| A | [01-K-and-R-C](../01-K-and-R-C/) | 2–4 周 | 独立写多文件 C + Makefile，会用 gdb |
| B | [02-Pointers-on-C](../02-Pointers-on-C/) | 3–5 周 | 能画结构体内存图、解释指针运算 |
| C | [03-C-Traps-and-Pitfalls](../03-C-Traps-and-Pitfalls/) | 1–2 周 | 能解释链接错误、宏坑、字节序 |
| D | [04-Expert-C-Programming](../04-Expert-C-Programming/) | 2–3 周 | 能读 tdecl、理解链接与内存段 |
| E | [05-Embedded-C-Self-Cultivation](../05-Embedded-C-Self-Cultivation/) | 3–4 周 | 读懂 `__attribute__`、链接脚本片段 |

**可并行**：02 与 03 部分章节；04 的 ch05 链接可与 03 ch04 对照读。

## 环境与工具（本仓库默认）

| 工具 | 用途 |
|------|------|
| **WSL2 + Ubuntu** | 与生产 Linux 一致；本仓库 demo 在 WSL 编译 |
| **gcc/clang** `-Wall -Wextra -std=c11` | 日常编译 |
| **gdb** | 段错误、core dump |
| **make** | 各章 `demo/Makefile` |
| **nm / readelf / objdump** | 符号、段、对齐（04 专家编程） |
| **tcpdump / wireshark** | 网络实战（K&R ch8 之后） |

```bash
# 在任意 demo 目录
make clean && make all && ./main
```

## 阶段 F：出书本后的实战（提纲）

1. **Linux 网络基础**：`socket`、`bind`、`epoll`、`SO_REUSEPORT`（K&R ch8 + man pages）
2. **DPDK 入门**：官方 [Getting Started Guide](https://doc.dpdk.org/guides/linux_gsg/)，`l2fwd` / `rxtx_callbacks` 示例
3. **性能概念**：CPU 亲和、NUMA、hugepage、cache line（与 05 章内存、07 可移植对齐关联）
4. **C++ 按需**：根目录 [08-Cpp-Concurrency](../../08-Cpp-Concurrency/)、[04-Effective-Modern-C++](../../04-Effective-Modern-C++/)

## 与 C++ 主线的关系

```text
HFT 推荐：  00(本页) → 00/01–05 → 网络/DPDK 实战 → C++ 08/04 按需
通用推荐：  C++ 01–04 → 00/01–05 → 内核/DPDK
```

## 学习进度（总览）

- [ ] [00 路线通读](./README.md)（本页）
- [ ] [01 K&R](../01-K-and-R-C/)
- [ ] [02 C 和指针](../02-Pointers-on-C/)
- [ ] [03 C 陷阱与缺陷](../03-C-Traps-and-Pitfalls/)
- [ ] [04 C 专家编程](../04-Expert-C-Programming/)
- [ ] [05 嵌入式 C 修养](../05-Embedded-C-Self-Cultivation/)
- [ ] 实战：Linux 网络 + DPDK demo

## 下一步

打开 **[01-K-and-R-C/ch01-introduction](../01-K-and-R-C/ch01-introduction/)** 开始第一本书。
