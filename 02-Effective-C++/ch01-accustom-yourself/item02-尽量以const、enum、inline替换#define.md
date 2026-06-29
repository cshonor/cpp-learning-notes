# 条款 2：尽量以 const、enum、inline 替换 #define

## 本节讲什么

宏没有类型检查、作用域污染、调试困难；常量用 `const`，类内常量用 `enum`，小函数用 `inline` 替代宏。
