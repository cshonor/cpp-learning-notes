# 条款 9：绝不在构造和析构过程调用虚函数

## 本节讲什么

构造派生类时基类构造阶段，虚函数只会走基类版本；析构同理，此时派生部分已经销毁，动态绑定失效。

## 示例

```cpp
class Base {
public:
    Base() { log(); }  // 不要：调用 virtual log()
    virtual void log() { std::cout << "Base\n"; }
};
```
