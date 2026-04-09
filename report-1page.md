# FIT4012 - Report 1 Page
## Lab 01 - CIA & Risk: Hệ thống lưu điểm

### 1. Mục tiêu bài lab
- Nhận diện tài sản cần bảo vệ trong một hệ thống thông tin đơn giản.
- Phân biệt Confidentiality, Integrity, Availability.
- Xác định threat, vulnerability, mitigation.
- Thực hành workflow GitHub cơ bản để nhận và nộp bài.

### 2. Cách làm
- Đọc bối cảnh và xác định các thành phần quan trọng của hệ thống.
- Phân tích từng sự cố theo bộ ba CIA.
- Chọn sự cố B để phân tích sâu hơn theo threat - vulnerability - mitigation.
- Hoàn thiện bài làm trong repo và commit/push lên GitHub.

### 3. Kết quả chính
**Assets:**
- Bảng điểm / dữ liệu điểm của sinh viên
- Tài khoản đăng nhập giảng viên và sinh viên
- Dữ liệu cá nhân sinh viên (MSSV, họ tên)

**CIA mapping:**
- Sự cố A -> Availability
- Sự cố B -> Integrity
- Sự cố C -> Confidentiality

**Phân tích sự cố B:**
- Threat: Tài khoản giảng viên bị xâm nhập hoặc người có quyền ghi điểm (giảng viên/insider) sửa điểm trái phép.
- Vulnerability: Hệ thống không kiểm tra chặt chẽ vai trò và quyền hạn khi cho phép sửa điểm, thiếu xác thực mạnh và audit log.
- Mitigation: Chỉ cho phép giảng viên hợp lệ sửa điểm, áp dụng kiểm soát truy cập theo vai trò (RBAC), yêu cầu xác thực mạnh và ghi nhật ký audit.

### 4. Kết luận ngắn
Qua bài lab này, em học được cách phân biệt rõ Confidentiality, Integrity và Availability trong một hệ thống lưu điểm. Phân tích thận trọng từng sự cố giúp thấy rõ loại rủi ro và phương án giảm thiểu phù hợp. Phần khó nhất là xác định threat và vulnerability sao cho đúng với vai trò giảng viên được phép nhập điểm. Em rút ra rằng cần chú ý kiểm soát quyền truy cập và ghi nhật ký để bảo vệ dữ liệu an toàn hơn.
