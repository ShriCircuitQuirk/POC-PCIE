# POC-PCIE


dmesg from jetson development kit:

pcie@ubuntu:~$ sudo su -
[sudo] password for pcie: 
root@ubuntu:~# dmesg | grep DTS
[    0.007436] DTS File Name: /dvs/git/dirty/git-master_linux/kernel/kernel-5.10/arch/arm64/boot/dts/../../../../../../hardware/nvidia/platform/t19x/jakku/kernel-dts/tegra194-p3668-0001-p3509-0000.dts
root@ubuntu:~# 

Install FDT viewer -> need docker for this

https://stackoverflow.com/questions/14000736/tool-to-visualize-the-device-tree-file-dtb-used-by-the-linux-kernel
https://github.com/dev-0x7C6/fdt-viewer

-------------------------------------------------------------------

Install docker

https://docs.docker.com/engine/install/ubuntu/

-------------------------------------------------------------------

Install from link-nvidia

https://forums.developer.nvidia.com/t/how-to-compile-jetpack3-0-kernel-device-tree-file-the-kernel-device-tree-which-one-is-used/55128
https://kernel.googlesource.com/pub/scm/utils/dtc/dtc.git
https://www.howtoinstall.me/ubuntu/18-04/device-tree-compiler/

-----------------------------------------------------------------------------------------------------------------------------
Custom dtb

https://forums.developer.nvidia.com/t/merge-our-custom-device-tree-dts-file-and-jetson-io-created-device-tree-file/182758

-----------------------------------------------------------------------------------------------------------------------------------

Device tree compiler

https://siliconbladeconsultants.com/2022/05/26/decompiling-the-linux-device-tree-dtb/


