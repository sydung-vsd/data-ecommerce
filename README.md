Các bước tiến hành deploy REST API với JSON Server lên Heroku
1 – Tạo một database

Clone repo sau về máy tính của bạn:

    git clone https://github.com/sydung-vsd/data-ecommerce

Sau đó thay db.json thành file json của bạn

2 - Tạo một repo trên github của bạn, và đẩy repo vừa được clone và thay thế đó lên repo mới tạo.

3 – Tạo một tài khoản https://heroku.com

4 – Cài đặt Heroku CLI vào máy tính của bạn https://devcenter.heroku.com/articles/heroku-cli

5 - Vào lại heroku và tạo một project, liên kết project đó với repo github của bạn. Rồi lấy link và sủ dụng

        ------------- Vậy là xong ------------

4 – Mở Terminal và gõ lệnh sau để kết nối Heroku CLI đến tài khoản của bạn đã tạo ra ở bước 2.

      heroku login

5 – Tạo một remote Heroku project, tương tự như tạo một git trên GitHub và đặt tên cho projec của bạn chẳng hạn như cgh-db

    heroku create cgh-db

6 – Push toàn bộ thư mục chứa file json lên Heroku

      git push heroku master

7 – Truy cập ứng dụng vừa được tạo bằng cách mở qua Heroku như sau:

    heroku open

8 – Nếu có lỗi xảy ra, ta có thể kiểm tra bằng cách sử dụng

heroku logs --tail


-----------Các bước deploy lên surge.sh----------- 
1 - Cài surge cho global.

    npm i -g surge 
2 - Chạy npm run build.

3 - Vào folder buil vừa được tạo ra.

    cd build
    
4 - Copy file index.html thêm một file khác, và đổi tên nó thành 200.html  (có để load khác page vẫn được)

5 - Deploy folder lên surge.sh

    surge
    
6 - Nhập email vào password đã dùng để đăng nhập trên surge.

7 - Chỉnh domain để dùng cho sau này.
