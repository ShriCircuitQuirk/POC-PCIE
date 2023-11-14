# POC-PCIE

https://forums.developer.nvidia.com/t/jetson-agx-orin-uefi-test/232846/2
https://developer.nvidia.com/blog/customize-your-own-carrier-board-with-nvidia-sdk-manager/
https://forums.developer.nvidia.com/t/hdmi-output-not-working/170047/43
https://docs.nvidia.com/jetson/archives/r35.4.1/DeveloperGuide/text/SD/Bootloader/UEFI.html#grub-support
https://www.ibm.com/docs/pl/aix/7.1?topic=tree-root-file-system
https://www.freecodecamp.org/news/how-to-set-an-environment-variable-in-linux/
https://www.scaler.com/topics/how-to-login-as-a-root-user-in-linux/
https://www.wikihow.com/Become-Root-in-Linux
https://github.com/fivdi/onoff/issues/62
https://docs.nvidia.com/jetson/archives/r35.4.1/DeveloperGuide/text/SD/Bootloader/UEFI.html#customizing-the-default-boot-order-in-the-configuration-file
https://stackoverflow.com/questions/14000736/tool-to-visualize-the-device-tree-file-dtb-used-by-the-linux-kernel

**Nvidia ticket:**
https://forums.developer.nvidia.com/t/jetson-xavier-carrier-board-hdmi-issue/271551/17

------------------------------------------------------------------------------------
uhj2kor@BANI-C-00428:~/Flash_Jetson_temp$ fdtdump tegra194-p3668-0000-p3509-0000.dtb > /tmp/test.txt 

fdtdump is a low-level debugging tool, not meant for general use.
If you want to decompile a dtb, you probably want
dtc -I dtb -O dts <filename>
------------------------------------------------------------------------------------
Install FDT viewer -> need docker for this

https://stackoverflow.com/questions/14000736/tool-to-visualize-the-device-tree-file-dtb-used-by-the-linux-kernel
https://github.com/dev-0x7C6/fdt-viewer
------------------------------------------------------------------------------------
Install docker

https://docs.docker.com/engine/install/ubuntu/
------------------------------------------------------------------------------------
Install from link-nvidia

https://forums.developer.nvidia.com/t/how-to-compile-jetpack3-0-kernel-device-tree-file-the-kernel-device-tree-which-one-is-used/55128
https://kernel.googlesource.com/pub/scm/utils/dtc/dtc.git
https://www.howtoinstall.me/ubuntu/18-04/device-tree-compiler/
------------------------------------------------------------------------------------
Custom dtb

https://forums.developer.nvidia.com/t/merge-our-custom-device-tree-dts-file-and-jetson-io-created-device-tree-file/182758
------------------------------------------------------------------------------------
Device tree compiler

https://siliconbladeconsultants.com/2022/05/26/decompiling-the-linux-device-tree-dtb/
------------------------------------------------------------------------------------
**dmesg from jetson development kit:**

pcie@ubuntu:~$ sudo su -
[sudo] password for pcie: 
root@ubuntu:~# dmesg | grep DTS
[    0.007436] DTS File Name: /dvs/git/dirty/git-master_linux/kernel/kernel-5.10/arch/arm64/boot/dts/../../../../../../hardware/nvidia/platform/t19x/jakku/kernel-dts/tegra194-p3668-0001-p3509-0000.dts
--------------------------------------------------------------------------------------
