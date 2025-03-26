#javascript/nodejs 
# Tổng quan
- NodeJS là một open source, cross platform [[Runtime enviroment]] cho [[JavaScript]]
- [[JavaScript]] engine là chương trình dịch [[JavaScript]] sang mã máy, thường được phát triển bởi các bên cung cấp trình duyệt
	- V8 - Engine mã nguồn mở của Google
	- SpiderMonkey - Engine của Mozilla Firefox
	- JavaScriptCore - Engine mã nguồn mở của Apple cho Safari
- [[NodeJS]] sử dụng V8, viết bằng C++ và mở rộng chức năng cho V8
![[Pasted image 20241111150931.png]]
- [[Cài đặt NodeJS]]
# Module
- Trong [[NodeJS]], mỗi file là 1 module
- Các loại module
	- Local modules: Modules tự tạo
	- Built-in modules: Modules có sẵn của NodeJS
	- Third-party modules: Modules tạo bởi lập trình viên khác, chia sẻ và cài đặt như thư viện
- NodeJS tuân theo tiêu chuẩn [[CommonJS]]