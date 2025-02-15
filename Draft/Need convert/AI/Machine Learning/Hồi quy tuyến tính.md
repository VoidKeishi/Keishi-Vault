- Loại: Học có giám sát -> Bài toán hồi quy
- Nhiệm vụ (T): Dự đoán kết quả thuộc miền liên tục dựa trên 1 hay nhiều thuộc tính đầu vào
- Kinh nghiệm (E)
	- Tập dữ liệu $D={(x_1,y_1),(x_2,y_2),...,(x_M,y_M)}$ 
	- $x_i=(x_{i1},x_{i2},...,x_{in})^T$ là quan sát được biểu diễn bằng vector n chiều, mỗi chiều biểu diễn một thuộc tính
	- $y_i$ là đầu ra tương ứng (mẫu)
- Biểu diễn mô hình : $f(x)=w_0+w_1x_1+...+w_nx_n$
	- $w_{0}$ tạo sự phong phú cho hàm tuyến tính (Không nhất thiết đi qua gốc tọa độ)
	- Mô hình là cách biểu diễn giả thuyết dưới dạng toán học (giả thuyết dữ liệu tuân theo quy luật tuyến tính)
- Việc học hàm hồi quy tuyến tính tương đương với việc học vector trọng số $w=(w_0,w_1,...,w_n)^T$ với mục tiêu phán đoán tương lai tốt nhất $f(x){\approx}y$ với $x$ ngoài E
- Phép đánh giá (P)
	- Hàm loss E
		- Với mỗi quan sát x: $r(x)=[c_x-f(x)]^2$
			- Sai khác luôn dương
			- Đơn giản hóa quá trình optimize (Dễ tính toán đạo hàm)
		- Với toàn bộ không gian: $E=E_x[r(x)]=E_x[c_x-f(x)]^2$
		- Mục tiêu là tìm hàm $f^*$ mà E nhỏ nhất với toàn bộ không gian, tuy nhiên thực tế không thể tính được cho toàn bộ -> Tính lỗi thực nghiệm và cực tiểu hóa nó
			- $f^*=argmin_{f{\in}H}E_x[r(x)]$
			- H là không gian hàm $f$
		- Lỗi thực nghiệm là trung bình lỗi trên tập D (dữ liệu huấn luyện)
	- Hàm lỗi thực nghiệm
		- Là xấp xỉ của hàm lỗi trên D![[Pasted image 20240227220220.png]]
		- Lỗi tổng quát hóa                           ![[Pasted image 20240227220344.png]]
			- Lấy trung bình để tiện so sánh kể cả khi M thay đổi + tránh tràn số
- Bình phương tối thiểu (Ordinary Least Square)
	- Tìm $w^*$ để RSS nhỏ nhất bằng cách giải phương trình RSS' = 0
	- Thuật toán
		- Input: D
		- Output: $w^*$
		- Tính ![[Pasted image 20240227220935.png]]
	- Nhược điểm
		- Có thể không tồn tại nghịch đảo
		- Độ phức tạp tính toán lớn (m hàng * n cột, tính nghịch đảo, nhân ma trận)
		- Khả năng overfitting cao
- Hồi quy Ridge
	- Thêm đại lượng hiệu chỉnh để tránh overfitting = Giảm độ phức tạp của mô hình![[Pasted image 20240227223601.png]]
	- $\lambda$ quá nhỏ -> OLS, overfitting
	- $\lambda$ quá lớn -> underfitting
	- Thuật toán
		- Input: D & $\lambda$
		- Output: $w*$
		- Giải phương trình RSS' = 0 ![[Pasted image 20240228103657.png]]
	- So với OLS
		- Đảm bảo luôn có nghiệm
		- Giảm overfitting tradeoff với việc lỗi trên tập học nhiều hơn
- Lasso
	- Thay thế chuẩn L2 = chuẩn L1 từ hồi quy Ridge![[Pasted image 20240228101341.png]]
	- Là hồi quy để lựa chọn đặc trưng
		- Thường tạo nghiệm thưa -> thành phần của w mang giá trị 0 -> Không phải đặc trưng quan trọng
- So sánh![[Pasted image 20240228104735.png]]