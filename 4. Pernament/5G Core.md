#networking/5g/core 
#casestudy
# Tổng quan mạng 5G 
- [[AMF]]
- Mạng thế hệ thứ 5, tốc độ nhanh hơn, độ trễ thấp hơn, khả năng chịu tải nhiều thiết bị cùng lúc hơn so với 4G
	- ![[Pasted image 20250331154446.png]]
- Dịch vụ sử dụng mạng 5G chia thành 3 nhóm chính
	- Enhanced Mobile Broadband (eMBB): Đáp ứng dịch vụ yêu cầu băng thông cao - video HD, VR, AR
	- Massive Machine Type Communication (mMTC): Tập trung vào xử lý số lượng lớn kết nối
	- Ultra-Reliable and Low-latency Communication (uRLLC): Tập trung vào độ trễ thấp như xe tự lái hay điều khiển từ xa
# Mô hình kiến trúc 5GS 3GPP Rel 16
- Kiến trúc theo chuẩn Rel 16 được định nghĩa bởi tổ chức 3GPP, thiết kế theo dạng module - [[SBA]] 
- Tách biệt [[UP]] và [[CP]], giúp triển khai linh hoạt các ứng dụng [[Edge computing]]
	- Vì [[UPF]] có thể đặt gần [[UE]] để giảm độ trễ, trong khi [[CP]] có thể đặt ở data center để tính toán tập trung
- Thiết kế tách biệt các chức năng thành các [[NF]] độc lập, 1 nghiệp vụ chỉ nằm trên 1 phần tử mạng
- Thiết kế lại toàn bộ mô hình kết nối báo hiệu nội bộ [[5G Core]], sử dụng duy nhất giao thức [[HTTPS]]
- Mô hình kiến trúc mạng có thể thể được biểu diễn theo 2 cách:
	- Reference Point Representation: Chỉ ra tên cụ thể của interface kết nối giữa các [[NF]]. Cách này chủ yếu dùng để biểu diễn với các mạng trước 5G
	- Service Based Representation: Các chức năng mạng được biểu diễn dưới dạng dịch vụ, giao tiếp với nhau thông qua API. Mỗi NF cung cấp dịch vụ mà các NF khác có thể cùng truy cập, thay vì kết nối điểm điểm. Cách biểu diễn này cũng bao gồm cả biểu diễn điểm điểm nếu có giao diện không hỗ trợ [[SBI]]
## [[SBI]]
- Các chức năng mạng giao tiếp với nhau thông qua [[SBI]]
## [[NF]]
- Tập các chức năng mạng dưới dạng dịch vụ trong 5G: [[NSSF]], [[NEF]], [[NRF]], [[PCF]], [[CHF]], [[UDM]], [[AF]], [[NSSAF]], [[AUSF]], [[AMF]], [[SMF]], [[SMSF]], [[SCP]], [[UDF]]