# tictac_and_my_flask
Tìm hiểu và chỉ ra sự khác biệt giữa mạng bridge mặc định và mạng bridge do người dùng tự tạo
1. Tên và ID: Mạng bridge mặc định có tên là bridge và có một ID duy nhất. Người dùng không thể tạo nhiều mạng bridge mặc định. Ngược lại, mạng bridge do người dùng tự tạo có thể được đặt tên theo mong muốn và có ID duy nhất cho mỗi mạng.
=> 1 cái là tên mạng duy nhất
=> 1 cái là tên mạng có thể custom

3. Sự Cách Ly:  Mạng bridge mặc định cách ly mạng cơ bản, có nghĩa là tất cả các container kết nối vào mạng bridge mặc định có thể giao tiếp với nhau. Mạng bridge do người dùng tự tạo mặc định là cách ly, nhưng người dùng có thể cấu hình để cho phép
hoặc ngăn chặn giao tiếp giữa các container trên cùng mạng.
=> 1 cái các container có thể giao tiếp với nhau nhưng không cấu hình hoặc ngăn chặn giao tiếp
=> 1 cái các container có thể giao tiếp với nhau nhưng có thể cấu hình hoặc ngăn chặn giao tiếp

5. Cấp Địa Chỉ IP: Mạng bridge mặc định sử dụng DHCP để cấp địa chỉ IP cho container, trong khi mạng bridge do người dùng tự tạo có thể được cấu hình để sử dụng DHCP hoặc các địa chỉ IP tĩnh được xác định trước.
=> 1 cái sử dụng DHCP để cấp IP address cho container
=> 1 cái sử dụng DHCP hoặc các IP Address Tĩnh để cấp IP address cho container

7. Port Mapping: Cả hai loại mạng bridge đều hỗ trợ port mapping (điều hướng cổng), cho phép bạn ánh xạ các cổng của container với các cổng trên máy chủ host. Điều này cho phép bạn truy cập các dịch vụ chạy trong container từ bên ngoài.
=> Cái này giống nhau

9. Tùy Chọn Cấu Hình: Mạng bridge do người dùng tự tạo cho phép bạn tùy chỉnh nhiều cài đặt như mạng mặc định, chẳng hạn như cấu hình địa chỉ IP, tắt hoặc bật DHCP, chặn hoặc cho phép giao tiếp giữa các container trên cùng mạng, và nhiều tùy chọn khác.
=> 1 cái để mặc định cấu hình
=> 1 cái có thể cấu hình TP, turn off/on DHCP, chặn hoặc cho phép giao tiếp trong cùng 1 mạng,...

11. Sự Linh Hoạt: Mạng bridge do người dùng tự tạo mang tính linh hoạt cao hơn và cho phép bạn tạo ra nhiều mạng bridge riêng biệt với các cài đặt và tính năng khác nhau để phù hợp với nhu cầu của ứng dụng cụ thể.
=> 1 cái để mạng chỉ 1 mạng
=> 1 cái có thể tạo ra nhiều mạng linh hoạt và riêng biệt theo từng nhu cầu
