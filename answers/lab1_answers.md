# Lab 01 Answers
## CIA & Risk: Hệ thống lưu điểm

**Họ và tên:** Trần Đình Khiêm

**MSSV:** 1871020334

**Lớp/Nhóm:** CNTT18-01

---

## 1. Assets
Liệt kê ít nhất 2 assets cần bảo vệ.

- Asset 1: Bảng điểm / dữ liệu điểm của sinh viên
- Asset 2: Tài khoản đăng nhập giảng viên và sinh viên
- Asset 3 (nếu có): Dữ liệu cá nhân sinh viên (MSSV, họ tên)

---

## 2. Mapping CIA
Ghép từng sự cố với CIA.

- Sự cố A -> Availability
- Sự cố B -> Integrity
- Sự cố C -> Confidentiality

---

## 3. Phân tích sự cố B
- Threat: Tài khoản giảng viên bị xâm nhập hoặc người có quyền ghi điểm (giảng viên/insider) sửa điểm trái phép, dẫn đến điểm của sinh viên bị thay đổi.
- Vulnerability: Hệ thống không kiểm tra chặt chẽ vai trò và quyền hạn khi cho phép sửa điểm, đồng thời thiếu xác thực mạnh và thiếu cơ chế audit log cho các thay đổi điểm.
- Mitigation: Chỉ cho phép giảng viên hợp lệ sửa điểm, áp dụng kiểm soát truy cập theo vai trò (RBAC), yêu cầu xác thực mạnh, và ghi nhật ký audit cho mọi thay đổi điểm.

---

## 4. Reflection
Nếu là quản trị viên, em sẽ ưu tiên xử lý sự cố B trước vì nó làm mất tính toàn vẹn của dữ liệu học tập và ảnh hưởng trực tiếp đến kết quả sinh viên. Điểm bị đổi có thể gây mất niềm tin và tranh chấp, nên phải xử lý gấp. Sau đó em sẽ xử lý C để bảo vệ thông tin điểm khỏi bị lộ. Cuối cùng em sẽ xử lý A để đảm bảo người dùng truy cập hệ thống ổn định.

---

## 5. Bonus Flag
`FIT4012{A-?-B-?-C-?}`

Flag của em: FIT4012{A-A-B-I-C-C}

