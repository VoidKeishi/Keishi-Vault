- Loại: Học không giám sát
- Input: Tập dữ liệu ${x_1,..,x_M}$ không có nhãn
- Output: Các cụm, nhóm của các quan sát
	- Cụm là tập các quan sát tương tự với nhau hoặc khác biệt với các quan sát của cụm khác
- Giải thuật phân cụm
	- Dựa trên phân hoạch
	- Dựa trên tích tụ phân cấp
	- Bản đồ tự tổ chức
	- Mô hình hỗn hợp
	- Deep clustering
- Đánh giá phân cụm
	- Khoảng cách giữa các cụm cần cực đại hóa
	- Khoảng cách trong một cụm cần cực tiểu hóa
- Phương pháp K-means
	- Là phương pháp dựa trên phần hoạch
	- Input: D, k, d(x,y)
	- Output: Các phân cụm
	- Thuật toán
		- Chọn ngẫu nhiên k quan sát làm điểm trung tâm khởi tạo của k cụm
		- Lặp liên tục 2 bước sau đến khi đạt điều kiện hội tụ
			- Với mỗi quan sát, gắn nó vào cụm có tâm gần nó nhất
				- Tính khoảng cách đến các tâm, tìm khoảng cách nhỏ nhất![[Pasted image 20240228125922.png]]
			- Với mỗi cụm, tính toán điểm trung tâm dựa trên tất cả các quan sát thuộc cụm đó![[Pasted image 20240228125859.png]]
		- Điều kiện hội tụ
			- Không có hoặc không đáng kể việc gán lại quan sát vào cụm khác
			- Không có hoặc không đáng kể thay đổi về điểm trung tâm các cụm
			- Giảm không đáng kể về tổng lỗi phân cụm
				- Lỗi phân cụm![[Pasted image 20240228125731.png]]
	- Ưu điểm
		- Đơn giản
		- Linh động: Dùng nhiều độ đo khác nhau
		- Hiệu quả
	- Nhược điểm
		- Số cụm k cần xác định trước (Nhưng không biết chính xác)
		- Nhạy cảm với outliers
			- Giải quyết ngoại lai
				- Quan sát một vài bước lặp phân cụm rồi quyết định loại bỏ
				- Lấy ngẫu nhiên một tập nhỏ từ D để học K cụm
		- Phụ thuộc vào các tâm khởi tạo
			- Giải quyết
				- Kết hợp các kết quả phân cụm với nhau
				- Cách chọn nên dùng
					- Chọn hạt nhân sau xa với hạt nhân gần nhất trong nhóm đã chọn -> K-means++
		- Không phù hợp để phát hiện các cụm không có dạng hình cầu
	- Online K-means
		- K-means không phù hợp với big data hoặc luồng dữ liệu liên tục
		- Online K-means cực tiểu hàm lỗi theo phương pháp leo đồi và dùng thông tin đạo hàm
		- Thuật toán
			- Khởi tạo K tâm ban đầu
			- Cập nhật tâm mỗi khi điểm dữ liệu mới đến
				- Tìm tâm gần với điểm dữ liệu mới nhất
				- Cập nhật tâm theo điểm mới đến
					- $w_{t+1}=w_{t}+{\gamma}_t(x_t-w_t)$
				- Cách chọn hệ số $\gamma$
					- Điều kiện của hệ số $\gamma$     ![[Pasted image 20240228132210.png]]
					- Hay dùng![[Pasted image 20240228132446.png]]
	- So sánh tốc độ hội tụ![[Pasted image 20240228132555.png]]
	- Coordinate descent
	- C -means
	- Hirarchical clustering