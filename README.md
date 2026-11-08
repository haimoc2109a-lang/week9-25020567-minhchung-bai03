# Bài 3 - CI

Chọn lớp `ShippingCalculator` làm hệ thống mẫu, tổ chức thành Maven + SLF4J/Logback + JUnit Jupiter.

Workflow `.github/workflows/ci.yml` chạy khi `push` hoặc `pull_request`, thực hiện `mvn -B clean verify` (test, package) và upload `target/*.jar`. Chạy tại máy: `./run.sh`.

**Kiểm chứng trên GitHub (cần thực hiện thật):** tạo repository có **nội dung Bai03 làm thư mục gốc**, push bản đúng để lấy ảnh Actions xanh. Sau đó đổi kỳ vọng `15000.0` trong test sang `16000.0`, push để quan sát log `expected ... but was ...`; lưu ảnh/log; cuối cùng sửa lại và push để xanh. Không nộp log giả.
