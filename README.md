# Báo cáo môn học Công Nghệ.Net
Nội dung:
•	Trình bày (liệt kê) các bước thực hiện tạo web giám sát thời gian thực.
- Gợi ý:
•	Trên CSDL dùng để lưu trữ cần làm các bước gì? (lưu ý phần SP trả về json thì làm như nào?)
•	Phần cứng (ko cần làm trong báo cáo này) nhưng tác động gì tới CSDL?
•	Các bước để tạo DLL độc lập có tương tác với CSDL?
•	Các bước để tạo API trên asp dot net giúp giao tiếp bằng json giữa server và client.
•	Sử dụng trang HTML + CSS + Jquery + Jquery-ui + Jquery-confirm : để hiển thị kết quả giao tiếp với API. (sử dụng class và id của thẻ html như nào? Dùng class và id này trong css ra sao? Jquery gửi/nhận json như nào? Jquery-ui dùng để làm gì? Jquery-confirm để hiển thị các dialog ra sao? …)


Dưới đây là danh sách các bước thực hiện để tạo web giám sát thời gian thực:

## 1. Cơ sở dữ liệu (CSDL):
- Thiết kế và tạo các bảng cần thiết trong SQL Server.
- Viết stored procedures để trả về dữ liệu dạng JSON.
- Viết stored procedures để cập nhật trạng thái và ghi nhận lịch sử.
- Cấu hình quyền truy cập và bảo mật cho CSDL.

## 2. Tác động phần cứng lên CSDL:
- Xây dựng hệ thống nhận dữ liệu từ thiết bị cảm biến và đẩy dữ liệu lên CSDL.
- Đảm bảo kết nối ổn định giữa thiết bị phần cứng và hệ thống server.

### 3. Tạo DLL độc lập có tương tác với CSDL:
- Tạo dự án Class Library (DLL) trong Visual Studio.
- Thêm thư viện kết nối với SQL Server (`System.Data.SqlClient`).
- Viết các lớp xử lý để kết nối, gọi stored procedures và trả về dữ liệu.
- Biên dịch và tạo file DLL để sử dụng trong các dự án khác.

## 4. Tạo API trên ASP.NET:
- Tạo dự án ASP.NET Web API.
- Cài đặt các gói cần thiết như `Newtonsoft.Json` để xử lý JSON.
- Viết các controller để nhận yêu cầu từ client và trả về dữ liệu JSON.
- Tạo các phương thức API để gọi các stored procedures và xử lý dữ liệu từ CSDL.

## 5. Giao diện HTML + CSS + jQuery:
- Tạo trang HTML với các thẻ và cấu trúc phù hợp, sử dụng `class` và `id` để định dạng và truy xuất.
- Viết CSS để định dạng giao diện theo nhu cầu.
- Sử dụng jQuery để gửi yêu cầu AJAX đến API và nhận JSON từ server.
- Sử dụng jQuery-UI để thêm tính năng giao diện nâng cao (như dialog, widgets).
- Sử dụng jQuery-confirm để hiển thị các dialog xác nhận hoặc thông báo.
- Viết script jQuery để cập nhật nội dung trang web dựa trên dữ liệu nhận được từ API.

# Nội dung: (tiếp)
•	Trình bày (liệt kê) các bước đã thực hiện với 3 bài tập đã làm
•	Kèm link github mỗi bài.
