# 条款 14：资源管理类谨慎设计拷贝行为

## 本节讲什么

资源不能拷贝：禁用拷贝；资源可以共享：引用计数（`shared_ptr`）；资源深度拷贝：完整复刻一份新资源。

## 示例

```cpp
class Handle {
    std::shared_ptr<Resource> res;
public:
    Handle(const Handle &) = default;  // 或禁止拷贝
    Resource *get() const { return res.get(); }
};
```
