- 8,10,11,29
# Cộng trừ số nguyên
- Bù 1: Đảo tất cả các bit
- Bù 2: +1 vào bù 1
- Đảo dấu là lấy bù 2
- Trừ là cộng với bù 2
# Nhân số nguyên
# Chia số nguyên
# Số dấu phẩy động
- Khuôn dạng 32 bit: S-e-m
	- S là 1 bit dấu
	- e là 8 bit thể hiện giá trị dịch chuyển của phần mũ
	- m là 23 bit thể hiện phần lẻ 
- Công thức: $X=(-1)^S*1.m*2^{e-127}$
	- ![[Pasted image 20230810155003.png]]