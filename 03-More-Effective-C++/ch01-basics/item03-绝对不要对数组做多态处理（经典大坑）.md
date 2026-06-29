# 条款 3：绝对不要对数组做多态处理（经典大坑）

## 本节讲什么

> 待补充详细笔记（错误案例、原理、正确写法、代码示例）。

## 示例

```cpp
class Base { public: virtual ~Base() = default; };
class Derived : public Base {};
// Base arr[10]; arr[1] = Derived();  // 危险：不要对数组做多态
```
