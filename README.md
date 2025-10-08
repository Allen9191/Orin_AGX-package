# Reinstallation of Orin_AGX / Orin_NANO 
##Before Flashing Machine
[NVIDIA Jetson AGX Orin 安裝 JetPack 6.0 正式版](https://blog.cavedu.com/2024/08/10/jetson-agx-orin-jp6-install/)
Force Recovery button 按住進入Recovery Mode模式，按著接電源，不然電腦供電可能會不足
然後再按開機鍵(Force Recovery button不能放)
##First Open
linux setting

>sudo apt update

>sudo apt upgrade

check vim

install Chroium-browser
>At aarch64 snap version:
>[Chromium, other browsers not working after flashing or updating](https://forums.developer.nvidia.com/t/chromium-other-browsers-not-working-after-flashing-or-updating-heres-why-and-quick-fix/338891)

>sudo apt-get install chromium-browser

##Install jtop
>[jetson-stats](https://rnext.it/jetson_stats/)

>reboot

##Solve jetpack missing & openCV version problem
jetpack missing
>[Jtop fix to show Jetpack 6.2.1](https://forums.developer.nvidia.com/t/jtop-fix-to-show-jetpack-6-2-1/339404/1)

>" /usr/local/lib/python3.10/dist-packages/jtop/core/"

>sudo vim jetson_variables.py

>reboot

OpenCV: 4.8.0 with CUDA: NO
>github [AastaNV/JEP](https://github.com/AastaNV/JEP/blob/master/script/install_opencv4.10.0_Jetpack6.1.sh)

>Download this file"JEP/script/install_opencv4.10.0_Jetpack6.1.sh"

>chmod +x install_opencv4.10.0_Jetpack6.1.sh

>./install_opencv4.10.0_Jetpack6.1.sh
確定要移除原本的OpenCV, yes




