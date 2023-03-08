# PhatTrienUngDungWeb
<h1>Cách chạy project:</h1>
<h3>Nếu mới tải project lần đầu thì copy file env.example đổi tên thành env và sửa tên database lại đúng tên</h3>
Các câu lệnh reset và update version:
- composer update
- php artisan cache:clear
- php artisan config:clear
Tạo khoá:
- php artisan key:generate
Chạy đồ án:
- php artisan serve
Các chức năng cần chạy lệnh:
+ Gửi mail:
sửa các thông tin lại (file env): 
MAIL_MAILER=smtp
MAIL_HOST=smtp.gmail.com
MAIL_PORT=587
MAIL_USERNAME= //Mail address
MAIL_PASSWORD=(Pass lấy từ google (Bật xác minh 2 bước) trong phần bảo mật -> mật khẩu ứng dụng -> chọn Thư và Hệ điều hành)
MAIL_ENCRYPTION=tls
MAIL_FROM_ADDRESS= //Mail address
MAIL_FROM_NAME="${APP_NAME}"

- php artisan que:work (1 terminal riêng) // Gửi mail thì phải chạy lệnh này
- sửa nhiều trong mail thì composer dump-autoload (tạo các fail job và job mail)
- khởi tạo laị các table php artisan migrate
