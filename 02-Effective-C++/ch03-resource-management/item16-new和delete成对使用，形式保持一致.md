# 条款 16：new 和 delete 成对使用，形式保持一致

## 本节讲什么

`new[]` 必须搭配 `delete[]`，普通 `new` 搭配普通 `delete`，混用直接未定义行为。

## 示例

```cpp
std::unique_ptr<int> p(new int(42));  // 好
// std::shared_ptr<int> sp(new int(42), new int(43));  // 坏：两条 new
```
