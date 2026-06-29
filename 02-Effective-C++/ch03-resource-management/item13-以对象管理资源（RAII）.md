# 条款 13：以对象管理资源（RAII）

## 本节讲什么

资源获取即初始化，把堆内存、文件句柄、锁等资源交给局部对象管理，出作用域自动析构释放；优先使用 `unique_ptr` / `shared_ptr` 智能指针。

## 示例

```cpp
class Lock {
    std::mutex &m;
public:
    explicit Lock(std::mutex &mu) : m(mu) { m.lock(); }
    ~Lock() { m.unlock(); }
};
```
