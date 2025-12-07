#networking/5g/core/concepts 
- Là một mạng logic, tách ra từ hạ tầng vật lý [[5G Core]], phục vụ một mục đích hoặc dịch vụ cụ thể như eMBB, URLLC, mIoT.
- Mỗi [[Network slice]] độc lập về mặt chức năng, tài nguyên, chính sách, như là một mạng riêng biệt chạy trên cùng một hạ tầng
- Thành phần
	- Các [[NF]] chuyên biệt, có thể triển khai riêng cho từng [[Network slice]] hoặc dùng chung
	- Chính sách riêng: QoS, bảo mật, định tuyến, truy cập,...
	- Tài nguyên logic riêng: CPU, băng thông, IP pool