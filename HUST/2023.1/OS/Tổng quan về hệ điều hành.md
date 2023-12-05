# Khái niệm hệ điều hành
## Cấu trúc phân lớp của hệ thống tính toán
- Các thành phần của hệ thống tính toán: 
	- Người dùng
	- Phần mềm hệ thống
	- Hệ điều hành
	- Phần cứng
- Vị trí và mục tiêu của hệ điều hành
	- Vị trí: Nằm giữa phần cứng và chương trình ứng dụng
	- Mục tiêu:
		- Chuẩn hóa giao diện người dùng
		- Sử dụng hiệu quả tài nguyên phần cứng và tối đa hiệu suất
## Chức năng
### Giả lập một máy tính ảo
- Giấu chi tiết phải thực hiện + khai thác các chức năng của phần cứng máy tính
- Đơn giản hóa việc lập trình
	- Không phải làm việc với dãy nhị phân
	- Mỗi chương trình được phân sẵn tài nguyên - từ góc nhìn của chương trình, nó được sở hữu toàn bộ bộ nhớ, thời gian CPU, thiết bị
	- Giúp giao tiếp với thiết bị dễ dàng hơn
### Quản lý tài nguyên của hệ thống
- Các chương trình đòi hỏi tài nguyên về thời gian và không gian
- Nhiệm vụ của hệ điều hành
	- Phân phối cho chương trình khi cần thiết
	- Giải quyết tranh chấp
	- Quyết định thứ tự cấp phát
# Lịch sử hệ điều hành
## 1948-1970
- Phần cứng đắt, nhân công rẻ
- Thiếu tương tác giữa người dùng và máy
- 1 người dùng tại một thời điểm
## 1970-1981
- Các máy tính có giá 10.000$, dùng được cho nhiều loại việc
- Hệ điều hành ổn định
- Cho phép nhiều người dùng tương tác tại một thời điểm
## 1981-1995
- Máy tính rẻ, nhân công đắt
- Tài nguyên phần cứng bị giới hạn
- Máy tính cá nhân mạnh dần và phổ biến
- Giao diện người dùng đồ họa
## 1995-Nay
- Thiết bị di động trở nên phổ biến
- Mạng diện rộng, mạng không dây
- Hệ thống ngang hàng
- Điện toán đám mây
# Định nghĩa và phân loại
- Định nghĩa theo các góc nhìn khác nhau
	- Người dùng
	- Người quản lý
	- Quan điểm kỹ thuật
	- Quan điểm hệ thống
- Phân loại hệ thống
	- Xử lý theo lô đơn chương trình
	- Xử lý theo lô đa chương trình
	- Phân chia thời gian
	- Xử lý thời gian thực
	- Song song
	- Phân tán
# Các khái niệm trong hệ điều hành
- Tiến trình: 
	- Là một chương trình đang thực hiện - trạng thái động của chương trình
	- Gồm: Code, data, stack, pointer, thanh ghi, thông tin cần thiết
- Luồng:
	- Là chuỗi lệnh được thực hiện trong tiến trình
	- Gồm: Code, data, stack, pointer, thanh ghi riêng
	- Một tiến trình có thể chứa nhiều luồng
- Tài nguyên hệ thống