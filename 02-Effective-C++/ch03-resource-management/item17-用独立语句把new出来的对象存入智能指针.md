# 条款 17：用独立语句把 new 出来的对象存入智能指针

## 本节讲什么

避免中间异常导致内存泄漏，不要把 `new` 直接嵌在函数传参里。

## 示例

```cpp
std::shared_ptr<Widget> pw(new Widget);
processWidget(pw, priority());  // 用独立语句，避免异常泄漏
```
