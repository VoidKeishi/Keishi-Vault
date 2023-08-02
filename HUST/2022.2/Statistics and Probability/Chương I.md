## Giải tích kết hợp
- Quy tắc
	- Quy tắc cộng: Một công việc nhiều trường hợp
	- Quy tắc nhân: Một công việc nhiều bước
- Giải tích kết hợp
	- Chỉnh hợp lặp: $\overline{A}^k_n=n^k$
	- Chỉnh hợp: $A^k_n=\frac{n!}{(n-k)!}$
	- Hoán vị: $P_n=n!$
	- Tổ hợp: $C^k_n=\frac{A^k_n}{k!}=\frac{n!}{k!(n-k)!}$
	- ![[Pasted image 20230730200041.png]]
## Sự kiện và các phép toán
### Một số định nghĩa
- Phép thử: Một quan sát (Dạng câu hỏi)
- Kết cục: Kết quả không thể chia nhỏ hơn được
- Không gian mẫu: Tập các kết cục
- Sự kiện: Tập con của không gian mẫu (Dạng mệnh đề)
	- Sự kiện sơ cấp: Chỉ gồm 1 kết cục
	- Sự kiện chắc chắn: Luôn xảy ra ($\Omega$)
	- Sự kiện không thể: Không xảy ra
	- Sự kiện ngẫu nhiên: Có thể xảy ra hoặc không
	- Phép thử ngẫu nhiên: Kết quả là sự kiện ngẫu nhiên
- Quan hệ giữa các sự kiện
	- Kéo theo: A => B
	- Tương đương: A <=> B
- Phép toán sự kiện
	- Tổng: C = A+B (OR)
	- Tích: C = A.B (AND)
	- Đối lập: C = $\overline{A}$ (NOT)
	- Hiệu: C = A+$\overline{B}$
	- Xung khắc: A.B = empty
- Tính chất: Giao hoán, kết hợp, phân phối, tương tác
## Các định nghĩa xác suất
- Định nghĩa chung: Xác suất của sự kiện là số nằm giữa 0 và 1, đo lường khả năng xảy ra của sự kiện khi phép thử được thực hiện
- Kí hiệu P(A)
- Tính chất cơ bản
	- $0\leq P(A)\leq 1$ 
	- $P(\Omega)=1; P(\empty)=0$ 
	- $P(A)+P(\overline{A})=1$ 
- Theo cổ điển : $P(A)=\frac{n_A}{n_\Omega}$ 
- Theo hình học : $P(A) = \frac{Độ \space miền\space A}{Độ \space miền \space \Omega}$ 
- Theo tần suất (thống kê) : $P(A)=\frac{Số \space lần\space ra \space A}{Số \space lần \space thử}$ (Với số lần thử lớn)
## Một số công thức tính xác suất
- Cộng: $P(A+B)=P(A)+P(B)-P(AB)$ 
	-  Nếu A B xung khắc 
	- ⇒ $A.B = \empty ⇒ P(A+B) = P(A) + P(B)$ 
- Xác suất có điều kiện $P(A|B)$ 
	-  $P(A|B) = \frac{P(AB)}{P(B)}$ 
- Nhân: $P(A.B) = P(A).P(B|A)=P(B).P(A|B)$ 
- Bernoulli
	- Xác suất để sự kiện A xảy ra k lần trong n phép thử
	- $p_n(k) = C^k_n.p^k.{(1-p)}^{n-k}$ 
## Công thức xác suất đầy đủ và Bayes