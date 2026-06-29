# 条款 6：不想用编译器自动生成的函数，就明确禁用

## 本节讲什么

C++11 前：声明为 `private` 且不实现；C++11 及以后：`= delete` 显式删除拷贝/赋值。

## 示例

```cpp
class NonCopyable {
public:
    NonCopyable() = default;
    NonCopyable(const NonCopyable &) = delete;
    NonCopyable &operator=(const NonCopyable &) = delete;
};
```
