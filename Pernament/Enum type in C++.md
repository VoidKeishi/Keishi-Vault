---
tags:
  - cpp
type: pernament
time created: 19-08-2024
last modified: 19-08-2024
---
- Là kiểu dữ liệu người dùng tự định nghĩa, giới hạn những giá trị có thể gán
```cpp
enum color{
	red,
	green,
	blue
};
color rgb1 = red
```
- Mỗi giá trị trong kiểu enum có index bắt đầu từ 0, có thể được định nghĩa lại
```cpp
enum first_enum{
	value1=1, 
	value2=10, 
	value3 //after index 10 is 11
};

first_enum e;
e=value3;
cout<<e;
```
- **Output:** 11
