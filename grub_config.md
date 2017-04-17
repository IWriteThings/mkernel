copy the kernel to /boot/

Edit /boot/grub2/grub.cfg

add -

```
menuentry 'myKernel' {
  set root='(hd0,msdos1)'
  multiboot /kern-701 ro
}

reboot and select kernel
