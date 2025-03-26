#cpp/class/enum
- Enum class là lớp đặc biệt, các đối tượng thuộc lớp này sẽ nhận 1 danh sách các giá trị được định nghĩa trong lớp
```cpp
enum class Color:char { 
	Red, 
	Green, 
	Blue 
};
```
- Ưu điểm so với [[Enum type in C++]]
	- Các giá trị enum được định nghĩa trong phạm vi lớp, không ảnh hưởng đến namespace toàn cục -> Tránh xung đột tên
	- An toàn: Giá trị trong các Enum class không thể chuyển đổi ngầm định sang nhau hay sang int
	- Chỉ định được kiểu cơ sở (ví dụ char) để kiểm soát kích thước biến, tương tác với mã yêu cầu kiểu cụ thể
