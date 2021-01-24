# systemd-boot-tools
scripts to maintain systemd-boot

written and tested on ubuntu 20.04 LTS

ensure the scripts are executable, otherwise make them executable with chmod +x

disclaimer: u have 2 know what u do, i'm not responsibly for any damage on your machine

## zz-systemd-boot-update
place in _/etc/kernel/postinst.d/_, after a new kernel is installed this script is called and add the new kernel to the systemd-boot loader

## zz-systemd-boot-remover
place in _/etc/kernel/postrm.d/_, after a kernel was removed this script is called and removes the kernel from the systemd-boot loader

## systemd-boot-setup
run for installing systemd-boot and adding the current running kernel
