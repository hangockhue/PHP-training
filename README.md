# PHP-training Write-up 

## 1. Các kiến thức cơ bản về PHP
4 thành phần tạo nên 1 trang web động là 1 web server(apache) , 1 ngôn ngữ kịch bản trên máy chủ ( server-side scritipting language : PHP , ASP , ASP.NET ..) , 1 hệ quảng trị cơ sở dữ liệu , 1 ngôn ngữ phía máy khách ( java scrip)

Sự khác biệt giữa PHP và Javascrip 

PHP ngôn ngữ chạy trên máy chủ

Javascip là ngôn ngữ chạy trêm máy khách

PHP có thể giao tiếp với database còn javascrip thì không

Javascrip có thể xóa các thẻ trong html một cách thuận lời còn php thì không 

Nếu gặp 1 bug trong một mã nguồn mở thì bạn có thể fix nhờ nhà phát hành 

## 2. Cách nhúng php vào một file HTML

Ta chỉ cần đánh dấu vùng nhập code PHP bằng <?php   ?> rồi sau đó nhập code vào trong đó 

Mục đích của chương trình FTP giúp kết nối giữa máy khách và máy chủ như update hay download ...

Cách kết nối database với php

Để kết nối database ta sẽ dùng hàm mysqli_connect với cấu trúc sau

`mysqli_connect($host,$user,$password,$database,$port,$socket).`

Trong đó 

`      $host là địa chỉ host của bạn

       $user và $password là tên đăng nhập và mật khẩu kết nối vào database

       $database là tên database bạn chọn để sử lý

       $port là cổng kết nối 

       $socket phương thức socket kết nối
 `

Ví dụ 

`$ketnoi = mysqli_connect('localhost','ngockhue','ngockhue123','demo') or die ('Không thể kết nối tới database')`
tất cả các tham số đó thì ta chỉ cần quan tâm đến 4 tham số đầu tiên 2 tham số còn lại không cần truyền vào . Còn đoạn code or die nghĩa là nếu không thể kết nối với database thì nó sẽ in ra màn hình thông báo đó 



