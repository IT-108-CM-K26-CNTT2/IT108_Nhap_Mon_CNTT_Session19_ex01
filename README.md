# Bài 1 : Xử lý cảnh báo đăng nhập giả mạo GitHub
## 2. Hiện trường giả
Sinh viên nộp một đoạn mã giả lập kiểm tra chuỗi URL nhưng lại bỏ qua việc kiểm tra các ký tự Unicode gây nhầm lẫn (Homograph attack).

## 3. Yêu cầu đầu ra
**Chỉ ra ký tự lạ trong URL trên và giải thích tại sao nó có thể đánh lừa người dùng.**
- [**https://githúb.com/login**](https://xn--githb-bva.com/login).
- mã bị chỉnh chữ github thành githúb và dẫn vào một link url khác của hacker
- Vì người dùng hay quen tay ấn và,phản xạ theo thói quen không kiểm tra kĩ chỉ lướt qua dẫn đến sự chủ quan.
  
**Đề xuất quy trình kiểm tra URL nhanh bằng mắt thường và công cụ hỗ trợ trước khi nhập Master Password.**
- Quy trình kiểm tra URL nhanh bằng mắt thường:
- Đọc nhanh thanh tìm kiếm từ trái sang phải,tập trung vào tên miền lẫn đuôi phía sau
- check kĩ các từ đúng kí tự (chắc chắn không có: khoảng trắng,@ hay xn--, các chữ cái la tin) phải có https://
- Nhớ mình đến bằng cách nào: bấm link từ email, tin nhắn hay quảng cáo thì không nhập.
**Công cụ hỗ trợ trước khi nhập Master Password**
  |Công cụ|Các dùng|
  |---|---|
  |Bookmark|Lưu sẵn những công cụ thưỡng xuyên vào|
  |AutoFill|Tự điền thông tin khi đã đúng URL|
  |Passkey|Gắn với tên miền thật, nên trên trang giả mạo sẽ không hoạt động|
  |Bật 2FA|Cho tài khoản trình quản lý mật khẩu.|
  |VirusTotal, URLScan.io|dán URL đáng ngờ để kiểm tra mà không cần mở.|
