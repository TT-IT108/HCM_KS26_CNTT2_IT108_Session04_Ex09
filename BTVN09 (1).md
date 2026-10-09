**Bài 9: Xử lý sự cố bảo mật file trên Server OrderTech bằng Terminal** 

**Bước 1 – Xác định vị trí:**

pwd

→ Kiểm tra đang đứng ở thư mục nào.

**Bước 2 – Xác nhận sự cố:**

ls .\\public

→ Kiểm tra db\_password.txt và hacker\_log.bat.

**Bước 3 – Tạo thư mục và di chuyển file:**

mkdir .\\secrets  
move .\\public\\db\_password.txt .\\secrets\\

→ Tạo secrets trước để tránh bị hiểu nhầm là đổi tên file, sau đó chuyển db\_password.txt vào đó.

**Bước 4 – Xóa file mã độc:**

del .\\public\\hacker\_log.bat

→ Xóa hacker\_log.bat khỏi thư mục public.

