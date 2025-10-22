# FreeCodeCamp — Quality Assurance Projects

This repository contains my solutions and projects for the freeCodeCamp Quality Assurance certification.

## Mục tiêu

Kho này tập hợp các bài tập từ chương trình Quality Assurance trong freeCodeCamp. Mục tiêu:

- Hoàn thành các bài tập thực hành (Unit testing, Functional testing, Integration testing).
- Triển khai các server/app nhỏ dùng để kiểm thử.
- Học cách viết test bằng Mocha, Chai, Chai-HTTP và các công cụ khác.

## Cấu trúc thư mục

- `American British Translator/` — Bài dịch Anh Mỹ, kèm server và tests.
- `Issue Tracker/` — Ứng dụng theo dõi issue, UI và tests.
- `Library/` — Ứng dụng quản lý thư viện cùng tests và endpoints mẫu.
- `Metric Imperial Converter/`, `Sodoku Solver/`, ... — Các bài tập khác (nếu có).

> Lưu ý: một số sub-projects đã có file `README.md` riêng (ví dụ `American British Translator`).

## Các công cụ & phụ thuộc

- Node.js (14+ khuyến nghị)
- Mocha — test runner
- Chai — assertion library
- Chai-HTTP — HTTP integration testing
- Express — web framework (nếu dự án dùng server)

Các phụ thuộc cụ thể nằm trong file `package.json` từng sub-project.

## Hướng dẫn chạy nhanh (từng project)

1. Chuyển vào thư mục sub-project, ví dụ:

   cd "Quality Assurance Projects\American British Translator"

2. Với những projects có sử dụng model vui lòng thêm file env với mẫu
   DB=your-mongodb-xxx
   PORT=3000
   NODE_ENV=test

3. Cài đặt phụ thuộc:

   npm install

4. Chạy server (nếu có):

   npm start

5. Chạy test:

   npm test

## Checklist khi nộp bài lên freeCodeCamp

- [ ] Tất cả tests local pass (Mocha/Chai)
- [ ] Ứng dụng lắng nghe port được yêu cầu (thường là 3000 hoặc process.env.PORT)
- [ ] Các endpoint trả về đúng JSON/HTML theo đề bài
- [ ] Không in lỗi ra console ở production

## Mẹo & ghi chú

- Kiểm tra `sample.env` hoặc `.env` (nếu có) để cấu hình biến môi trường.
- Nếu test dùng cơ sở dữ liệu tạm (cơ sở kiểm thử), reset dữ liệu trước mỗi test.
- Dùng `npm run test:watch` hoặc `nodemon` khi phát triển để tự động reload.
- Nếu gặp lỗi port đang được dùng, đổi PORT bằng biến môi trường.

## Góp ý & đóng góp

Bạn có thể mở issue hoặc PR để góp ý, sửa lỗi hoặc thêm giải pháp khác cho các bài tập.

---

_File này được tạo tự động để giúp quản lý các dự án Quality Assurance từ khóa học freeCodeCamp._
