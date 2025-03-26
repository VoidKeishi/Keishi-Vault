#data_format 
- Viết tắt của JavaScript Object Notation, ban đầu được tạo ra theo [[JavaScript]]
- Dùng để mã hóa data và ghi file config
- Ưu điểm: 
	- Dễ đọc, ngắn gọn và cú pháp đơn giản hơn [[XML]]
	- Schema support: Dữ liệu có cấu trúc, ràng buộc, quy tắc
	- Truyền dữ liệu nhanh và dễ dàng
- Nhược điểm
	- Không có xử lý lỗi nếu hệ thống không handle
	- Có thể không hỗ trợ cấu hình phức tạp
- Syntax: 
```json
{
    "Employees": [
    {
            "name": "John Doe",
            "department": "Engineering",
            "country": "USA"
        },

        {
            "name": "Kate Kateson",
            "department": "IT support",
            "country": "United Kingdom"
        }
    ]
}
```