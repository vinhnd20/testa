Bước 1: Chuẩn bị môi trường
1. Cài đặt Git:
Tải và cài đặt Git từ https://git-scm.com/.
2. Cài đặt Python:
Tải và cài đặt Python từ https://www.python.org/downloads/.
3. Cài đặt Pip:
Nếu chưa cài đặt, có thể cài đặt Pip từ https://pip.pypa.io/en/stable/installing/.
1. Cài đặt và cấu hình Visual Studio Code:
Tải và cài đặt Visual Studio Code (VS Code) từ https://code.visualstudio.com/.
Cài đặt extension Python cho VS Code qua Marketplace.

Bước 2: Tạo môi trường ảo và clone dự án
1. Tạo Folder:
Tạo một folder trên máy tính để lưu trữ dự án.
2. Mở VS Code và Terminal:
Mở VS Code và mở terminal tích hợp (sử dụng phím tắt `Ctrl + ``).
3. Tạo môi trường ảo:
- Để tạo môi trường ảo, dùng lệnh sau trong terminal của VS Code:
    python -m venv venv  # Hoặc python3 -m venv venv cho macOS
- Kích hoạt môi trường ảo:
    + Windows: .\venv\Scripts\activate
    + macOS: source venv/bin/activate
4. Clone dự án:
- Clone dự án bằng lệnh:
    git clone https://github.com/vijaythapa333/django-student-management-system.git
- Sau đó, di chuyển vào thư mục dự án:
    cd django-student-management-system

Bước 3: Cài đặt các thư viện và chạy dự án
1. Cài đặt các thư viện:
- Cài đặt các thư viện cần thiết bằng cách chạy lệnh:
    pip install -r requirements.txt
2. Chỉnh sửa settings.py:
- Mở file settings.py và thêm '*' vào ALLOWED_HOSTS nếu chưa có:
    ALLOWED_HOSTS = ['*']
3. Chạy server:
- Chạy server Django bằng lệnh:
    python manage.py runserver  # Hoặc python3 manage.py runserver cho macOS
4. Tạo Super User:
- Tạo super user để đăng nhập vào trang quản trị:
    python manage.py createsuperuser
5. Truy cập dự án:
    Mở trình duyệt và truy cập http://localhost:8000 để xem dự án.

**6. Login Credentials**

Create Super User (HOD)
```
$  python manage.py createsuperuser
```
Then Add Email, Username and Password

**or Use Default Credentials**

*For HOD /SuperAdmin*
Email: admin@gmail.com
Password: admin

*For Staff*
Email: staff@gmail.com
Password: staff

*For Student*
Email: student@gmail.com
Password: student
