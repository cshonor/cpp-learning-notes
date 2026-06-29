# 条款 12：复制对象时勿忘其每一个成员

## 本节讲什么

自定义拷贝构造/赋值时，必须拷贝**所有成员变量 + 基类部分**，遗漏父类成员会造成切片、数据不全。

## 示例

```cpp
class String {
    char *data;
public:
    String(const String &o) : data(new char[std::strlen(o.data) + 1]) {
        std::strcpy(data, o.data);
    }
};
```
