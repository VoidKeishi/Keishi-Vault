# Định nghĩa
- $\sum\limits_{n=1}^{\infty}u_n:u_{n} \geq{0} \forall{n}$
# 4 tiêu chuẩn so sánh
## So sánh: 
- Cho $\sum\limits a_{n},\sum\limits b_{n}$ là hai chuỗi số dương
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
## Tích phân: $\int\limits_{1}^{+\infty}f(x)dx$  và $\sum\limits_{n=1}^{+\infty}{f(n)}$ 
- Cho $f(x)$ liên tục thỏa mãn $f(x)\geq{0}$ $\forall$ $x \geq 0$, $f(x)$ là hàm giảm trên $[0;+\infty)$. Khi đó: 
- $\int\limits_{1}^{+\infty}f(x)dx$  và $\sum\limits_{n=1}^{+\infty}{f(n)}$ cùng tính chất
- $\int\limits_{1}^{+\infty}f(x)dx$ hội tụ khi có giá trị hữu hạn
- VD: $\sum\limits_{n=2}^{+\infty}{\frac{1}{n.ln^2(n)}}$ và $\int\limits_{2}^{+\infty}\frac{1}{x.ln^2(x)}$
## D'Alambert: Cho $\sum\limits{u_n}$ dương, $\lim\limits_{n\rightarrow+\infty}\frac{u_{n+1}}{u_n}=k$
- $k>1\rightarrow$ phân kỳ
- $k<1\rightarrow$ hội tụ
- $k = 1\rightarrow$ Raphb
## Cauchy: Cho $\sum\limits{u_n}$ dương, $\lim\limits_{n\rightarrow+\infty}\sqrt[n]{u_n}=k$
- $k>1\rightarrow$ phân kỳ
- $k<1\rightarrow$ hội tụ
- $k = 1\rightarrow$ Raphb