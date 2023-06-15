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

Connect to router, default password 123456789

Connect to router wifi with your mobile phone.
Download Mi Wi-fi app.
Connect router to your Mi account.

On PC go to https://d.miwifi.com/rom/ssh

Connect with your Mi account

![image](https://github.com/hienhoanghien2006/my_storage/assets/111626123/aafde009-de87-44fb-ba6a-67065d308d8a)

Where you will find SSH login username and password.

And SSH download. Click button, fix address with https://

Save Miwifi_ssh.bin file.

Format USB flash drive to Fat32

Copy Miwifi_ssh.bin file to the flash drive.

Turn off power on your router.
Stick USB drive.
Hold reset button.
And plug power back in till orange LED starts to blink, release reset button.

Wait blue LED to light solid.

Download breed-mt7621-xiaomi-r3g.bin from https://breed.hackpascal.net/

Copy file to the USB flash drive and plug to router.

Download and open putty
https://www.putty.org

Connect to the router 192.168.31.1

![33791961228_7d94e6f437_o](https://github.com/hienhoanghien2006/my_storage/assets/111626123/56380ebd-1a9c-4bf8-a72a-e8d83b89cace)

Write mount
```
 mtd write /extdisks/sda1/breed-mt7621-xiaomi-r3g.bin Bootloader
```
Disconnect router from power.

Connect WAN port to LAN on PC

Hold reset, plug power, wait for LED to flash, release reset

Go 192.168.1.1

[​IMG]

Choose flash ROM and select file MI-R3G_3.4.3.9L-100[56960f9][12-04-2019_18-08].trx

[​IMG]

Click ok.

Connect to Asus Wifi, password 1234567890

Go 192.168.1.1 login admin admin

Enjoy new firmware and features!
FTP, UPnP/DLNA Media Server, NAS, torrents and much more with your new Xiaomi Mi Router 3G and Padavan firmware!

[​IMG]
