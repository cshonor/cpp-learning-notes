# 条款 6：分清前置 ++/-- 和后置 ++/-- 重载写法、性能差异

## 本节讲什么

> 待补充详细笔记（错误案例、原理、正确写法、代码示例）。

## 示例

```cpp
class Counter {
    int v_;
public:
    Counter &operator++() { ++v_; return *this; }      // 前置，少一次拷贝
    Counter operator++(int) { Counter t = *this; ++v_; return t; }
};
```
