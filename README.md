# CÀI ĐẶT BOOTLOADER BREEDWED VÀ CẬP NHẬT FIRMWARE PADAVAN CHO ROUTER XIAOMI GEN 3G
CÁC BƯỚC CƠ BẢN ĐỂ CÀI ĐẶT BOOTLOADER BREEDWED VÀ CẬP NHẬT FIRMWARE PADAVAN CHO ROUTER XIAOMI GEN 3G

Thời gian cập nhật bài viết: 22:27
Chủ Nhật, 11 tháng 6, 2023 (GMT+7)
![image](https://github.com/hienhoanghien2006/my_storage/assets/111626123/b8e09202-ea89-45c8-8605-feaf60f4733c)

Trong bài viết này mình sẽ hướng dẫn các cách để cài đặt Bootloader Breedwed và cập nhật Firmware Padavan ngôn ngữ Tiếng Anh cho Router Xiaomi Mi Wifi Router 3G

1. ĐẦu tiên tải xuống  Firmware Xiaomi MI Wifi 3G danh cho nhà phát trển (Developer)
tại đây:
http://bigota.miwifi.com/xiaoqiang/rom/r3g/miwifi_r3g_firmware_12f97_2.25.124.bin

Sau khi Firmware được tải thành công tiến hành tiếp các bước như trong ảnh đưới đây để Flash Firmware developer.

![image](https://github.com/hienhoanghien2006/my_storage/assets/111626123/224c08ad-36bd-4769-8a71-f434e555337f)

![image](https://github.com/hienhoanghien2006/my_storage/assets/111626123/8ada752d-e492-4a5a-89f5-2c605083607e)

![image](https://github.com/hienhoanghien2006/my_storage/assets/111626123/6767091c-c7a1-4080-bcb1-e35c42759e35)

Kết nối với bộ định tuyến, mật khẩu mặc định 123456789

Kết nối với bộ định tuyến wifi bằng điện thoại di động của bạn.
Tải xuống ứng dụng Mi Wi-fi.
Kết nối bộ định tuyến với tài khoản Mi của bạn.

Trên PC, hãy truy cập https://d.miwifi.com/rom/ssh 

Kết nối với tài khoản Mi đã được kêt nối với bộ định tuyến qua app MI WIFI

![image](https://github.com/hienhoanghien2006/my_storage/assets/111626123/aafde009-de87-44fb-ba6a-67065d308d8a)

Tại đây bạn sẽ tìm thấy tên người dùng và mật khẩu đăng nhập SSH. Và tiến hành tải file ssh về máy tính của bạn.

Sau khi lưu thành công tệp "Miwifi_ssh.bin".
Kết nối USB với máy tính và định dạng Ổ USB thành FAT32. Sao chép tệp "Miwifi_ssh.bin" đến ổ flash USB FAR32

Tắt nguồn bộ định tuyến của bạn bằng việc nguồn điện.
Gắn USB với bộ định tuyến thông qua cổng USB phía sau bộ định tuyến.
Giữ nút đặt lại.Và cắm lại nguồn cho đến khi đèn LED màu cam bắt đầu nhấp nháy, nhả nút đặt lại.

Đợi đèn LED màu xanh sáng liên tục.

Tải xuống BOOTLOADER BREEDWED breed-mt7621-xiaomi-r3g.bin tại địa chỉ https://breed.hackpascal.net/

Sao chép tệp "breed-mt7621-xiaomi-r3g.bin" đến ổ USB.

Tải về phần mềm PUTY và mở nó
https://www.putty.org

Kết nối SSH đến router với địa chỉ IP 192.168.31.1 

![33791961228_7d94e6f437_o](https://github.com/hienhoanghien2006/my_storage/assets/111626123/56380ebd-1a9c-4bf8-a72a-e8d83b89cace)

Dán đoạn code bên dưới vào trình SSH của PUTTY
```
 mtd write /extdisks/sda1/breed-mt7621-xiaomi-r3g.bin Bootloader
```
Tắt nguồn bộ định tuyến của bạn bằng việc nguồn điện.

Kết nối Cổng WAN đến cổng LAN Của Máy tính

Nhấn giữ reset, cắm nguồn, đợi LED nháy, nhả reset.

Dùng trình duyệt trên máy tính của bạn truy cập địa chỉ 192.168.1.1

[​IMG]


Như vậy đã hoàn thành việc cài đặt BOOTLOADER BREEDWED 
Choose flash ROM and select file MI-R3G_3.4.3.9L-100[56960f9][12-04-2019_18-08].trx

[​IMG]

Click ok.

Connect to Asus Wifi, password 1234567890

Go 192.168.1.1 login admin admin

Enjoy new firmware and features!
FTP, UPnP/DLNA Media Server, NAS, torrents and much more with your new Xiaomi Mi Router 3G and Padavan firmware!

[​IMG]
