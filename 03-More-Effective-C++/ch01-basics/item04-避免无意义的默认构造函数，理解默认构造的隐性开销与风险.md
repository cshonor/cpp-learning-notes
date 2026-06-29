# 条款 4：避免无意义的默认构造函数，理解默认构造的隐性开销与风险

## 本节讲什么

> 待补充详细笔记（错误案例、原理、正确写法、代码示例）。

## 示例

```cpp
class NoDefault {
    int id;
public:
    explicit NoDefault(int i) : id(i) {}  // 无意义默认构造时显式要求参数
};
```
