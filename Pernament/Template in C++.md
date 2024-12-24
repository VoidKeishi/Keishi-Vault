---
tags:
  - cpp
  - programming_concept
type: pernament
time created: 20-08-2024
last modified: 20-08-2024
---
- Là tính năng cho phép hàm và lớp hoạt động với nhiều kiểu dữ liệu khác nhau, bằng cách quy định logic với kiểu dữ liệu giả định T
- Ví dụ hàm tính tổng
```cpp
template <typename T>
T add(T a, T b) {
    return a + b;
}

int main() {
    int intResult = add(3, 4);           // Works with integers
    double doubleResult = add(3.5, 2.5); // Works with doubles
    return 0;
}
```
- Ví dụ lớp Container
```cpp
template <typename T>
class Container {
private:
    T element;
public:
    Container(T arg) : element(arg) {}
    T getElement() {
        return element;
    }
};

int main() {
    Container<int> intContainer(42);            // Integers
    Container<string> stringContainer("Hello"); // Strings
    return 0;
}
```