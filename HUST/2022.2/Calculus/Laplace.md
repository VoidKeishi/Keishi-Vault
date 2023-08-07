# Biến đổi Laplace
- $Lf(t)\rightarrow F(s:=\int\limits_{0}^{+\infty}e^{-st}f(t)dt)$, $s>0$
- Điều kiện đủ để Laplace tồn tại
	- $f(t)$ liên tục từng khúc
	- $f(t)$ có tốc độ tăng không vượt quá hàm mũ
# Tính chất
- $L\{f+g\}=L\{f\}+L\{g\}$
- $L\{kf(t)\}=kL\{f(t)\}$
# Biến đổi Laplace ngược
- $f(t)=L^{-1}\{F(s)\}$ nếu $L\{f(t)\}=F(s)$
# Phép tịnh tiến theo trục s
- $L\{e^{at}f(t)\}=F(s-a)$
- Hệ quả: $L^{-1}\{F(s-a)\}=e^{at}.L^{-1}\{F(s)\}$
# Đạo hàm của Laplace
- $L\{f'\}=s.F(s)-f(0)$
- $L\{f''\}=s^2F(s)-sf(0)-f'(0)$
- $L\{f^{(n)}\}=s^nF(s)-s^{n-1}f(0)-...-f^{n-1}(0)$
# Tích phân của Laplace
- $L\{\frac{f(t)}{t}\}=\int\limits_{s}^{+\infty}F(s)du$
# Laplace của đạo hàm
# Laplace của tích phân
# Tích chập
- $f(t)*g(t):=\int$
# Phép tịnh tiến theo trục t