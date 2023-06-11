# Install_breedwed_Xiaomi_r3g
CÁC BƯỚC CƠ BẢN ĐỂ CÀI ĐẶT BOOTLOADER VÀ CẬP NHẬT FIRMWARE PADAVAN CHO ROUTER XIAOMI GEN 3G

Thời gian cập nhật bài viết: 22:27
Chủ Nhật, 11 tháng 6, 2023 (GMT+7)
![image](https://github.com/hienhoanghien2006/my_storage/assets/111626123/b8e09202-ea89-45c8-8605-feaf60f4733c)

This guide will cover how to flash

Xiaomi Mi Wifi Router 3G with English Padavan Firmware

Download the latest Xiaomi MI Wifi 3G Developer Firmware
Current version http://bigota.miwifi.com/xiaoqiang/rom/r3g/miwifi_r3g_firmware_12f97_2.25.124.bin

Flash developer firmware.

[​IMG]
[​IMG]

[​IMG]

Connect to router, default password 123456789

Connect to router wifi with your mobile phone.
Download Mi Wi-fi app.
Connect router to your Mi account.

On PC go to https://d.miwifi.com/rom/ssh

Connect with your Mi account

[​IMG]

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

[​IMG]


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
