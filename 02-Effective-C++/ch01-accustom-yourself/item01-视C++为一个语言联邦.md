# 条款 1：视 C++ 为一个语言联邦

## 本节讲什么

C++ 由 4 个子集构成：C 语言、面向对象 C++、模板 C++、STL；不同场景编码规则不一样，不能一概而论。

## 示例

```cpp
// C 子集：数组与指针
char buf[] = "hello";
// OOP：类与封装
class Widget { public: void draw() {} };
// 模板 + STL
#include <vector>
std::vector<int> v{1, 2, 3};
```
