# datn

Các bước cài đặt
Bước 1: Đầu tiên, lấy source code từ Git Repository, sau đó chạy các lệnh:
•	cd/path/to/foldercode
•	composer i
•	cp .env.example .env
•	php artisan key:generate 
Bước 2: Setup liên kết với database, gán dòng sau vào file .env vừa copy từ bước 1. 
DB_CONNECTION=mysql
DB_HOST=127.0.0.1
DB_PORT=3306
DB_DATABASE=dbname
DB_USERNAME=root
DB_PASSWORD=
Bước 3: Chạy các câu lệnh:
•	php artisan migrate.
•	php artisan passport:install.
•	php artisan db:seed…
Bước 4: Setup APP_NAME, gán các dòng sau vào file .env:
•	APP_NAME=weblinhkien.
•	MAIL_PREFIX_SUBJECT=[Shopping Mail].
Bước 5: Cài đặt OAuth2 với passport laravel bằng câu lệnh:
•	php artisan passport:install .
Bước 6: Sau khi cài đặt, ứng dụng sẽ khởi động trên server ảo là 127.0.0.1:8000 hoặc khởi động với hostname mặc định là “localhost”.
