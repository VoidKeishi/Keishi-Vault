---
tags:
  - compiler
type: reference
time created: 26-09-2024
last modified: 26-09-2024
---
# Giới thiệu chung
- Một số khái niệm của ngôn ngữ lập trình
	- Cú pháp: Chính tả và văn phạm của các cấu trúc ngôn ngữ
	- Ngữ nghĩa: Ý nghĩa và hiệu quả của các cấu trúc ngôn ngữ
- Bộ xử lý ngôn ngữ
	- Các dạng
		- Compiler: Dịch từ ngôn ngữ nguồn sang mã máy
		- Assembler: Dịch từ Assembly sang mã máy
		- Interpreter: Dịch và thực thi trực tiếp từng thao tác của chương trình nguồn
	- Cấu trúc: Bộ tiền xử lý -> Trình biên dịch -> Assembler/Interpreter -> Loader/Link editor
# Các pha chính của chương trình dịch
- Tổng quan các pha
	- Phân tích từ vựng: Phân nhóm ký tự ra token
	- Phân tích cú pháp: Kiểm tra ngữ pháp của dãy token
	- Phân tích ngữ nghĩa: Phân tích ý nghĩa từng lệnh
	- Sinh mã trung gian: Mã không phụ thuộc máy, dễ tối ưu
	- Sinh mã đích: Sinh ra lệnh máy
	- Tối ưu mã: Thực hiện với mã trung gian và mã đích
- 
