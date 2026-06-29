# 条款 19：设计类等同于设计一种全新类型

## 本节讲什么

完整规划：创建销毁、初始化赋值、传参方式、取值范围、继承、类型转换等整套行为。

## 示例

```cpp
class BankAccount {
public:
    void deposit(double amount);  // 接口简单、难误用
    // 不暴露裸指针给外部随意修改余额
};
```
