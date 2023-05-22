# Rtl8188eus
RTL8188EUS Driver installation in kali (TP-Link)
![image](https://github.com/bhanugoudm041/Rtl8188eus/assets/92798414/dc5be2c4-8290-4efe-9d13-a72cf880ac88)

sudo apt clean && apt update && apt upgrade && apt dist-upgrade

apt install gcc

sudo apt install bc

sudo rmmod r8188eu.ko

git clone https://github.com/aircrack-ng/rtl8188eus

cd rtl8188eus

sudo -i

echo "blacklist r8188eu.ko" > "/etc/modprobe.d/realtek.conf"

exit

make

sudo make install

sudo modprobe 8188eu

cd ~

nano .bashrc

sudo rmmod r8188eu.ko
