# Ứng dụng Lên Kế Hoạch Bữa Ăn Gia Đình

## I. Tổng quan dự án

### 1. Mục tiêu
Xây dựng một ứng dụng web nhằm:
- Hỗ trợ người dùng quản lý nguyên liệu sẵn có và công thức nấu ăn.  
- Tự động gợi ý thực đơn theo ngày/tuần dựa trên nhu cầu dinh dưỡng, sở thích và số lượng thành viên trong gia đình.  
- Sinh danh sách mua sắm (shopping list) từ thực đơn đã lên kế hoạch.  
- Cung cấp thống kê dinh dưỡng, đảm bảo bữa ăn cân bằng.  

### 2. Phạm vi ứng dụng
Ứng dụng tập trung vào các chức năng:
- Đăng ký/đăng nhập người dùng.  
- Quản lý nguyên liệu và công thức món ăn.  
- Lập kế hoạch bữa ăn hằng ngày/tuần.  
- Sinh danh sách mua sắm.  
- Thống kê, gợi ý dinh dưỡng cơ bản.  

Trong giai đoạn mở rộng, ứng dụng có thể tích hợp:
- AI gợi ý thực đơn thông minh.  
- Kết nối với dịch vụ giao hàng siêu thị.  
- Xuất báo cáo thực đơn ra PDF/Excel để chia sẻ.  

### 3. Giả định và Ràng buộc
- Hệ thống chỉ phục vụ cho việc lên kế hoạch bữa ăn gia đình, không phải là một nền tảng nấu ăn chuyên nghiệp hay dịch vụ giao đồ ăn.  
- Hệ thống quản lý công thức, nguyên liệu và kế hoạch bữa ăn, không phải là phần mềm kế toán, quản lý kho hay mua sắm trực tuyến toàn diện.  
- Hệ thống hỗ trợ sinh danh sách mua sắm, nhưng không tích hợp trực tiếp với siêu thị hoặc đơn vị cung cấp thực phẩm bên ngoài.  
- Hệ thống có chức năng thống kê dinh dưỡng cơ bản, không phải là một ứng dụng y tế chuyên sâu hay phần mềm theo dõi sức khỏe toàn diện.

## II Yêu cầu chức năng  
### 1 Các tác nhân  

- **Guest (Khách vãng lai):** Người dùng chưa đăng nhập, chỉ có thể xem giới thiệu ứng dụng hoặc một số công thức mẫu.  
- **User (Người dùng/Thành viên gia đình):** Người dùng có tài khoản, đăng nhập để quản lý nguyên liệu, công thức, lập kế hoạch bữa ăn.  
- **Planner (Người lập kế hoạch):** Lên kế hoạch bữa ăn, sinh danh sách mua sắm và xem thống kê dinh dưỡng.  
- **Nutritionist (Chuyên gia dinh dưỡng):** Cung cấp dữ liệu dinh dưỡng, đưa ra khuyến nghị về chế độ ăn.  
- **Admin (Quản trị viên):** Quản lý tài khoản, công thức mặc định và giám sát hệ thống.

##CHỖ NÀY CODE CÁI USER CASE 

## 2 Các chức năng chính  

### 👤 Guest (Khách vãng lai)  
- Xem công thức nấu ăn: Danh sách công thức sẵn có.  
- Tìm kiếm công thức: Theo nguyên liệu, loại món, hoặc chế độ ăn.  
- Xem chi tiết công thức: Nguyên liệu, cách chế biến, hình ảnh, thông tin dinh dưỡng.  
- Đăng ký: Tạo tài khoản mới để sử dụng đầy đủ tính năng.  
- Đăng nhập: Truy cập bằng tài khoản đã đăng ký.  

---

### 👩‍🍳 User (Người dùng)  
- Quản lý tài khoản: Cập nhật thông tin cá nhân, mật khẩu, chế độ ăn.  
- Quản lý nguyên liệu: Thêm, sửa, xóa nguyên liệu có sẵn trong gia đình.  
- Quản lý công thức cá nhân: Lưu công thức yêu thích hoặc tự tạo công thức riêng.  
- Lên kế hoạch bữa ăn: Tạo kế hoạch bữa ăn hằng ngày/tuần.  
- Sinh danh sách mua sắm: Tự động tạo shopping list từ kế hoạch bữa ăn.  
- Theo dõi dinh dưỡng: Thống kê calo, chất đạm, chất béo, vitamin,...  

---

### 🥗 Nutritionist (Chuyên gia dinh dưỡng)
- Gợi ý thực đơn thông minh: Đưa ra gợi ý dựa trên nhu cầu dinh dưỡng.  
- Kiểm tra cân bằng dinh dưỡng: Đánh giá chế độ ăn hiện tại.  
- Đưa ra khuyến nghị: Tư vấn cải thiện bữa ăn cho người dùng.  


### 🛠️ Admin (Quản trị viên)  
- Quản lý tài khoản: Xem, tạo, sửa, xóa, khóa/mở khóa tài khoản người dùng.  
- Quản lý công thức: Duyệt, chỉnh sửa, xóa công thức trong hệ thống.  
- Quản lý dữ liệu: Giám sát nguyên liệu, kế hoạch ăn, shopping list.  
- Cấu hình hệ thống: Quản lý các cài đặt chung, tham số dinh dưỡng mặc định.
- 
# Biểu đồ Use Case
##CHỖ NÀY CODE CÁI USER CASE 
# Biểu đồ Use Case chi tiết
##CHỖ NÀY CODE CÁI USER CASE 
# Chức năng Guest
##CHỖ NÀY CODE CÁI USER CASE 
# Chức năng User
##CHỖ NÀY CODE CÁI USER CASE 
# Chức năng Planner
##CHỖ NÀY CODE CÁI USER CASE 
# Chức năng Nutritionist
##CHỖ NÀY CODE CÁI USER CASE 
# Chức năng Admin
##CHỖ NÀY CODE CÁI USER CASE

## Quy trình hoạt động

###  Quy trình lên kế hoạch bữa ăn
 **Thành viên gia đình**  
   - Đăng nhập ứng dụng.  
   - Chọn **"Tạo kế hoạch bữa ăn"**.  
   - Nhập số bữa, loại món (sáng/trưa/tối), khẩu vị, nguyên liệu mong muốn.  

 **Hệ thống**  
   - Lưu kế hoạch với trạng thái **"Chờ xác nhận"**.  
   - Gợi ý thực đơn dựa trên dữ liệu có sẵn.  
   - Gửi thông báo đến **Người phụ trách nấu ăn**.  

 **Người phụ trách nấu ăn**  
   - Xem kế hoạch, điều chỉnh thực đơn nếu cần.  
   - Với bữa quan trọng → gửi lên **Người lớn trong gia đình** duyệt.  

 **Người lớn trong gia đình (Bố/Mẹ/Ông/Bà)**  
   - Xem lại kế hoạch bữa ăn, chi phí và nguyên liệu.  
   - **Phê duyệt** hoặc **Yêu cầu chỉnh sửa**.  

 **Hệ thống**  
   - Cập nhật trạng thái cuối cùng.  
   - Gửi thông báo cho cả gia đình về **menu & phân công công việc**.


##CHỖ NÀY CODE CÁI USER CASE

## III. Các Luồng Xử Lý

### 1. Luồng xử lý: Tạo kế hoạch bữa ăn
- **Diễn viên chính**: Thành viên gia đình  
- **Mô tả**: Người dùng muốn tạo kế hoạch bữa ăn cho ngày/tuần  
- **Luồng chính**:
  1. Thành viên đăng nhập vào ứng dụng.  
  2. Chọn chức năng **"Tạo kế hoạch bữa ăn"**.  
  3. Nhập thông tin: số bữa, khẩu vị, nguyên liệu mong muốn.  
  4. Hệ thống gợi ý thực đơn.  
  5. Người dùng xác nhận kế hoạch.  
  6. Hệ thống lưu kế hoạch ở trạng thái **"Chờ xác nhận"**.  
- **Luồng phụ/ngoại lệ**:  
  - Nếu thiếu thông tin → Hệ thống yêu cầu bổ sung.  
  - Nếu không có món phù hợp → Hệ thống gợi ý thay thế từ kho công thức.  

---

### 2. Luồng xử lý: Xem và chỉnh sửa kế hoạch
- **Diễn viên chính**: Người phụ trách nấu ăn  
- **Mô tả**: Kiểm tra và điều chỉnh kế hoạch bữa ăn đã tạo  
- **Luồng chính**:
  1. Người phụ trách đăng nhập.  
  2. Truy cập danh sách kế hoạch **"Chờ xác nhận"**.  
  3. Xem chi tiết kế hoạch và đề xuất chỉnh sửa (món ăn, khẩu phần, chi phí).  
  4. Lưu thay đổi.  
  5. Với bữa quan trọng → gửi lên **Người lớn trong gia đình** duyệt.  
- **Luồng phụ/ngoại lệ**:  
  - Nếu nguyên liệu không có sẵn → Đánh dấu cần đi chợ.  
  - Nếu chi phí vượt ngân sách → Cảnh báo cho người dùng.  

---

### 3. Luồng xử lý: Phê duyệt kế hoạch
- **Diễn viên chính**: Người lớn trong gia đình (Bố/Mẹ/Ông/Bà)  
- **Mô tả**: Duyệt hoặc từ chối kế hoạch bữa ăn quan trọng  
- **Luồng chính**:
  1. Người lớn đăng nhập.  
  2. Truy cập danh sách kế hoạch cần phê duyệt.  
  3. Xem thông tin: thực đơn, chi phí, nguyên liệu.  
  4. Chọn **Phê duyệt** hoặc **Từ chối**.  
  5. Hệ thống cập nhật trạng thái kế hoạch.  
- **Luồng phụ/ngoại lệ**:  
  - Nếu từ chối → hệ thống trả về trạng thái **"Cần chỉnh sửa"** và thông báo cho người phụ trách.  

---

### 4. Luồng xử lý: Đi chợ & chuẩn bị bữa ăn
- **Diễn viên chính**: Người đi chợ, Người nấu ăn  
- **Mô tả**: Sau khi kế hoạch được duyệt, các công việc được phân công  
- **Luồng chính**:
  1. Ứng dụng phân công công việc (ai đi chợ, ai nấu, ai dọn).  
  2. Người đi chợ xem danh sách nguyên liệu cần mua.  
  3. Người nấu ăn xem công thức, bước chế biến.  
  4. Sau khi hoàn tất, đánh dấu công việc **Hoàn thành**.  
- **Luồng phụ/ngoại lệ**:  
  - Nếu thiếu nguyên liệu → có thể cập nhật thay thế trong ứng dụng.  
  - Nếu có sự thay đổi đột xuất → Người dùng khác có thể nhận thay công việc.  

---

### 5. Luồng xử lý: Thông báo & nhắc nhở
- **Diễn viên chính**: Hệ thống  
- **Mô tả**: Gửi thông báo cho các thành viên  
- **Luồng chính**:
  1. Gửi thông báo khi có kế hoạch mới được tạo.  
  2. Gửi thông báo khi kế hoạch được duyệt hoặc yêu cầu chỉnh sửa.  
  3. Nhắc nhở khi đến giờ đi chợ/nấu ăn/dọn dẹp.  
  4. Thông báo kết quả sau khi bữa ăn hoàn thành.




  ## IV. Các trạng thái thực thể trong hệ thống

### 1. Trạng thái Kế hoạch bữa ăn
| Trạng thái | Mô tả |
|------------|-------|
| **Mới tạo** | Kế hoạch vừa được tạo bởi thành viên, chưa có xác nhận. |
| **Chờ xác nhận** | Kế hoạch đang chờ người phụ trách nấu ăn hoặc người lớn trong gia đình xem xét. |
| **Chờ phê duyệt** | Kế hoạch quan trọng đã được chỉnh sửa, đang chờ người lớn trong gia đình phê duyệt. |
| **Đã phê duyệt** | Kế hoạch đã được phê duyệt, có thể tiến hành đi chợ và chuẩn bị bữa ăn. |
| **Đang thực hiện** | Công việc đi chợ, nấu ăn đang diễn ra. |
| **Hoàn thành** | Bữa ăn đã chuẩn bị xong, tất cả công việc liên quan đã hoàn tất. |
| **Bị từ chối/Chỉnh sửa** | Kế hoạch bị từ chối hoặc yêu cầu chỉnh sửa; người tạo cần cập nhật lại. |

---

### 2. Trạng thái Món ăn
| Trạng thái | Mô tả |
|------------|-------|
| **Đang gợi ý** | Món ăn được hệ thống gợi ý dựa trên nguyên liệu và khẩu vị. |
| **Đang chọn** | Thành viên hoặc người phụ trách nấu ăn đang chọn món cho thực đơn. |
| **Đã chọn** | Món ăn đã được thêm vào kế hoạch bữa ăn. |
| **Đang chuẩn bị** | Món ăn đang được nấu/chế biến. |
| **Hoàn thành** | Món ăn đã nấu xong và sẵn sàng phục vụ. |
| **Bị loại bỏ** | Món ăn không được chọn hoặc bị thay thế bởi món khác. |

---

### 3. Trạng thái Công việc
| Trạng thái | Mô tả |
|------------|-------|
| **Chưa bắt đầu** | Công việc (đi chợ, nấu, dọn) chưa thực hiện. |
| **Đang thực hiện** | Công việc đang được tiến hành. |
| **Hoàn thành** | Công việc đã hoàn tất. |
| **Bị hoãn** | Công việc tạm thời bị hoãn do thiếu nguyên liệu hoặc lý do khác. |


## V. Yêu cầu phi chức năng

###  Hiệu suất
-  **Tải trang**: Thời gian tải các màn hình chính (trang kế hoạch, thực đơn, danh sách công việc) không quá **3 giây**.  
-  **API phản hồi**: Thời gian phản hồi cho các API quan trọng (tạo kế hoạch, đồng bộ công việc, xem thực đơn) không quá **1 giây**.  
-  **Chịu tải đồng thời**: Hệ thống phải hỗ trợ ổn định khi có tối thiểu **20 thành viên** cùng lúc truy cập, chỉnh sửa kế hoạch hoặc cập nhật thực đơn.  
-  **Tài nguyên tối ưu**: Hình ảnh món ăn và tài nguyên tĩnh (CSS/JS) phải được nén để giảm thời gian tải.  

###  Bảo mật
-  **Mã hóa dữ liệu**: Thông tin người dùng (tài khoản, chế độ ăn, lịch sử bữa ăn) phải được mã hóa mạnh trong cơ sở dữ liệu.  
-  **Chống tấn công**: Hệ thống có cơ chế phòng chống SQL Injection, Cross-Site Scripting và CSRF.  
-  **Logging**: Ghi lại các hoạt động quan trọng như đăng nhập, tạo/ký duyệt kế hoạch, chỉnh sửa thực đơn.  
-  **Sao lưu định kỳ**: Dữ liệu (kế hoạch, công thức món ăn) phải được sao lưu tự động theo định kỳ.  

###  Khả năng mở rộng
-  **Kiến trúc Module**: Hệ thống xây dựng theo kiến trúc module để dễ dàng bảo trì và thêm tính năng mới (ví dụ: theo dõi dinh dưỡng, thống kê chi phí).  
-  **Tích hợp bên thứ ba**: Sẵn sàng tích hợp với dịch vụ mua sắm online hoặc ứng dụng quản lý sức khỏe.  
-  **Tài liệu hóa**: Cung cấp tài liệu API rõ ràng cho các nhà phát triển muốn mở rộng ứng dụng.  

###  Giao diện người dùng
-  **Thiết kế đáp ứng (Responsive)**: Giao diện hiển thị tốt trên mọi kích thước màn hình, từ điện thoại đến máy tính bảng và PC.  
-  **Dễ sử dụng**: Người dùng mới có thể làm quen và sử dụng các chức năng chính (tạo kế hoạch, xem thực đơn, phân công công việc) trong vòng dưới **15 phút**.  
-  **Tính nhất quán**: Giao diện và luồng hoạt động đồng bộ trên toàn bộ hệ thống.  

###  Tương thích
-  **Trình duyệt**: Hoạt động tốt trên Chrome, Firefox, Safari, Edge.  
-  **Thiết bị di động**: Tương thích với Android và iOS.  
-  **Tối ưu kết nối**: Ứng dụng vẫn hoạt động mượt mà ngay cả khi kết nối Internet chậm.  

###  Độ tin cậy
-  **Uptime**: Hệ thống hoạt động ổn định tối thiểu **99.5%**.  
-  **Phục hồi sau sự cố**: Thời gian phục hồi hệ thống không quá **2 giờ** sau khi xảy ra sự cố.  
-  **Kế hoạch dự phòng**: Có phương án dự phòng cho cơ sở dữ liệu và máy chủ.  

###  Khả năng bảo trì
-  **Clean Code**: Mã nguồn tuân thủ tiêu chuẩn clean code, dễ đọc và dễ mở rộng.  
-  **Tài liệu kỹ thuật**: Các chức năng quan trọng và quyết định kiến trúc phải được ghi chú rõ ràng.  
-  **Khả năng Rollback**: Có quy trình triển khai cho phép dễ dàng quay lại phiên bản ổn định nếu bản cập nhật mới gặp sự cố.  
