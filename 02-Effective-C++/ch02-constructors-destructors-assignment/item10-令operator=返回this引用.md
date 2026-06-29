# 条款 10：令 operator= 返回 *this 引用

## 本节讲什么

支持连续赋值链式调用：`a = b = c`。

## 示例

```cpp
class Widget {
public:
    Widget &operator=(const Widget &rhs) {
        // ...
        return *this;
    }
};
```
