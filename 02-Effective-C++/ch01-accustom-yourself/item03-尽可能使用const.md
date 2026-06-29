# 条款 3：尽可能使用 const

## 本节讲什么

修饰变量、指针、函数参数、成员函数；`const` 可以限定只读语义，编译器帮你校验错误，成员函数 `const` 保证不修改对象。

## 示例

```cpp
class TextBlock {
public:
    char operator[](std::size_t pos) const { return text[pos]; }
    char &operator[](std::size_t pos) { return text[pos]; }
private:
    std::string text;
};
```
