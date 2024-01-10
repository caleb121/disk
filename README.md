# /dev/loop(虚拟块设备，替代某些文件如iso和img，让文件可以向磁盘一样被挂载)
losetup /dev/loop0 xxx.iso
mount /dev/loop0 /path/to/file

umount /dev/loop0
losetup -d /dev/loop0


# /dev/zram(虚拟块设备，利用swap技术将ram中不太需要的内存放到zram中压缩再返回给ram)

# /dev/ram(虚拟块设备)
