# Mobile Game Testing Project: Candy Crush Saga

Dự án này thực hiện kiểm thử thủ công (Manual Testing) các logic cốt lõi của trò chơi Candy Crush. Mục tiêu là đảm bảo tính chính xác của thuật toán xử lý kẹo, trải nghiệm người dùng mượt mà và sự ổn định của ứng dụng trên thiết bị di động.

## 📌 Tổng quan dự án
* **Sản phẩm:** Candy Crush Saga (Mobile Game)
* **Phạm vi kiểm thử:** Functional Testing (Kiểm thử chức năng), Logic Testing, Interrupt Testing (Kiểm thử gián đoạn).
* **Trạng thái:** Hoàn thành bộ Test Cases và Tài liệu yêu cầu.

---

## 🛠 Các chức năng kiểm thử chính (Scope)

Dự án tập trung vào 4 Module logic quan trọng nhất của trò chơi:

1. **Hoán đổi kẹo (Candy Swapping):** - Kiểm tra logic hoán đổi giữa 2 viên kẹo kề nhau theo hàng ngang/dọc.
   - Xác nhận cơ chế hoàn tác (Revert) khi hoán đổi không tạo ra cụm match hợp lệ.
2. **Nổ kẹo (Candy Matching):** - Kiểm tra nhận diện cụm 3 viên cùng màu.
   - Xác nhận tính toán điểm số và hiệu ứng biến mất của kẹo.
3. **Lấp đầy kẹo (Candy Refilling):** - Kiểm tra cơ chế rơi kẹo tự do (Gravity) sau khi nổ.
   - Đảm bảo kẹo mới sinh ra từ đỉnh bảng luôn lấp đầy các ô trống.
4. **Tạo kẹo đặc biệt (Special Candy Creation):** - Kiểm tra logic tạo kẹo Sọc (match 4), kẹo Gói (hình chữ L/T), và Bom màu (match 5).

---

## 📂 Cấu trúc tài liệu (Project Structure)

Dự án bao gồm các tài liệu chi tiết sau:

* **[Requirement Specification]:** Mô tả chi tiết các quy tắc nghiệp vụ (Business Rules) và logic vận hành của từng loại kẹo.
* **[Test Case Specification]:** Tập hợp các kịch bản kiểm thử từ cơ bản đến nâng cao, bao gồm cả các trường hợp ngoại lệ (Edge cases),kiểm tra độ ổn định khi thiết bị ở trạng thái **Pin yếu (< 20%)** và **vừa sạc vừa chơi**.

---

## 📱 Môi trường kiểm thử (Testing Environment)

* **Thiết bị:** iPhone 13 pro (iOS 18.7)
* **Công cụ quản lý:** Google Sheets, Jira (Bug Tracking)
* **Điều kiện đặc biệt:** Kiểm thử hiệu năng (Performance) trong tình trạng thiết bị nóng do vừa sạc vừa xử lý đồ họa nặng.

---

## 🚀 Cách xem dự án

1. Đọc file `REQUIREMENT` để nắm rõ luật chơi và logic hệ thống.
2. Theo dõi các bước thực hiện trong `TEST_CASES` để đối chiếu kết quả thực tế (Actual Result) với kết quả mong đợi (Expected Result).

---

## Link
* **Test case:** https://docs.google.com/spreadsheets/d/1RFPoVVlOU6_CC3DNG-ren9hFE4-YZhIFGmV91RFjm3A/edit?gid=1934597564#gid=1934597564
