# 条款 5：警惕编译器隐式类型转换函数带来的意外调用

## 本节讲什么

> 待补充详细笔记（错误案例、原理、正确写法、代码示例）。

## 示例

```cpp
class Fraction {
public:
    explicit Fraction(int n) : num_(n) {}
    // Fraction(int) 作为转换函数时要谨慎
private:
    int num_;
};
```
