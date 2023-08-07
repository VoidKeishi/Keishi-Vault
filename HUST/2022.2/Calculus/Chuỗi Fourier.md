# Định nghĩa
- $f(x)=\frac{a_0}{2}+\sum\limits_{n=1}^{+\infty}(a_n.cos(\frac{\pi n.x}{L})+b_n.sin(\frac{\pi n.x}{L}))$, $f(x)$ tuần hoàn với chu kỳ $T=2L$
	- $a_0=\frac{1}{L}\int\limits_{-L}^{L}f(x)dx$
	- $a_n=\frac{1}{L}\int\limits_{-L}^{l}f(x).cos(\frac{\pi n.x}{L})dx$
	- $b_n=\frac{1}{L}\int\limits_{-L}^{L}f(x).sin(\frac{\pi n.x}{L})dx$
# Khai triển Fourier theo hàm chẵn
- $b_n=0$
- $a_n=\frac{2}{L}\int\limits_{0}^{L}f(x).cos(\frac{\pi n.x}{L})dx$
# Khai triển Fourier theo hàm lẻ
- $a_0,a_n=0$
- $b_n=\frac{2}{L}\int\limits_{0}^{L}f(x).sin(\frac{\pi n.x}{L})dx$