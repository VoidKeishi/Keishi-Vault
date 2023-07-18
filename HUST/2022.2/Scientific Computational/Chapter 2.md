# Hệ phương trình tuyến tính
## Định nghĩa
$A.x=b$
Trong đó: 
	A là ma trận m x n - hệ số
	x là ma trận n x 1 - biến
	b là ma trận m x 1 - vế phải
	m là số phương trình
	n là số ẩn 
Các khả năng: 
	m = n : hệ vuông (dễ có duy nhất nghiệm)
		$x=A^{-1}b$
	m < n : hệ thiếu (dễ vô số nghiệm)
	m > n : hệ dư (dễ vô nghiệm)
Kronecker-Capelli : Dành cho mọi hệ
	$A.x=b$ có nghiệm $(=)$ $rank(A)=rank(Ab)$
Giải hệ vuông (m=n)
	$det(A)\neq0$ => nghiệm duy nhất
		Tính $A^{-1}.b$ => nghiệm duy nhất
	$det(A)=0$ => dùng Kronecker-Capelli =>có/vô nghiệm => vô số/vô nghiệm
		A suy biến => không tồn tại $A^{-1}$
	Ví dụ:
		$10x_1-7x_2=7$
		$-0.1x$


