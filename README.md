Để tải một dự án Laravel từ GitHub về và chạy dự án, bạn có thể thực hiện các bước sau:

### 0. Tạo database:
Tại phpMyAdmin tạo database, tải file baocao.sql rồi import vào database.


### 1. Clone Repository từ GitHub:
git clone https://github.com/ohmygosh11/ecom_proj.git


### 2. Di chuyển vào Thư Mục Dự Án:
cd ten_thu_muc_project


### 3. Cài Đặt Các Gói PHP:
composer install


### 4. Sao Chép File `.env`:
cp .env.example .env


### 5. Tạo Key Ứng Dụng:
php artisan key:generate


### 6. Cấu Hình Database:
DB_CONNECTION=mysql

DB_HOST=127.0.0.1

DB_PORT=3306

DB_DATABASE=ten_database

DB_USERNAME=ten_nguoi_dung

DB_PASSWORD=mat_khau


### 7. Chạy Migrations:
php artisan migrate


### 8. Chạy Seeder (Nếu Có):
php artisan db:seed


### 9. Chạy Ứng Dụng Laravel:
php artisan serve

Sau đó, bạn có thể truy cập ứng dụng Laravel của mình tại `http://localhost:8000` trong trình duyệt web của bạn.


**Lưu ý**:
Bạn cần cài đặt Composer trước khi chạy các lệnh `composer install`. Để chạy ứng dụng Laravel, bạn cũng cần có một môi trường PHP và MySQL hoặc SQLite đã được cài đặt.
