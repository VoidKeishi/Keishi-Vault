---
tags:
  - devops_tool
  - sentry
type: pernament
time created: 29-11-2024
last modified: 29-11-2024
---
- [Nguồn - Sentry docs](https://docs.sentry.io/product/sentry-basics/integrate-frontend/upload-source-maps/)
- Là 1 loại files giúp tool như [[Sentry]] có thể truy ngược, tạo ra code JS được viết từ code JS đã dịch và biến đổi
- Cách tạo và upload source map
	- Tạo bằng Javascript build tool - Nếu sử dụng webpack
	- Sử dụng [Sentry Wizard](https://docs.sentry.io/platforms/javascript/sourcemaps/#uploading-source-maps)
- Theo dõi lỗi trong trang Issues của [[Sentry]]