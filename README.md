# How-to-change-domain-loclhost-127.0.0.1-8000-into-another-virtual-domain
Mặc định khi các bạn cài XAMPP muốn truy cập vào host ảo của mình thì phải gõ http://localhost hoặc nếu đổi Port thì http://localhost:8080... Không phải ai cũng thích chữ localhost này, có nhiều bạn thích một cái gì đó của riêng bạn chẳng hạn chúng tôi muốn truy cập vào trang web của mình là blogtipstop.com thay vì http://localhost.

Vấn đề này không phải riêng ai mà hầu hết tất cả điều muốn như vậy, nắm được điều này chúng tôi sẽ hướng dẫn cho bạn cách thay đổi tên miền `localhost` thành một tên miền bất kỳ mà bạn thích.

Bước đầu tiên thực hiện thay đổi các bạn vào đường dẫn thư mục chứa tập tin host của hệ thống window như sau: ` C:\Windows\System32\drivers\etc `. Truy cập vào thư mục trên bạn sẽ thấy một tập tin có tên là `hosts`.

Tiếp theo, các bạn `click chuột phải vào tập tin hosts` chọn `Properties` một của sổ sẽ hiện lên các bạn chọn sang `Tab Security`.

Tiếp theo, `click chọn xuống phần Users ở cuối (Dưới cái Administrator) và chọn Edit`, `phần tên Users này mỗi máy sẽ khác nhau tùy thuộc vào bạn đổi tên gì hoặc hệ thống để mặc định`.

Một `cửa sổ mới hiện lên` các bạn cũng `chọn xuống phần Users cuối cùng tích hết vào ô Allow và lưu lại`.

Bây giờ `quay lại tập tin hosts trong thư mục bạn hãy mở nó ra bằng trình soạn thảo bất kỳ`, trỏ tên miền ảo cần thêm về `IP của localhost là 127.0.0.1`. 

ví dụ : 127.0.0.1   blogtipstop.com

`Thêm xong các bạn lưu file lại và đừng quên khởi động lại Apache` nếu không mọi thao tác trên sẽ không có hiệu lực.


Bây giờ chúng tôi sẽ mở trình duyệt truy cập vào tên miền mới của mình blogtipstop.com, do ở bài trước chúng tôi đã đổi Port Apache sang 8080 nên sẽ có thêm :8080 ở phía sau :D, nếu các bạn sử dụng Port 80 mặc định sẽ không hiển thị phần này.
