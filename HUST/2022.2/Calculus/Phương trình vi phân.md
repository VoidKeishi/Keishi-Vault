
# Định nghĩa mở đầu
- Dạng $f(x,y',y'',...,y^{(n)})=0$
	- n là cấp của phương trình vi phân - Cấp đạo hàm cao nhất
- Dạng nghiệm
	- $y=f(x)$
	- $f(x,y)=0$
	- $x=f(t),y=g(t)$
- Bài toán Cauchy: Có điều kiện ban đầu
	- VD: $y(0)=1$
# Phương trình vi phân cấp I: $f(x,y,y')=0$
## Phương trình khuyết x - $f(y,y')=0$
- Tính được $y'=f(y)$
	- Đặt $\frac{dy}{dx}=f(y)$
	- $\frac{dy}{f(y)}=dx$
	- $\int\frac{dy}{f(y)}=\int{dx}$
- Tính được $y=f(y')$
	- Đặt $y'=t \rightarrow y=f(t) \rightarrow dx=\frac{dy}{t}=\frac{f'(t)dt}{t}$
	- $x=\int\frac{f'(t)}{t}dt$
- Không giải được đối với $y,y'$
	- Đặt $y'=a(t),y=b(t)$, tìm x theo t
## Phương trình khuyết y - $f(x,y')$
- Dạng $y'=f(x)$ - Tính nguyên hàm 2 vế
- Dạng $x=f(y')$
	- Đặt $y'=t$
	- $x=f(t)$
	- $dy=f'(t)dt$
	- $y=\int{f'(t)}dt$
## Phương trình biến số phân ly - $f(x)dx=f(y)dy$
- $\int{f(x)}dx=\int{f(y)}dy$
## Phương trình đẳng cấp - $y'=f(\frac{y}{x})$
- Đặt $u=\frac{y}{x} \rightarrow$ phương trình biến số phân ly
## Phương trình vi phân tuyến tính
- Dạng $y'+p(x).y=q(x)$
- $\rightarrow[ye^{\int{p(x)}dx}]'=q(x).e^{\int{p(x)}dx}$
- $\rightarrow y=e^{-\int{p(x)}dx}.[\int{q(x)}.e^{\int{p(x)}dx}dx+C]$
## Phương trình Bernoulie
- Dạng $y'+p(x)y=q(x)y^\alpha$, $\alpha\neq0;1$
- Xét $y=0$ có là nghiệm
- Giả sử $y\neq0$, chia cả 2 vế cho $y^\alpha$
- $\rightarrow y'.y^{-\alpha}+p(x).y^{1-\alpha}=q(x)$
- Đặt $z=y^{1-\alpha}\rightarrow z'=(1-\alpha).y^{-\alpha}.y'$
- $\rightarrow\frac{z'}{1-\alpha}+p(x)z=q(x)\rightarrow$ Phương trình vi phân tuyến tính
## Phương trình vi phân toàn phân
- $P(x,y)dx+Q(x,y)dy=0$ với $P'_y=Q'_x$
- Lập hệ $u'_x=P,u'_y=Q$
- $u=\int{P(x,y)dx+C(y)}$
- $u'_y=Q\rightarrow C(y)=?$
# Phương trình vi phân cấp II
- $f(x,y,y',y'')=0$
## Phương trình khuyết
### Khuyết x
- $f(y,y',y'')=0$
- Đặt $y'=u\rightarrow y''=\frac{du}{dy}u$
### Khuyết y
- $f(x,y',y'')=0$
- Đặt $y'=u\rightarrow f(x,u,u')=0$
- Giải ra $u\rightarrow y' \rightarrow y$ 
## Phương trình tuyến tính cấp II
### Thuần nhất
- $y''+p(x)y'+q(x)y=0$
### Không thuần nhất
- $y''+p(x)y'+q(x)y=f(x)$
### Hệ số hằng
- $y''+ay'+by=f(x)$
### Phương trình Euler
# Hệ phương trình vi phân
## Hệ PTVP tuyến tính
- Đưa về PTVP cấp 2
## Hệ PTVP phi tuyến