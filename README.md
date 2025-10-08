# Reinstallation of Orin_AGX / Orin_Nano 
## Before Flashing Machine (This part JUST for Orin_AGX!)
### Warning: Please follow the instructions below STEP BY STEP.
[NVIDIA Jetson AGX Orin 安裝 JetPack 6.0 正式版](https://blog.cavedu.com/2024/08/10/jetson-agx-orin-jp6-install/)

## Steps from now on ALSO work on Orin_Nano.

After start up, then open terminal and follow those commands.
>sudo apt update

>sudo apt upgrade

If you discover there is no vim, then
>sudo apt install vim

### Debug Chromium Web Browser

If you find there is a problem when opening Chromium, follow the instruction and command.

At aarch64 snap version:
[Chromium, other browsers not working after flashing or updating](https://forums.developer.nvidia.com/t/chromium-other-browsers-not-working-after-flashing-or-updating-heres-why-and-quick-fix/338891)

>sudo apt-get install chromium-browser

### Install jtop

Follow the instruction and command.

[jetson-stats](https://rnext.it/jetson_stats/)

>reboot

### Solve Jetpack MISSING & OpenCV 4.XX.X with CUDA: NO

Open terminal and enter jtop, and go to see INFO if you discover two problems as title. Please follow those instructions or commands.

[Jtop fix to show Jetpack 6.2.1](https://forums.developer.nvidia.com/t/jtop-fix-to-show-jetpack-6-2-1/339404/1)

>" /usr/local/lib/python3.10/dist-packages/jtop/core/"

>sudo vim jetson_variables.py

>reboot

OpenCV: 4.8.0 with CUDA: NO
>github [AastaNV/JEP](https://github.com/AastaNV/JEP/blob/master/script/install_opencv4.10.0_Jetpack6.1.sh)

>Download this file"JEP/script/install_opencv4.10.0_Jetpack6.1.sh"

>chmod +x install_opencv4.10.0_Jetpack6.1.sh

>./install_opencv4.10.0_Jetpack6.1.sh
確定要移除原本的OpenCV, yes




