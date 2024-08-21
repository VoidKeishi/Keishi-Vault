## Biến ngẫu nhiên và hàm phân phối xác suất
### Định nghĩa
- Biến ngẫu nhiên: Biến có giá trị ngẫu nhiên tùy thuộc vào phép thử
- Phân loại
	- Biến ngẫu nhiên rời rạc: Tập giá trị hữu hạn hoặc vô hạn đếm được
	- Biến ngẫu nhiên liên tục: Tập giá trị lấp kín một khoảng trục số hoặc cả trục số
- Hàm phân phối xác suất: $F(x) = P(X<x), x \in R$
	- Tổng xác suất nhận được các giá trị bên trái điểm x
	- Tính chất
		- $0 \leq F(x) \leq 1$ 
		- $\lim_{x\to{-\infty}}F(x) = 0 ; \space  \lim_{x\to{+\infty}}F(x) =1$ 
		- F(x) là hàm không giảm : $\forall a<b, F(a) \leq F(b)$ 
		- $P(a \leq X < b) = F(b)- F(a)$ 
- Bảng phân phối xác suất
	- Ghi giá trị mà X nhận được kèm xác suất nhận giá trị đó
### Tham số đặc trưng
- Kỳ vọng: Giá trị trung bình
	- $E(X) = \Sigma x_i.p_i$ 
- Phương sai: Mức độ phân tán dữ liệu
	- $V(X) = E{(X-EX)}^2=E(X^2)-({EX})^2$ 
- Độ lệch chuẩn: Để quy về cùng đơn vị với dữ liệu
	- $\sigma(X)=\sqrt{V(X)}$ 
- Mode: $mod(X)$ - Giá trị X có $P(X)$ lớn nhất với biến rời rạc
- Phân vị: Giá trị $z_p$ sao cho $F(z_p)=P(X<z_p)=p$ 
	- Trung vị : $med(X)$, $P(x<med(X))= P(x  \geq med(X)) = 0,5$ 
## Một số luật phân phối xác suất thông dụng
### Phân phối nhị thức (Binomial distribution)
- Thực hiện n phép thử, mỗi phép thử có xác suất xảy ra sự kiện A là p và gọi X là số lần xảy ra sự kiện A => X tuân thủ phân phối nhị thức
- Tập giá trị của X: 0,1,2,3,4,...(số lần xảy ra 1 sự kiện)
- Xác suất tính theo Bernoulli: $P(X=k) = C^k_n.p^k.{(1-p)}^{n-k}$ 
- Kĩ hiệu: $X$ ~$B(n;p)$ 
- Tham số đặc trưng
	- $EX=np$ 
	- $VX=np(1-p)$ 
	- $(n+1)p-1 \leq mod(X) \leq (n+1)p$ 
### Phân phối Poisson (Poisson distribution)
- E là sự kiện xuất ngẫu nhiên với tần suất c, X là số lần xuất hiện của E trong 1 khoảng thời gian => X tuân theo phân phối Poisson
- Tập giá trị của X: 0,1,2,3,4,
