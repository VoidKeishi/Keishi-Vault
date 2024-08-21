---
tags:
  - cpp
type:
  - reference
time created: 19-08-2024
last modified: 19-08-2024
---
- Concurrency: Khi có từ 2 công việc trở lên cùng making progress trong 1 khoảng thời gian (không nhất thiết thực hiện đồng thời)
	- Time-slicing: Thực hiện 1 công việc một thời điểm (CPU đơn nhân), phân chia thời gian giữa các công việc để đều making progress -> virtual parallelism
	- Parallelism: Từ 2 công việc trở lên được thực hiện đồng thời
- Concurrency với đa tiến trình
	- Chia chương trình được thực thi thành nhiều tiến trình
	- Giao tiếp giữa các tiến trình thường phức tạp (đòi hỏi OS) và chậm
	- Dễ đảm bảo tính an toàn
	- Dễ chạy các tiến trình trên nhiều máy khác nhau giao tiếp qua mạng
- Concurrency với đa luồng
	- Chia tiến trình thành nhiều luồng
	- Chi phí, tài nguyên yêu cầu ít hơn so với đa tiến trình
	- Cần đảm bảo phần dữ liệu được truy cập chung giữa các luồng
	- Là hướng tiếp cận của C++
- Tại sao cần sử dụng concurrency
	- Tách biệt xử lý vấn đề
		- Dễ đọc và kiểm thử
	- Tăng hiệu năng
		- 2 cách sử dụng concurrency
			- Task parallelism: Chia nhỏ công việc và chạy song song các công việc con
			- 