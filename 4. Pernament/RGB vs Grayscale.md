#computer_science/image_processing
# RGB
- $r,g,b \in [0,256]$ : Chỉ số red, green, blue của một điểm ảnh tổng hợp nên màu của điểm ảnh
- Kích cỡ của 1 ảnh màu cỡ X x Y là $X.Y.3$
# Grayscale
- Một điểm ảnh chỉ gồm chỉ số $x \in [0,256]$
- $x=r*0.299 + g*0.587 + b*0.114$
- Không thể chuyển từ grayscale sang RGB chính xác