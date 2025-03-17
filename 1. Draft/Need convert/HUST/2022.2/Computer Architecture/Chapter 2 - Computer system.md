- Main slides: 14,17,20,22,25,30,32
# CPU
- CU: đơn vị điều khiển
- ALU: đơn vị số học và logic
- RF: tập thanh ghi
- PC: bộ đếm chương trình
# Bộ nhớ
- Cache
	- L1,L2,L3
- Bộ nhớ chính
	- Chia theo byte nhớ
- Lưu trữ ngoài
# I/O
- ![[Pasted image 20230810142845.png]]
# Hoạt động cơ bản của máy tính
## Thực hiện
- Gồm nhận lệnh và thực hiện lệnh
- Dừng nếu
	- Lệnh lỗi
	- Gặp lệnh dừng
	- Tắt máy
## Ngắt
- 2 nguyên nhân ngắt
	- Biệt lệ - Exception: Lỗi khi thực hiện
	- Ngắt từ bên ngoài - External Interrupt: Do I/O gửi tín hiệu ngắt
- Xử lý ngắt tuần tự
	- Chỉ thực hiện một ngắt một lúc
- Xử lý ngắt ưu tiên
	- Các ngắt được định nghĩa mức ưu tiên
	- Có thể ngắt lồng nhau
## Vào ra
- 2 kiểu hoạt động
	- CPU trao đổi với I/O bởi lệnh trong chương trình
	- CPU cấp quyền cho I/O truy cập bộ nhớ chính
- Bus
	- Địa chỉ
	- Dữ liệu
	- Điều khiển
- Độ rộng bus: Số đường dây của bus có thể truyền các thông tin đồng thời (ko dùng cho bus điều khiển)
- Bus địa chỉ: Độ rộng 32 bit $2^{32}$ bytes nhớ = 4GB
