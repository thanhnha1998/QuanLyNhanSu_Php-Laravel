<p align="center"><img src="https://camo.githubusercontent.com/5ceadc94fd40688144b193fd8ece2b805d79ca9b/68747470733a2f2f6c61726176656c2e636f6d2f6173736574732f696d672f636f6d706f6e656e74732f6c6f676f2d6c61726176656c2e737667" width="400"></p>

<p align="center">
<a href="https://travis-ci.org/laravel/framework"><img src="https://travis-ci.org/laravel/framework.svg" alt="Build Status"></a>
<a href="https://packagist.org/packages/laravel/framework"><img src="https://poser.pugx.org/laravel/framework/d/total.svg" alt="Total Downloads"></a>
<a href="https://packagist.org/packages/laravel/framework"><img src="https://poser.pugx.org/laravel/framework/v/stable.svg" alt="Latest Stable Version"></a>
<a href="https://packagist.org/packages/laravel/framework"><img src="https://poser.pugx.org/laravel/framework/license.svg" alt="License"></a>
</p>

## Giới thiệu

Đây là ứng dụng quản lý nhân sự, quản lý lương được xây dựng bằng Laravel framework.

## Hướng dẫn cài đặt sau khi clone source code từ github về:

Tại phpmyadmin tiến hành thêm một database mới. Import database vào mysql. Database được lưu trữ trong folder Database của project. Mở thư mục project vừa clone, mở command prompt từ thư mục và chạy lệnh theo thứ tự sau:
- composer install
- composer update
- cp .env example .env
- php artisan config:clear
- php artisan cache:clear
- php artisan key:generate

Sau khi chạy xong, mở file .env lên và thay đổi DB_DATABASE=laravel thành DB_DATABASE "database vừa thêm".
Ở phần MAIL cũng tiến hành thay đổi nội dung như sau:
- MAIL_DRIVER=smtp
- MAIL_HOST=smtp.gmail.com <đây là server của gmail>
- MAIL_PORT=587
- MAIL_USERNAME="tên mail dùng để gửi mật khẩu tài khoản"
- MAIL_PASSWORD="password của mail"
- MAIL_ENCRYPTION=tls

Để truy cập vào trang đăng nhập tài khoản, nhập đường dẫn như sau: domain/private hoặc domain/login

- Tài khoản admin: admin@gmail.com
- Password: 123456


## Tính năng

- Quản lý nhân sự (Thông tin cá nhân, hồ sơ, hợp đồng, quyết định, bảo hiểm, chức vụ...).
- Quản lý các ý kiến, đề xuất từ các nhân viên trong công ty.
- Quản lý lương, thuế của nhân viên.
- In nhanh hợp đồng lao động, quyết định, ý kiến...
- Phân quyền quản lý người dùng.
- Cấu hình thông tin công ty.
- Giới thiệu tin tức, tuyển dụng công ty.
...

## Contributing

Thank you for considering contributing to the Laravel framework! The contribution guide can be found in the [Laravel documentation](https://laravel.com/docs/contributions).

## Security Vulnerabilities

If you discover a security vulnerability within Laravel, please send an e-mail to Taylor Otwell via [taylor@laravel.com](mailto:taylor@laravel.com). All security vulnerabilities will be promptly addressed.

## License

The Laravel framework is open-source software licensed under the [MIT license](https://opensource.org/licenses/MIT).
