#machine_learning/model_evaluation/bias_variance
- Bias: Độ chệch khỏi ground truth của dự đoán - Giả thuyết dữ liệu tuân theo một quy luật là sai
- Variance: Mức độ dao động - high sensitivity to variations in training data
- BIểu hiện
	- High bias: Độ chệch lớn, train set error -> Underfitting, mô hình quá đơn giản
	- High variance: Mức độ dao động lớn, dev set error -> Có thể là overfitting, thiếu sự tổng quát
- Sự đánh đổi giữa bias và variance![[Pasted image 20240421161645.png]]
	- f^ là hàm mô hình học được từ D
	- f là quy luật thực tế (dự đoán khi biết f(x) vẫn tồn tại lỗi từ nhiễu là irreduciable error)