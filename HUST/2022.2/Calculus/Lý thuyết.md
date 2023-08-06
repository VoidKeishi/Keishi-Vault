# Chuỗi
## Một số định nghĩa
### Chuỗi
- $\{u_n\}_{n=0}^{\infty}:\sum\limits_{n=1}^{\infty}u_n=u_1+u_2+...$
### Tổng riêng
- $S_n=u_1+u_2+...+u_n$ - Tổng riêng thứ n
### Phần dư
- $\{u_n\}_{n=0}^{\infty}-S_n=u_{n+1}+u_{n+2}+...$
### Sự hội tụ
- $\exists\lim\limits_{n\to\infty}S_n=S\rightarrow$ $\{u_n\}_{n=0}^\infty$ hội tụ
## Điều kiện cần để chuỗi hội tụ
- $\lim\limits_{n\to\infty}u_n=0$
## Các loại chuỗi
### Chuỗi dương
#### Định nghĩa
- $\sum\limits_{n=1}^{\infty}u_n:u_{n} \geq{0} \forall{n}$
#### 4 tiêu chuẩn so sánh
- So sánh: Cho $\sum\limits a_{n},\sum\limits b_{n}$ là hai chuỗi số dương
	- Loại 1: $a_{n}\geq{b_{n}}\forall{n} \geq{n_0}$
		- $\sum\limits a_n$ hội tụ => $\sum\limits{b_n}$ hội tụ
		- $\sum\limits b_n$ phân kỳ => $\sum\limits{a_n}$ phân kỳ
	- Loại 2: $\lim\limits_{n\rightarrow\infty}\frac{a_n}{b_n}=k$
		- $k\in(0,\infty)$ => 2 chuỗi cùng phân kỳ hoặc hội tụ
		- $k=0$ 
			- $\sum\limits b_n$ hội tụ => $\sum\limits{a_n}$ hội tụ
			- $\sum\limits a_n$ phân kỳ => $\sum\limits{b_n}$ phân kỳ
		- $k=+\infty$
			- $\sum\limits a_n$ hội tụ => $\sum\limits{b_n}$ hội tụ
			- $\sum\limits b_n$ phân kỳ => $\sum\limits{a_n}$ phân kỳ
- Tích phân: $\int\limits_{1}^{+\infty}f(x)dx$  và $\sum\limits_{n=1}^{+\infty}{f(n)}$ 
	- Cho $f(x)$ liên tục thỏa mãn $f(x)\geq{0}$ $\forall$ $x \geq 0$, $f(x)$ là hàm giảm trên $[0;+\infty)$. Khi đó: 
	- $\int\limits_{1}^{+\infty}f(x)dx$  và $\sum\limits_{n=1}^{+\infty}{f(n)}$ cùng tính chất
	- $\int\limits_{1}^{+\infty}f(x)dx$ hội tụ khi có giá trị hữu hạn
	- VD: $\sum\limits_{n=2}^{+\infty}{\frac{1}{n.ln^2(n)}}$ và $\int\limits_{2}^{+\infty}\frac{1}{x.ln^2(x)}$
- D'Alambert: Cho $\sum\limits{u_n}$ dương, $\lim\limits_{n\rightarrow+\infty}\frac{u_{n+1}}{u_n}=k$
	- $k>1\rightarrow$ phân kỳ
	- $k<1\rightarrow$ hội tụ
	- $k = 1\rightarrow$ Raphb
- Cauchy: Cho $\sum\limits{u_n}$ dương, $\lim\limits_{n\rightarrow+\infty}\sqrt[n]{u_n}=k$
	- $k>1\rightarrow$ phân kỳ
	- $k<1\rightarrow$ hội tụ
	- $k = 1\rightarrow$ Raphb
### Chuỗi có dấu bất kỳ
#### Định nghĩa
- $\sum\limits_{n=1}^{\infty}u_n,u_n$ có dấu bất kỳ
- Hội tụ tuyệt đối: $\sum\limits_{n=1}^{\infty}|{u_n}|$ hội tụ
- Bán hội tụ: $\sum\limits_{n=1}^{\infty}|{u_n}|$ phân kỳ
#### Chuỗi đan dấu
- Dạng: $\sum\limits_{n=1}^{\infty}(-1)^n.u_n,u_n\geq{0}$ $\forall$ ${n}$
- Tiêu chuẩn Leibniz
	- Nếu $u_n\rightarrow{0}$ và $\{u_n\}$ là dãy giảm
	- Thì $\sum\limits_{n=1}^{\infty}(-1)^n.u_n$ hội tụ
### Chuỗi hàm
#### Định nghĩa
- Dạng: $\sum\limits_{n=1}^{\infty}u_n(x)$
- Miền hội tụ: Tập giá trị của x làm chuỗi hội tụ
- Hội tụ đều: $\sum\limits_{n=1}^{\infty}u_n(x)$ gọi là hội tụ đều tới hàm S(x) trên tập X nếu:
	- $\forall$ $\epsilon>0$ ,$\exists$ $n_0$ : $\forall$ $n>n_0$ $|\sum\limits_{k=1}^{n}u_n(x)-S(x)|\leq\epsilon$ $\forall$ $x\in{X}$
#### Tiêu chuẩn Weierstrass:  
- Cho $\sum\limits_{n=1}^{\infty}u_n(x)$ và $\sum\limits_{n=1}^{\infty}a_n$ hội tụ
- Nếu $|u_n(x)|\leq{a_n}$ $\forall$ $x\in{X}$
- Thì $\sum\limits_{n=1}^{\infty}u_n(x)$ hội tụ đều trên X
#### Tính chất hội tụ đều
- Tính liên tục
- Tính khả tích
- Tính khả vi
#### Chuỗi lũy thừa
- Dạng $\sum\limits_{n=0}^{+\infty}a_n.x^n$, $a_n\in{R}$ 
- Định lý Abel: $\sum\limits_{n=0}^{+\infty}a_n.x^n$ hội tụ tại $x_0$ thì hội tụ tuyệt đối tại mọi $|x|<|x_0|$
- Bán kính hội tụ: $R=\lim\limits_{n\rightarrow+\infty}|\frac{a_n}{a_{n+1}}|$ hoặc $R=\lim\limits_{n\rightarrow+\infty}\frac{1}{\sqrt[n]{|a_n|}}$
- Tìm miền hội tụ:
	- Tìm bán kính hội tụ $R$
	- Xét $R,-R$ để biết lấy đầu mút không
	- Kết luận
- Tính chất: Chuỗi lũy thừa hội tụ đều trên mọi khoảng con $[a,b]$ của miền hội tụ
### Chuỗi Maclaurin
- $e^x=\sum\limits_{n=0}^{+\infty}\frac{x^n}{n!}$, $x\in{R}$
- $sin(x)=\sum\limits_{n=0}^{+\infty}\frac{(-1)^n.x^{2n+1}}{(2n+1)!}$, $x\in{R}$
- $cos(x)=\sum\limits_{n=0}^{+\infty}\frac{(-1)^n.x^{2n}}{(2n)!}$, $x\in{R}$
- $ln(1+x)=\sum\limits_{n=1}^{+\infty}\frac{x^n.(-1)^{n-1}}{n}$, $x\in(-1;1)$
- $(1+x)^\alpha=1+\alpha.x+\frac{\alpha.(\alpha-1)}{2!}.x^2+...+\frac{\alpha.(\alpha-1)...(\alpha-n+1)}{n!}.x^n$
- $\frac{1}{1-x}=\sum\limits_{n=0}^{+\infty}x^n$, $\frac{1}{1+x}=\sum\limits_{n=0}^{+\infty}(-1)^n.x^n$
### Chuỗi Fourier
#### Định nghĩa
- $f(x)=\frac{a_0}{2}+\sum\limits_{n=1}^{+\infty}(a_n.cos(\frac{\pi n.x}{L})+b_n.sin(\frac{\pi n.x}{L}))$, $f(x)$ tuần hoàn với chu kỳ $T=2L$
	- $a_0=\frac{1}{L}\int\limits_{-L}^{L}f(x)dx$
	- $a_n=\frac{1}{L}\int\limits_{-L}^{l}f(x).cos(\frac{\pi n.x}{L})dx$
	- $b_n=\frac{1}{L}\int\limits_{-L}^{L}f(x).sin(\frac{\pi n.x}{L})dx$
#### Khai triển Fourier theo hàm chẵn
- $b_n=0$
- $a_n=\frac{2}{L}\int\limits_{0}^{L}f(x).cos(\frac{\pi n.x}{L})dx$
#### Khai triển Fourier theo hàm lẻ
- $a_0,a_n=0$
- $b_n=\frac{2}{L}\int\limits_{0}^{L}f(x).sin(\frac{\pi n.x}{L})dx$
# Phương trình vi phân
- Dạng $f(x,y',y'',...,y^{(n)})=0$
	- n là cấp của phương trình vi phân - Cấp đạo hàm cao nhất
- Dạng nghiệm
	- $y=f(x)$
	- $f(x,y)=0$
	- $x=f(t),y=g(t)$
- Bài toán Cauchy: Có điều kiện ban đầu
	- VD: $y(0)=1$
## Phương trình vi phân cấp I: $f(x,y,y')=0$
### Phương trình khuyết x - $f(y,y')=0$
- Tính được $y'=f(y)$
	- Đặt $\frac{dy}{dx}=f(y)$
	- $\frac{dy}{f(y)}=$
### Phương trình khuyết y
### Phương trình phân ly biến số
### Phương trình đẳng cấp
### Phương trình vi phân tuyến tính
### Phương trình Bernoulie
### Phương trình vi phân toàn phân
## Phương trình vi phân cấp II
### Phương trình khuyết
#### Khuyết y
#### Khuyết x
### Phương trình tuyến tính cấp II
#### Thuần nhất
#### Không thuần nhất
#### Hệ số hằng
#### Phương trình Euler
### Hệ phương trình vi phân
# Toán tử Laplace
## Biến đổi Laplace
## Tính chất
## Biến đổi Laplace ngược
## Phép tịnh tiến theo trục s
## Đạo hàm của Laplace
## Tích phân của Laplace
## Laplace của đạo hàm
## Laplace của tích phân
## Tích chập
## Phép tịnh tiến theo trục t