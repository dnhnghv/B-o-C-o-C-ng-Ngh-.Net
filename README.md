# Báo cáo môn học Công Nghệ.Net
# Lời cảm ơn
Kính gửi thầy Đỗ Duy Cốp
Trước khi đến với phần nội dung của báo cáo, em muốn dành một chút thời gian để bày tỏ sự biết ơn của em đến với thầy ạ!
em xin tự giới thiệu về bản thân, em tên là : Đinh Nguyễn Hoàng Vũ, sinh viên lớp K57KMT, theo dự kiến thì khoảng một năm nữa là khoá của bọn em sẽ được ra trường, tuy là vậy nhưng khi bước vào năm thứ 4 thì em tự nhận thấy rằng bản thân vẫn rất mông lung với những gì mình đã học, cũng như chưa tìm ra được cho mình một hướng đi cụ thể nào cả. Cho đến khi được học tập và làm việc với thầy thông qua môn công nghệ. net này, được học hỏi những bài học, kinh nghiệm quý giá mà thầy chia sẻ qua những tiết học. em tự thấy bản thân đã có sự trưởng thành hơn trong sự tư duy mình, đã bắt đầu nghiêm túc hơn về học tập cũng như công việc...
Em thật sự biết ơn sâu sắc về sự chỉ bảo và dạy dỗ của thầy, người đã tận tình hướng dẫn em trong suốt quá trình học tập. Thầy đã dành nhiều thời gian quý báu để hỗ trợ, chỉ dẫn chi tiết và góp ý.
Cuối cùng, em muốn bày tỏ lòng biết ơn đến thầy Đỗ Duy Cốp một lần nữa, Chúc thầy có sức khoẻ cũng như ngày càng thành công hơn trong công việc.

Em xin chân thành cảm ơn!
 

# Nội dung:
•	Trình bày (liệt kê) các bước thực hiện tạo web giám sát thời gian thực.

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
## Bài 1 :
Dưới đây là quy trình các bước chi tiết để hoàn thành yêu cầu:

1. Tạo Solution mới: Tạo một Solution mới trong Visual Studio.
2. Tạo Console App đầu tiên: Thêm một dự án mới dạng Console App và đặt tên phù hợp.
3. Viết mã trong Program.cs: Gõ code để xử lý bài toán tính tiền điện.
4. Chạy và kiểm tra ứng dụng: Đảm bảo rằng chương trình chạy đúng và tính toán chính xác.

### Tạo thư viện DLL
5. Thêm Project Library: Thêm một dự án dạng Class Library vào Solution.
6. Di chuyển xử lý vào Class Library: Chuyển phần xử lý tính toán từ Console App vào một class trong dự án Library để đảm bảo tính độc lập và tái sử dụng.
7. Biên dịch DLL: Biên dịch Library để tạo file DLL.
### Tạo Console App thứ hai
8. Tạo Console App thứ hai: Thêm một dự án Console App mới vào Solution.
10. Tham chiếu đến DLL: Add tham chiếu đến DLL vừa tạo ở bước 6.
11. Viết mã nhập liệu và sử dụng DLL: Viết mã nhập liệu và dùng DLL để xử lý tính toán, sau đó hiển thị kết quả.

### Tạo ứng dụng web
12. Tạo Project Web: Thêm một dự án Web (ASP.NET) vào Solution.
13. Thêm tham chiếu DLL: Add tham chiếu đến DLL ở bước 6.
14. Thiết kế giao diện Webform: Thêm một Webform (`default.aspx`) và tạo layout phù hợp từ Toolbox.
15. Thêm sự kiện xử lý: Đặt sự kiện `onClick` cho các nút để xử lý input.
16. Viết mã xử lý trong `default.aspx.cs: Viết mã để lấy dữ liệu từ Webform, xử lý bằng DLL và xuất kết quả lên giao diện Web.
### link : https://github.com/dnhnghv/btvncongnghe.net

## Bài 2:
1. Thiết lập Cơ sở Dữ liệu (SQL Server)
•	Tạo bảng ThanhVien: Chứa thông tin của từng thành viên, bao gồm ID, Tên, và Vị trí hiện tại.
•	Tạo bảng LichSuViTri: Chứa lịch sử thay đổi vị trí, gồm các trường ID, ID thành viên, Vị trí, Thời gian cập nhật.
•	Tạo bảng NguoiDung: Chứa thông tin đăng nhập của người dùng, bao gồm Username, Password (hash), và Quyền (cho phép xem hay cập nhật).
2. Thiết lập Dự án ASP.NET Web Application (.NET Framework)
•	Tạo một dự án ASP.NET Web Application với .NET Framework 2.0.
3. Tạo Giao diện (index.html)
•	Thiết kế giao diện trang chính index.html theo kiểu One Page Application.
•	Dùng các phần tử ảnh (PNG) để đại diện cho từng thành viên. Ảnh có thể hiển thị dưới các trạng thái khác nhau tương ứng với vị trí của từng thành viên (ở KTX, ở nhà trọ, ở trường, v.v.).
•	Sử dụng các class và id để định danh cho từng đối tượng thành viên, giúp theo dõi và thay đổi vị trí trên giao diện.
4. Cập nhật Vị trí Thành viên
•	Thêm tính năng kéo-thả các đối tượng thành viên để thay đổi vị trí. Sử dụng thư viện jQueryUI để cho phép kéo-thả.
•	Lưu các thay đổi về vị trí: Khi thả đối tượng vào vị trí mới, sử dụng CSS để xác định vị trí và cập nhật vào file CSS.
5. Tạo các Hộp thoại Xác nhận
•	Thêm các hộp thoại xác nhận bằng jQuery-Confirm khi có các thao tác quan trọng, ví dụ như thay đổi vị trí thành viên.
•	Thiết lập nội dung phù hợp cho từng hộp thoại, chẳng hạn thông báo rằng vị trí của thành viên đã được cập nhật.
6. Tạo File JavaScript (script.js)
•	Sử dụng jQuery để điều khiển các sự kiện click trên đối tượng thành viên, gọi đến các hàm để cập nhật vị trí.
•	Xử lý và gửi dữ liệu thay đổi vị trí đến API để lưu trữ trong cơ sở dữ liệu.
7. Tạo API để Cập nhật Dữ liệu (api.aspx)
•	Tạo file api.aspx và chỉ giữ lại dòng đầu tiên, xóa bỏ các mã tự động tạo.
•	Thêm mã trong api.aspx.cs để xử lý yêu cầu từ các sự kiện (cập nhật vị trí thành viên, lấy dữ liệu lịch sử).
•	Xử lý hàm Page_Load để nhận yêu cầu cập nhật vị trí và lưu dữ liệu vào cơ sở dữ liệu.
8. Tạo Form Đăng nhập
•	Thiết kế form đăng nhập trên giao diện với các trường nhập Username và Password.
•	Sử dụng mã hash mật khẩu khi lưu và kiểm tra thông tin đăng nhập trong cơ sở dữ liệu để đảm bảo bảo mật.
•	Kiểm tra đăng nhập: Chỉ người dùng đăng nhập thành công mới có quyền thay đổi vị trí thành viên, nếu không đăng nhập thì chỉ có quyền xem.
9. Thống kê và Báo cáo
•	Thêm một bảng thống kê trên giao diện để hiển thị lịch sử thay đổi vị trí của từng thành viên.
•	Tạo báo cáo với thời gian tất cả thành viên có mặt tại trường.
### link : https://github.com/dnhnghv/web_giamsatsvk57kmt

## Bài 3: Tạo Mã Caprcha
Dưới đây là các bước để thực hiện yêu cầu:

### 1. Class Library (.NET Framework 2.0) để tạo CAPTCHA (DLL)
- Tạo một dự án Class Library.
- Thêm khoảng 10 ảnh nền gây nhiễu vào Resource của dự án.
- Tạo phương thức nhận vào một chuỗi ký tự và sinh ra một ảnh `Bitmap` chứa chuỗi đó.
- Vẽ từng ký tự trong chuỗi:
  - Sử dụng font ngẫu nhiên từ một tập font xác định trước.
  - Xoay từng ký tự một góc ngẫu nhiên (-45 độ đến +45 độ).
  - Chọn kích thước, màu sắc ngẫu nhiên cho từng ký tự.
  - Đặt tọa độ `x` của mỗi ký tự tăng dần và `y` ngẫu nhiên.
- Thêm các hiệu ứng nhiễu:
  - Vẽ các đường thẳng, hình tròn, tam giác ngẫu nhiên với màu sắc, kích thước và vị trí ngẫu nhiên.

### 2. Windows Form App để kiểm thử CAPTCHA
- Tạo một ứng dụng Windows Forms.
- Tham chiếu tới DLL CAPTCHA đã tạo.
- Thêm một `PictureBox` để hiển thị CAPTCHA.
- Thêm một `TextBox` để nhập chuỗi và một `Button` để tạo ảnh CAPTCHA từ chuỗi nhập vào.
- Hiển thị ảnh CAPTCHA trong `PictureBox` khi nhấn nút.

### 3. ASP.NET Web Application để login với CAPTCHA
- Tạo một ứng dụng ASP.NET Web Forms.
- Lưu thông tin user (uid, pwd) trong cơ sở dữ liệu SQL Server.
- Sử dụng Session để đếm số lần đăng nhập thất bại.
- Sau 3 lần đăng nhập sai, hiển thị CAPTCHA yêu cầu người dùng nhập đúng để tiếp tục.
- Sinh ảnh CAPTCHA bằng cách gọi phương thức từ DLL và lưu text CAPTCHA trong Session.
- Hiển thị CAPTCHA qua thẻ `<img>` với thuộc tính `src` trỏ đến một URL sinh ảnh động hoặc base64.
- Xác thực text CAPTCHA nhập vào với text lưu trong Session khi người dùng gửi form login.
- Sử dụng các thư viện jQuery và jQuery-Confirm để hỗ trợ viết mã JavaScript cho client-side validation.

### link : [dnhnghv/Captcha (github.com)](https://github.com/dnhnghv/Captcha)
