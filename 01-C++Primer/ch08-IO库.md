# 第 8 章 IO 库

C++ 通过标准库中的一族类处理输入和输出。本章介绍如何读写设备（控制台、命名文件）以及内存中的 `string` 对象。

## IO 类体系

| 头文件 | 用途 |
|--------|------|
| `iostream` | 读写控制台流（`cin`、`cout`、`cerr`） |
| `fstream` | 读写命名文件 |
| `sstream` | 读写内存中的 `string` 对象 |

继承机制使得 `fstream` 或 `sstream` 可替代接受 `iostream` 引用参数的地方。

## 管理条件状态

- 每个 IO 对象维护一组状态标志（有效、文件尾、错误等）
- `rdstate`、`setstate`、`clear` 等：检测和复位流状态

## 文件输入输出

- `ifstream`、`ofstream`、`fstream` 结合 `open`、`close` 处理文件关联
- **文件模式（File Mode）**：
  - `in`：读
  - `out`：写
  - `app`：追加
  - `trunc`：截断

## string 流

- **`istringstream`**：从 `string` 读取数据（逐行读取后按单词分解）
- **`ostringstream`**：向 `string` 写入数据（逐步构造格式化输出后一次性打印）
