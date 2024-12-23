---
tags:
  - programming_language
  - mobile_development
type: pernament
time created: 29-10-2024
last modified: 29-10-2024
---
# [[Kotlin basic]]
- Toán tử
- Kiểu dữ liệu
- Biến
- Lệnh rẽ nhánh
- List và array
- Null safety
# [[Kotlin functions]]
- Hầu hết mọi thứ đều mang giá trị
- Function
	- Kiểu trả về Unit (giống void)
	- Arguments
		- Default: gán sẵn giá trị mặc định
		- Required: yêu cầu kiểu dữ liệu
		- Named: chỉ định tên biến truyền vào, khi truyền có thể thay đổi thứ tự
- Lambdas: giống arrow function
- Higher-order function: truyền hàm vào hàm hoặc hàm trả ra hàm
	- Last parameter call stack: nên để hàm là tham số xuống cuối
- List filters: myList.filter {condition}
	- Eager filter: luôn lọc (mặc định)
	- Lazy filter: chỉ lọc khi cần trong runtime
		- Sử dụng asSequence() để dùng lazy filter, có thể biến thành list lại bằng toList()
# [[Kotlin classes]]
- Định nghĩa lớp
- Constructor
- getter/setter mặc định có sẵn và có thể override
- Kế thừa: đơn kế thừa
	- Dùng open để cho phép kế thừa, override
	- Dùng abstract để tạo lớp trừu tượng
- Interface: class a() : interface
- 
