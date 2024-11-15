<h2 align="center">Food Website 🍲</h2>

## Giới thiệu
- **Đây là một website bán thực phẩm trực tuyến được xây dựng bằng PHP. Website cho phép người dùng tìm kiếm, xem thông tin chi tiết các món ăn, và đặt hàng. Với giao diện thân thiện và dễ sử dụng, website "Food" là nền tảng lý tưởng để người dùng trải nghiệm mua sắm trực tuyến các sản phẩm thực phẩm**

## Chức năng
- **Trang chủ: Hiển thị danh sách các món ăn phổ biến và các danh mục.** 
- **Đăng ký / Đăng nhập: Người dùng có thể tạo tài khoản và đăng nhập để sử dụng các tính năng nâng cao.**
- **Xem chi tiết sản phẩm: Xem mô tả, giá và hình ảnh của từng sản phẩm**
- **Giỏ hàng: Thêm, sửa và xóa sản phẩm trong giỏ hàng**
- **Thanh toán: Thanh toán đơn hàng trực tuyến.**
- **Quản lý đơn hàng: Người dùng có thể theo dõi trạng thái đơn hàng của mình**

## Cài đặt
Yêu cầu hệ thống
- **XAMPP hoặc WAMP (Chạy PHP và MySQL)**
- **PHP (Phiên bản >= 7.4)**
- **MySQL (Phiên bản >= 5.6)**

## Các bước cài đặt
Clone repository này về máy:

git clone https://github.com/ThaiDinhHuu/Food_Project_PHP.git
Di chuyển vào thư mục project và sao chép toàn bộ vào thư mục htdocs của XAMPP (hoặc www của WAMP):

cd Food_Project_PHP
Khởi động Apache và MySQL thông qua XAMPP hoặc WAMP.

Tạo một database mới với tên là food_db và import file SQL có sẵn (nếu có) vào database:

CREATE DATABASE food_db;
Sau đó, import dữ liệu vào food_db bằng cách sử dụng phpMyAdmin hoặc chạy file .sql qua dòng lệnh.

Cấu hình thông tin kết nối database trong file connect.php:

<?php
$db = new PDO('mysql:host=localhost;dbname=food_db', 'root', '');
?>
Mở trình duyệt và truy cập vào http://localhost/Food_Project_PHP để bắt đầu sử dụng website.

Cấu trúc thư mục
admin/: Chứa các trang và chức năng quản lý cho admin.
components/: Chứa các file kết nối và xử lý chung.
css/: Chứa các file CSS để định dạng giao diện.
images/: Chứa hình ảnh sử dụng trên website.
js/: Chứa các file JavaScript để tương tác với giao diện.
uploaded_img/: Chứa các hình ảnh tải lên từ người dùng.
index.php: Trang chính của website.
about.php: Trang giới thiệu về website.
cart.php: Trang giỏ hàng.

Công nghệ sử dụng
PHP: Xử lý phía server.
MySQL: Lưu trữ dữ liệu người dùng, sản phẩm và đơn hàng.
HTML/CSS: Xây dựng giao diện người dùng.
JavaScript: Tạo các hiệu ứng và xử lý các sự kiện trên trang web.
