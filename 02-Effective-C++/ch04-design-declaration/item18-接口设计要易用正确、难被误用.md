# 条款 18：接口设计要易用正确、难被误用

## 本节讲什么

限制类型、强制构造、禁止隐式转换、限定参数合法范围，从接口层面堵错误。

## 示例

```cpp
class Date {
public:
    explicit Date(int y, int m, int d);
    static Date fromString(const std::string &);  // 工厂函数
};
```
