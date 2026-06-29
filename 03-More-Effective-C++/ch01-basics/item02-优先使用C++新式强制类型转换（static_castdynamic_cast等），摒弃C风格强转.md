# 条款 2：优先使用 C++ 新式强制类型转换（static_cast/dynamic_cast 等），摒弃 C 风格强转

## 本节讲什么

> 待补充详细笔记（错误案例、原理、正确写法、代码示例）。

## 示例

```cpp
double d = 3.14;
int i = static_cast<int>(d);
// int j = (int)d;  // 避免 C 风格强转
```
