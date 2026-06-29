# 条款 4：确定对象被使用前已先被初始化

## 本节讲什么

内置类型手动初始化；成员变量走**初始化列表**而非构造函数内赋值；跨编译单元全局变量初始化顺序不确定，用局部静态变量懒加载规避。

## 示例

```cpp
class PhoneNumber { /* ... */ };
class Person {
    std::string name;
    PhoneNumber phone;  // 成员自动默认构造，优于裸指针
public:
    Person() : name(""), phone() {}
};
```
