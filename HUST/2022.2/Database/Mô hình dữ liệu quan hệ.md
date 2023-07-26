### Các khái niệm
- Thuộc tính (Trường): Đặc tính của đối tượng
- Miền thuộc tính: Miền giá trị của thuộc tính
- Quan hệ: Tập các n-bộ giá trị sao cho mỗi giá trị thuộc miền giá trị của thuộc tính
	- Một quan hệ có thể biểu diễn dưới dạng bảng
	- Một dòng tương ứng một bộ
	- Một cột tương ứng một thuộc tính
- Bậc của một quan hệ: Số thuộc tính của quan hệ - Số cột của bảng
- Lực lượng của một quan hệ: Số bộ của quan hệ - Số hàng
- Sơ đồ quan hệ: Là tập hữu hạn các thuộc tính
	- ![[Sơ đồ quan hệ.png]]
- Khóa: Là tập các thuộc tính mà 2 bộ bất kì của quan hệ luôn có giá trị của ít nhất 1 thuộc tính trong tập khác nhau
	- Một quan hệ có thể có nhiều khóa
	- Siêu khóa là khóa chứa khóa khác
	- Khóa tối thiểu là khóa mà mọi tập con của nó không phải khóa
	- Khóa ngoài K của quan hệ r(U) tham chiếu đến một quan hệ r' nếu K là khóa chính của r'
### Ưu điểm
- Dựa trên lý thuyết tập hợp
- Khả năng tối ưu hóa các xử lý phong phú
### Nhược điểm
- Hạn chế trong biểu diễn ngữ nghĩa
- Cấu trúc dữ liệu không linh hoạt