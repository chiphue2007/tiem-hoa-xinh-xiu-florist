TIỆM HOA XINH XÍU FLORIST — BẢN CẤU HÌNH CHO TIỆM
Địa chỉ: 763 Nguyễn Công Trứ, Hoa Lư, Ninh Bình
Zalo: 0342884938

TRIỂN KHAI NETLIFY (KHUYẾN NGHỊ GITHUB)
1. Giải nén ZIP; tạo repository GitHub riêng tư và upload toàn bộ các file, giữ nguyên thư mục netlify/functions.
2. Vào https://app.netlify.com/ > Add new project > Import an existing project > GitHub; chọn repository.
3. Build command: npm install (hoặc để Netlify tự cài dependencies); Publish directory: . ; Functions directory: netlify/functions (đã khai báo trong netlify.toml).
4. Trong Netlify > Project configuration > Environment variables, thêm:
   ZALO_PHONE = 0342884938
   ADMIN_PASSWORD = [MẬT KHẨU MẠNH TỰ CHỌN]
   Không ghi mật khẩu vào file mã nguồn, không chia sẻ mật khẩu.
5. Deploy lại sau khi thêm biến môi trường. Mở URL Netlify của dự án.
6. Khách đặt hoa tại / ; quản lý tại /admin.html. Kiểm tra tạo đơn, mở Zalo, đăng nhập quản trị và cập nhật trạng thái.

LƯU Ý
- Chưa triển khai trên tài khoản Netlify của bạn; cần bạn tự đăng nhập và cấu hình.
- Mẫu hoa, giá và biểu tượng là DEMO. Khi thay sản phẩm/giá phải cập nhật cả index.html và catalog trong netlify/functions/orders.mjs.
- Đơn được lưu bằng Netlify Blobs thông qua Netlify Functions; chỉ hoạt động sau khi deploy đúng cấu hình, không chạy bằng cách mở file HTML trực tiếp.
- Nút Zalo mở hội thoại và có nút sao chép nội dung đơn; khách tự dán/gửi, không tự động nhắn tin.
- Phí giao hàng chưa được tính vào tổng. Chưa có thanh toán online, thông báo tự động hay chống spam nâng cao.
- Trước khi nhận đơn thật, thử nghiệm lưu và tải lại đơn trong trang admin; kiểm tra quyền riêng tư, giới hạn sử dụng và chi phí Netlify.
