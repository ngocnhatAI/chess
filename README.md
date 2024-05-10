# How to run a local server ?
Open new terminal in VScode, run two commands below:
'pip install -r requirements.txt'
'python manage.py runserver'


# Cấu trúc cơ bản của web
ChessWeb/chessWeb là file quản lí và deploy web

Folder 'static' chứa các file tĩnh như ảnh hoặc css, javascript files, trong đó chess.js là quan trọng nhất chứa hầu hết logic của bàn cờ và sử dụng ajax để truyền và nhận dữ liệu từ giao diện web qua thuật toán thông qua users/views.py

users có những file quan trọng cần lưu ý gồm : 
- users/templates chứa file html tạo các đối tượng cho web và chỉnh sửa 
- users/views.py : dùng để giao tiếp (truyền và nhận dữ liệu) giữa phần giao diện và thuật toán python
- users/urls.py : Import các hàm từ views.py vào để thực thi
- users/montecarlotree.py : Chứa thuật toán MCTS
- users/algorithms.py : Chứa thuật toán Alpha Beta

Ngoài ra còn những file khác cần thiết để cài đặt một dự án django web app hoàn chỉnh nhưng phía trên là hầu hết những gì quan trọng
