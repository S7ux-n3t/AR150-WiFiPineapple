# AR-150 WiFi Pineapple NANO

Converting your AR-150 to a WiFi Pineapple NANO should be an easy process. However, the web & git is full of broken bin images and botched firmware builders... resulting in a broken or partially-working firmware. The latest working build available elsewhere is 2.4.2. Here, we start with version 2.5.4.
This version is almost 100% equal of the original hardware.

Summary for 2.7.x:
1. Rootfs 1M (mini 1.2M)
2. PineAP(d) working.
3. Drivers for: kmod-rt2800, kmod-rtl8187 and others
4. Kernel 4.14.171 (OpenWrt 19.02.2)
5. Fix LAN and WAN ports. No more swapped ports.
6. Use pendrive like original SD.

Recomended setup
1. USB 2.0 2 ports hub https://www.ebay.co.uk/itm/USB-2-0-2-Dual-Port-Hub-For-Laptop-Macbook-Notebook-PC-Mouse-Flash-Disk/273070654192
2. Generic RT5370 adapter
3. Please support Hak5 work and buy the original hardware

Notes:
1. For format jffs2 (overlayFS) use jffs2reset command.
2. If you are stuck at the message "The WiFi Pineapple is still booting" don't panic, this is a known issue with running the WiFi Pineapple firmware on the AR150. Executing the command jffs2reset -y && reboot should resolve your problems. 
3. For generate a custom build use this toolset https://github.com/xchwarze/wifi-pineapple-cloner


### If you want to collaborate with hardware 

To develop the next versions of this project I need:

For TETRA clone project:
https://www.gl-inet.com/products/gl-ar750s/#specs

For "WiFi Pineapple Mark 6.5" project:
https://www.gl-inet.com/products/gl-mt1300/#specs
