# PhatTrienUngDungWeb
<h1>Cách chạy project:</h1>
<h3>Nếu mới tải project lần đầu thì copy file env.example đổi tên thành env và sửa tên database lại đúng tên</h3>
Các câu lệnh reset và update version: </br>
- composer update</br>
- php artisan cache:clear</br>
- php artisan config:clear</br>
Tạo khoá:</br>
- php artisan key:generate</br>
Chạy đồ án:</br>
- php artisan serve</br>
Các chức năng cần chạy lệnh:</br>
+ Gửi mail:</br>
sửa các thông tin lại (file env): </br>
MAIL_MAILER=smtp</br>
MAIL_HOST=smtp.gmail.com</br>
MAIL_PORT=587</br>
MAIL_USERNAME= //Mail address</br>
MAIL_PASSWORD=(Pass lấy từ google (Bật xác minh 2 bước) trong phần bảo mật -> mật khẩu ứng dụng -> chọn Thư và Hệ điều hành)</br>
MAIL_ENCRYPTION=tls</br>
MAIL_FROM_ADDRESS= //Mail address</br>
MAIL_FROM_NAME="${APP_NAME}"</br>

- php artisan que:work (1 terminal riêng) // Gửi mail thì phải chạy lệnh này</br>
- sửa nhiều trong mail thì composer dump-autoload (tạo các fail job và job mail)</br>
- khởi tạo laị các table php artisan migrate</br>
