# 条款 27：尽量减少类型转型（cast）

C 风格强转危险；优先 `static_cast` / `const_cast`，少用 `dynamic_cast` / `reinterpret_cast`；转型会破坏类型安全，重构设计规避转型。
