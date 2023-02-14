В уроке надо сделать любое задание на выбор, напрмер свою вариацию команды lsof

```
[root@otusproc ~]# find /proc/[0-9]*/fd -type l -exec ls -la {} \;
```
что даст вооооот такой вывод всех запущенных в системе процессов (система ничем не нагружена, так что процессы легковесные

<details>
  <summary>Вывод</summary>
  
```
lrwx------. 1 root root 64 Feb 14 10:01 /proc/1/fd/0 -> /dev/null
lrwx------. 1 root root 64 Feb 14 10:01 /proc/1/fd/1 -> /dev/null
lrwx------. 1 root root 64 Feb 14 10:01 /proc/1/fd/2 -> /dev/null
lrwx------. 1 root root 64 Feb 14 10:01 /proc/1/fd/3 -> anon_inode:[timerfd]
lrwx------. 1 root root 64 Feb 14 10:03 /proc/1/fd/4 -> anon_inode:[eventpoll]
lrwx------. 1 root root 64 Feb 14 10:03 /proc/1/fd/5 -> anon_inode:[signalfd]
lr-x------. 1 root root 64 Feb 14 10:03 /proc/1/fd/6 -> /sys/fs/cgroup/systemd
lrwx------. 1 root root 64 Feb 14 10:03 /proc/1/fd/7 -> anon_inode:[timerfd]
lrwx------. 1 root root 64 Feb 14 10:03 /proc/1/fd/8 -> socket:[11222]
lr-x------. 1 root root 64 Feb 14 10:03 /proc/1/fd/9 -> /proc/1/mountinfo
lr-x------. 1 root root 64 Feb 14 10:03 /proc/1/fd/10 -> anon_inode:inotify
lr-x------. 1 root root 64 Feb 14 10:03 /proc/1/fd/11 -> /proc/swaps
lrwx------. 1 root root 64 Feb 14 10:03 /proc/1/fd/12 -> socket:[11223]
lrwx------. 1 root root 64 Feb 14 10:03 /proc/1/fd/14 -> socket:[26465]
lr-x------. 1 root root 64 Feb 14 10:03 /proc/1/fd/15 -> anon_inode:inotify
lr-x------. 1 root root 64 Feb 14 10:03 /proc/1/fd/16 -> anon_inode:inotify
lrwx------. 1 root root 64 Feb 14 10:03 /proc/1/fd/18 -> socket:[11228]
lrwx------. 1 root root 64 Feb 14 10:01 /proc/1/fd/22 -> socket:[7244]
lrwx------. 1 root root 64 Feb 14 10:01 /proc/1/fd/23 -> socket:[7246]
lrwx------. 1 root root 64 Feb 14 10:01 /proc/1/fd/24 -> socket:[11514]
lrwx------. 1 root root 64 Feb 14 10:01 /proc/1/fd/25 -> socket:[7264]
lr-x------. 1 root root 64 Feb 14 10:03 /proc/1/fd/26 -> /dev/autofs
lrwx------. 1 root root 64 Feb 14 10:03 /proc/1/fd/27 -> socket:[7267]
lrwx------. 1 root root 64 Feb 14 10:01 /proc/1/fd/28 -> socket:[7269]
lrwx------. 1 root root 64 Feb 14 10:01 /proc/1/fd/29 -> socket:[13428]
lrwx------. 1 root root 64 Feb 14 10:01 /proc/1/fd/30 -> socket:[12418]
lrwx------. 1 root root 64 Feb 14 10:03 /proc/1/fd/31 -> socket:[13486]
lrwx------. 1 root root 64 Feb 14 10:03 /proc/1/fd/32 -> socket:[13528]
lrwx------. 1 root root 64 Feb 14 10:03 /proc/1/fd/33 -> socket:[13938]
lrwx------. 1 root root 64 Feb 14 10:01 /proc/1/fd/34 -> socket:[14650]
lrwx------. 1 root root 64 Feb 14 10:03 /proc/1/fd/35 -> socket:[13444]
lrwx------. 1 root root 64 Feb 14 10:03 /proc/1/fd/36 -> socket:[15889]
lrwx------. 1 root root 64 Feb 14 10:03 /proc/1/fd/37 -> socket:[16095]
lrwx------. 1 root root 64 Feb 14 10:03 /proc/1/fd/38 -> socket:[23146]
lr-x------. 1 root root 64 Feb 14 10:03 /proc/1/fd/39 -> pipe:[11298]
lrwx------. 1 root root 64 Feb 14 10:03 /proc/1/fd/40 -> socket:[11967]
lrwx------. 1 root root 64 Feb 14 10:03 /proc/1/fd/41 -> socket:[13425]
lrwx------. 1 root root 64 Feb 14 10:03 /proc/1/fd/42 -> /run/systemd/initctl/fifo
lrwx------. 1 root root 64 Feb 14 10:03 /proc/1/fd/44 -> socket:[11266]
lrwx------. 1 root root 64 Feb 14 10:03 /proc/1/fd/46 -> socket:[11383]
lr-x------. 1 root root 64 Feb 14 10:02 /proc/2677/fd/0 -> /dev/null
lrwx------. 1 root root 64 Feb 14 10:02 /proc/2677/fd/1 -> socket:[23122]
lrwx------. 1 root root 64 Feb 14 10:02 /proc/2677/fd/2 -> socket:[23122]
lrwx------. 1 root root 64 Feb 14 10:02 /proc/2677/fd/3 -> anon_inode:[eventfd]
lrwx------. 1 root root 64 Feb 14 10:02 /proc/2677/fd/4 -> anon_inode:[eventfd]
lrwx------. 1 root root 64 Feb 14 10:02 /proc/2677/fd/5 -> socket:[23124]
lr-x------. 1 root root 64 Feb 14 10:02 /proc/2677/fd/6 -> net:[4026531956]
lr-x------. 1 root root 64 Feb 14 10:02 /proc/2677/fd/7 -> mnt:[4026532130]
lrwx------. 1 root root 64 Feb 14 10:02 /proc/2677/fd/8 -> socket:[23128]
lrwx------. 1 root root 64 Feb 14 10:02 /proc/2677/fd/9 -> socket:[23129]
lrwx------. 1 root root 64 Feb 14 10:02 /proc/2677/fd/10 -> socket:[23130]
lrwx------. 1 root root 64 Feb 14 10:02 /proc/2677/fd/11 -> socket:[23144]
lrwx------. 1 root root 64 Feb 14 10:02 /proc/2677/fd/12 -> anon_inode:[eventfd]
lr-x------. 1 root root 64 Feb 14 10:02 /proc/2677/fd/13 -> anon_inode:inotify
lr-x------. 1 root root 64 Feb 14 10:02 /proc/2677/fd/14 -> anon_inode:inotify
lrwx------. 1 root root 64 Feb 14 10:02 /proc/2677/fd/15 -> socket:[23198]
lrwx------. 1 root root 64 Feb 14 10:02 /proc/2677/fd/16 -> anon_inode:[eventpoll]
lrwx------. 1 root root 64 Feb 14 10:02 /proc/2677/fd/17 -> socket:[23202]
lrwx------. 1 root root 64 Feb 14 10:02 /proc/2677/fd/18 -> socket:[23327]
l-wx------. 1 root root 64 Feb 14 10:02 /proc/2677/fd/19 -> /run/systemd/inhibit/3.ref
lrwx------. 1 root root 64 Feb 14 10:02 /proc/2677/fd/20 -> anon_inode:[eventpoll]
lrwx------. 1 root root 64 Feb 14 10:02 /proc/2677/fd/21 -> anon_inode:[timerfd]
lrwx------. 1 root root 64 Feb 14 10:02 /proc/2677/fd/22 -> socket:[23374]
lr-x------. 1 root root 64 Feb 14 10:02 /proc/2692/fd/0 -> /dev/null
l-wx------. 1 root root 64 Feb 14 10:02 /proc/2692/fd/1 -> /dev/null
l-wx------. 1 root root 64 Feb 14 10:02 /proc/2692/fd/2 -> /dev/null
lrwx------. 1 root root 64 Feb 14 10:02 /proc/2692/fd/3 -> socket:[23369]
l-wx------. 1 root root 64 Feb 14 10:02 /proc/2692/fd/4 -> /var/lib/NetworkManager/dhclient-5fb06bd0-0bb0-7ffb-45f1-d6edd65f3e03-eth0.lease
lrwx------. 1 root root 64 Feb 14 10:02 /proc/2692/fd/5 -> socket:[23382]
lrwx------. 1 root root 64 Feb 14 10:02 /proc/2692/fd/6 -> socket:[23383]
lr-x------. 1 root root 64 Feb 14 10:01 /proc/331/fd/0 -> /dev/null
l-wx------. 1 root root 64 Feb 14 10:01 /proc/331/fd/1 -> /dev/null
l-wx------. 1 root root 64 Feb 14 10:01 /proc/331/fd/2 -> /dev/null
lrwx------. 1 root root 64 Feb 14 10:01 /proc/331/fd/3 -> socket:[7264]
lrwx------. 1 root root 64 Feb 14 10:01 /proc/331/fd/4 -> socket:[7267]
lrwx------. 1 root root 64 Feb 14 10:01 /proc/331/fd/5 -> socket:[7269]
l-wx------. 1 root root 64 Feb 14 10:01 /proc/331/fd/6 -> /dev/kmsg
lrwx------. 1 root root 64 Feb 14 10:01 /proc/331/fd/7 -> anon_inode:[eventpoll]
lrwx------. 1 root root 64 Feb 14 10:01 /proc/331/fd/8 -> /dev/kmsg
lr-x------. 1 root root 64 Feb 14 10:01 /proc/331/fd/9 -> /proc/sys/kernel/hostname
lrwx------. 1 root root 64 Feb 14 10:01 /proc/331/fd/10 -> anon_inode:[signalfd]
lrwx------. 1 root root 64 Feb 14 10:01 /proc/331/fd/11 -> socket:[11623]
lrwx------. 1 root root 64 Feb 14 10:01 /proc/331/fd/12 -> anon_inode:[timerfd]
lrwx------. 1 root root 64 Feb 14 10:01 /proc/331/fd/13 -> /run/log/journal/b15cb2a63d97a044a8065e4083d397c8/system.journal
lrwx------. 1 root root 64 Feb 14 10:01 /proc/331/fd/14 -> socket:[13486]
lrwx------. 1 root root 64 Feb 14 10:01 /proc/331/fd/15 -> socket:[13528]
lrwx------. 1 root root 64 Feb 14 10:01 /proc/331/fd/16 -> socket:[14650]
lrwx------. 1 root root 64 Feb 14 10:01 /proc/331/fd/17 -> socket:[15889]
lrwx------. 1 root root 64 Feb 14 10:03 /proc/331/fd/20 -> socket:[12418]
lrwx------. 1 root root 64 Feb 14 10:03 /proc/331/fd/21 -> socket:[23146]
lrwx------. 1 root root 64 Feb 14 10:01 /proc/331/fd/23 -> socket:[13938]
lrwx------. 1 root root 64 Feb 14 10:01 /proc/331/fd/24 -> socket:[16095]
lr-x------. 1 root root 64 Feb 14 10:03 /proc/3639/fd/0 -> /dev/null
lrwx------. 1 root root 64 Feb 14 10:03 /proc/3639/fd/1 -> /dev/null
lrwx------. 1 root root 64 Feb 14 10:03 /proc/3639/fd/2 -> /dev/null
lrwx------. 1 root root 64 Feb 14 10:03 /proc/3639/fd/3 -> socket:[26507]
lrwx------. 1 root root 64 Feb 14 10:03 /proc/3639/fd/4 -> socket:[26613]
lrwx------. 1 root root 64 Feb 14 10:03 /proc/3639/fd/5 -> /dev/ptmx
l-wx------. 1 root root 64 Feb 14 10:03 /proc/3639/fd/6 -> /run/systemd/sessions/4.ref
lrwx------. 1 root root 64 Feb 14 10:03 /proc/3639/fd/7 -> socket:[26617]
lrwx------. 1 root root 64 Feb 14 10:03 /proc/3642/fd/0 -> /dev/null
lrwx------. 1 root root 64 Feb 14 10:03 /proc/3642/fd/1 -> /dev/null
lrwx------. 1 root root 64 Feb 14 10:03 /proc/3642/fd/2 -> /dev/null
lrwx------. 1 root root 64 Feb 14 10:03 /proc/3642/fd/3 -> socket:[26507]
lrwx------. 1 root root 64 Feb 14 10:03 /proc/3642/fd/4 -> socket:[26613]
lrwx------. 1 root root 64 Feb 14 10:03 /proc/3642/fd/5 -> socket:[26616]
l-wx------. 1 root root 64 Feb 14 10:03 /proc/3642/fd/6 -> /run/systemd/sessions/4.ref
lr-x------. 1 root root 64 Feb 14 10:03 /proc/3642/fd/7 -> pipe:[26628]
l-wx------. 1 root root 64 Feb 14 10:03 /proc/3642/fd/8 -> pipe:[26628]
lrwx------. 1 root root 64 Feb 14 10:03 /proc/3642/fd/9 -> /dev/ptmx
lrwx------. 1 root root 64 Feb 14 10:03 /proc/3642/fd/13 -> /dev/ptmx
lrwx------. 1 root root 64 Feb 14 10:03 /proc/3642/fd/14 -> /dev/ptmx
lrwx------. 1 vagrant vagrant 64 Feb 14 10:03 /proc/3643/fd/0 -> /dev/pts/0
lrwx------. 1 vagrant vagrant 64 Feb 14 10:03 /proc/3643/fd/1 -> /dev/pts/0
lrwx------. 1 vagrant vagrant 64 Feb 14 10:03 /proc/3643/fd/2 -> /dev/pts/0
lrwx------. 1 vagrant vagrant 64 Feb 14 10:03 /proc/3643/fd/255 -> /dev/pts/0
lrwx------. 1 root root 64 Feb 14 10:03 /proc/3664/fd/0 -> /dev/pts/0
lrwx------. 1 root root 64 Feb 14 10:03 /proc/3664/fd/1 -> /dev/pts/0
lrwx------. 1 root root 64 Feb 14 10:03 /proc/3664/fd/2 -> /dev/pts/0
lrwx------. 1 root root 64 Feb 14 10:03 /proc/3664/fd/3 -> socket:[26681]
lrwx------. 1 root root 64 Feb 14 10:03 /proc/3664/fd/4 -> socket:[26694]
l-wx------. 1 root root 64 Feb 14 10:03 /proc/3664/fd/6 -> /run/systemd/sessions/4.ref
lr-x------. 1 root root 64 Feb 14 10:03 /proc/3664/fd/7 -> pipe:[26697]
l-wx------. 1 root root 64 Feb 14 10:03 /proc/3664/fd/8 -> pipe:[26697]
lrwx------. 1 root root 64 Feb 14 10:03 /proc/3666/fd/0 -> /dev/pts/0
lrwx------. 1 root root 64 Feb 14 10:03 /proc/3666/fd/1 -> /dev/pts/0
lrwx------. 1 root root 64 Feb 14 10:03 /proc/3666/fd/2 -> /dev/pts/0
lrwx------. 1 root root 64 Feb 14 10:03 /proc/3666/fd/255 -> /dev/pts/0
lr-x------. 1 root root 64 Feb 14 10:01 /proc/372/fd/0 -> /dev/null
lrwx------. 1 root root 64 Feb 14 10:01 /proc/372/fd/1 -> socket:[12417]
lrwx------. 1 root root 64 Feb 14 10:01 /proc/372/fd/2 -> socket:[12417]
lrwx------. 1 root root 64 Feb 14 10:01 /proc/372/fd/3 -> socket:[11514]
lrwx------. 1 root root 64 Feb 14 10:01 /proc/372/fd/4 -> socket:[11266]
lrwx------. 1 root root 64 Feb 14 10:01 /proc/372/fd/5 -> socket:[12481]
lr-x------. 1 root root 64 Feb 14 10:01 /proc/372/fd/6 -> /etc/udev/hwdb.bin
lr-x------. 1 root root 64 Feb 14 10:01 /proc/372/fd/7 -> anon_inode:inotify
lrwx------. 1 root root 64 Feb 14 10:01 /proc/372/fd/8 -> anon_inode:[signalfd]
lrwx------. 1 root root 64 Feb 14 10:01 /proc/372/fd/9 -> socket:[12641]
lrwx------. 1 root root 64 Feb 14 10:01 /proc/372/fd/10 -> socket:[12642]
lrwx------. 1 root root 64 Feb 14 10:01 /proc/372/fd/11 -> anon_inode:[eventpoll]
lrwx------. 1 root root 64 Feb 14 10:03 /proc/384/fd/0 -> /dev/null
lrwx------. 1 root root 64 Feb 14 10:03 /proc/384/fd/1 -> /dev/null
lrwx------. 1 root root 64 Feb 14 10:03 /proc/384/fd/2 -> /dev/null
lrwx------. 1 root root 64 Feb 14 10:03 /proc/384/fd/3 -> socket:[12650]
l-wx------. 1 root root 64 Feb 14 10:03 /proc/384/fd/5 -> /var/log/audit/audit.log
lrwx------. 1 root root 64 Feb 14 10:03 /proc/384/fd/6 -> anon_inode:[eventpoll]
lrwx------. 1 root root 64 Feb 14 10:03 /proc/384/fd/7 -> anon_inode:[eventfd]
lrwx------. 1 root root 64 Feb 14 10:03 /proc/384/fd/8 -> socket:[12654]
lrwx------. 1 root root 64 Feb 14 10:03 /proc/384/fd/9 -> socket:[12663]
lrwx------. 1 root root 64 Feb 14 10:03 /proc/384/fd/10 -> socket:[12664]
lrwx------. 1 root root 64 Feb 14 10:01 /proc/431/fd/0 -> /dev/null
lrwx------. 1 root root 64 Feb 14 10:01 /proc/431/fd/1 -> socket:[13527]
lrwx------. 1 root root 64 Feb 14 10:01 /proc/431/fd/2 -> socket:[13527]
lrwx------. 1 root root 64 Feb 14 10:01 /proc/431/fd/3 -> socket:[13425]
lrwx------. 1 root root 64 Feb 14 10:01 /proc/431/fd/4 -> anon_inode:[eventpoll]
lrwx------. 1 root root 64 Feb 14 10:01 /proc/431/fd/5 -> socket:[13565]
lrwx------. 1 root root 64 Feb 14 10:01 /proc/431/fd/6 -> socket:[13566]
lr-x------. 1 root root 64 Feb 14 10:01 /proc/431/fd/7 -> anon_inode:inotify
lrwx------. 1 root root 64 Feb 14 10:01 /proc/431/fd/8 -> socket:[13571]
lrwx------. 1 root root 64 Feb 14 10:01 /proc/431/fd/9 -> socket:[13572]
lrwx------. 1 root root 64 Feb 14 10:01 /proc/431/fd/10 -> socket:[13573]
lrwx------. 1 root root 64 Feb 14 10:01 /proc/431/fd/11 -> socket:[14115]
lrwx------. 1 root root 64 Feb 14 10:01 /proc/431/fd/12 -> socket:[14456]
lrwx------. 1 root root 64 Feb 14 10:01 /proc/431/fd/13 -> socket:[23145]
lrwx------. 1 root root 64 Feb 14 10:01 /proc/431/fd/14 -> socket:[14726]
lrwx------. 1 root root 64 Feb 14 10:01 /proc/431/fd/15 -> socket:[17026]
lrwx------. 1 root root 64 Feb 14 10:01 /proc/431/fd/18 -> socket:[23203]
lr-x------. 1 root root 64 Feb 14 10:03 /proc/433/fd/0 -> /dev/null
lrwx------. 1 root root 64 Feb 14 10:03 /proc/433/fd/1 -> socket:[13485]
lrwx------. 1 root root 64 Feb 14 10:03 /proc/433/fd/2 -> socket:[13485]
lrwx------. 1 root root 64 Feb 14 10:03 /proc/433/fd/3 -> socket:[13545]
lr-x------. 1 root root 64 Feb 14 10:03 /proc/433/fd/4 -> pipe:[13574]
lrwx------. 1 root root 64 Feb 14 10:03 /proc/433/fd/5 -> anon_inode:[eventpoll]
lrwx------. 1 root root 64 Feb 14 10:03 /proc/433/fd/6 -> socket:[13555]
lrwx------. 1 root root 64 Feb 14 10:03 /proc/433/fd/7 -> socket:[13556]
lrwx------. 1 root root 64 Feb 14 10:03 /proc/433/fd/8 -> socket:[13557]
lrwx------. 1 root root 64 Feb 14 10:03 /proc/433/fd/9 -> socket:[13558]
l-wx------. 1 root root 64 Feb 14 10:03 /proc/433/fd/10 -> pipe:[13574]
lrwx------. 1 root root 64 Feb 14 10:01 /proc/446/fd/0 -> /dev/null
lrwx------. 1 root root 64 Feb 14 10:01 /proc/446/fd/1 -> /dev/null
lrwx------. 1 root root 64 Feb 14 10:01 /proc/446/fd/2 -> /dev/null
lr-x------. 1 root root 64 Feb 14 10:01 /proc/446/fd/3 -> anon_inode:inotify
lrwx------. 1 root root 64 Feb 14 10:01 /proc/446/fd/4 -> anon_inode:[eventfd]
lrwx------. 1 root root 64 Feb 14 10:01 /proc/446/fd/5 -> anon_inode:[eventfd]
lrwx------. 1 root root 64 Feb 14 10:01 /proc/446/fd/6 -> socket:[14455]
lrwx------. 1 root root 64 Feb 14 10:01 /proc/446/fd/7 -> anon_inode:[eventfd]
lr-x------. 1 root root 64 Feb 14 10:01 /proc/446/fd/8 -> anon_inode:inotify
lrwx------. 1 root root 64 Feb 14 10:01 /proc/446/fd/9 -> anon_inode:[eventfd]
lrwx------. 1 root root 64 Feb 14 10:01 /proc/446/fd/10 -> anon_inode:[eventfd]
lrwx------. 1 root root 64 Feb 14 10:01 /proc/446/fd/11 -> socket:[14662]
lr-x------. 1 root root 64 Feb 14 10:01 /proc/447/fd/0 -> /dev/null
lrwx------. 1 root root 64 Feb 14 10:01 /proc/447/fd/1 -> socket:[13937]
lrwx------. 1 root root 64 Feb 14 10:01 /proc/447/fd/2 -> socket:[13937]
lrwx------. 1 root root 64 Feb 14 10:01 /proc/447/fd/3 -> socket:[14036]
lrwx------. 1 root root 64 Feb 14 10:01 /proc/447/fd/4 -> anon_inode:[eventpoll]
lrwx------. 1 root root 64 Feb 14 10:01 /proc/447/fd/5 -> anon_inode:[timerfd]
lr-x------. 1 root root 64 Feb 14 10:01 /proc/447/fd/6 -> /sys/devices/virtual/tty/tty0/active
lrwx------. 1 root root 64 Feb 14 10:01 /proc/447/fd/7 -> anon_inode:[signalfd]
lrwx------. 1 root root 64 Feb 14 10:01 /proc/447/fd/8 -> socket:[14110]
lrwx------. 1 root root 64 Feb 14 10:01 /proc/447/fd/9 -> socket:[14111]
lrwx------. 1 root root 64 Feb 14 10:01 /proc/447/fd/10 -> socket:[14112]
lrwx------. 1 root root 64 Feb 14 10:01 /proc/447/fd/11 -> socket:[14113]
lrwx------. 1 root root 64 Feb 14 10:01 /proc/447/fd/12 -> socket:[14114]
lrwx------. 1 root root 64 Feb 14 10:01 /proc/447/fd/13 -> anon_inode:[timerfd]
lrwx------. 1 root root 64 Feb 14 10:01 /proc/447/fd/14 -> /dev/input/event0
lrwx------. 1 root root 64 Feb 14 10:01 /proc/447/fd/15 -> /dev/input/event1
lrwx------. 1 root root 64 Feb 14 10:01 /proc/447/fd/16 -> /dev/tty6
lrwx------. 1 root root 64 Feb 14 10:01 /proc/447/fd/17 -> /dev/input/event4
lr-x------. 1 root root 64 Feb 14 10:01 /proc/447/fd/18 -> /run/systemd/inhibit/3.ref
lr-x------. 1 root root 64 Feb 14 10:01 /proc/447/fd/19 -> /run/systemd/sessions/4.ref
lr-x------. 1 root root 64 Feb 14 10:03 /proc/458/fd/0 -> /dev/null
l-wx------. 1 root root 64 Feb 14 10:03 /proc/458/fd/1 -> /dev/null
lrwx------. 1 root root 64 Feb 14 10:03 /proc/458/fd/2 -> /dev/null
lrwx------. 1 root root 64 Feb 14 10:03 /proc/458/fd/3 -> socket:[14058]
lrwx------. 1 root root 64 Feb 14 10:03 /proc/458/fd/5 -> socket:[14145]
lrwx------. 1 root root 64 Feb 14 10:03 /proc/458/fd/6 -> socket:[14146]
lr-x------. 1 root root 64 Feb 14 10:03 /proc/458/fd/7 -> /dev/urandom
lrwx------. 1 root root 64 Feb 14 10:03 /proc/458/fd/8 -> socket:[14147]
lrwx------. 1 root root 64 Feb 14 10:03 /proc/466/fd/0 -> /dev/null
lrwx------. 1 root root 64 Feb 14 10:03 /proc/466/fd/1 -> /dev/null
lrwx------. 1 root root 64 Feb 14 10:03 /proc/466/fd/2 -> /dev/null
lrwx------. 1 root root 64 Feb 14 10:03 /proc/466/fd/3 -> socket:[13428]
lr-x------. 1 root root 64 Feb 14 10:03 /proc/466/fd/4 -> /run/rpcbind.lock
lrwx------. 1 root root 64 Feb 14 10:03 /proc/466/fd/5 -> socket:[14166]
lrwx------. 1 root root 64 Feb 14 10:03 /proc/466/fd/6 -> socket:[14070]
lrwx------. 1 root root 64 Feb 14 10:03 /proc/466/fd/7 -> socket:[14086]
lrwx------. 1 root root 64 Feb 14 10:03 /proc/466/fd/8 -> socket:[14087]
lrwx------. 1 root root 64 Feb 14 10:03 /proc/466/fd/9 -> socket:[14088]
lrwx------. 1 root root 64 Feb 14 10:03 /proc/466/fd/10 -> socket:[14089]
lrwx------. 1 root root 64 Feb 14 10:03 /proc/466/fd/11 -> socket:[14090]
lr-x------. 1 root root 64 Feb 14 10:01 /proc/503/fd/0 -> /dev/null
lrwx------. 1 root root 64 Feb 14 10:01 /proc/503/fd/1 -> socket:[14649]
lrwx------. 1 root root 64 Feb 14 10:01 /proc/503/fd/2 -> socket:[14649]
lrwx------. 1 root root 64 Feb 14 10:01 /proc/503/fd/3 -> /run/crond.pid
lrwx------. 1 root root 64 Feb 14 10:01 /proc/503/fd/4 -> socket:[14759]
lr-x------. 1 root root 64 Feb 14 10:01 /proc/503/fd/5 -> anon_inode:inotify
lrwx------. 1 root root 64 Feb 14 10:02 /proc/504/fd/0 -> /dev/tty1
lrwx------. 1 root root 64 Feb 14 10:02 /proc/504/fd/1 -> /dev/tty1
lrwx------. 1 root root 64 Feb 14 10:02 /proc/504/fd/2 -> /dev/tty1
lr-x------. 1 root root 64 Feb 14 10:02 /proc/722/fd/0 -> /dev/null
lrwx------. 1 root root 64 Feb 14 10:02 /proc/722/fd/1 -> socket:[15888]
lrwx------. 1 root root 64 Feb 14 10:02 /proc/722/fd/2 -> socket:[15888]
l-wx------. 1 root root 64 Feb 14 10:02 /proc/722/fd/3 -> /var/log/tuned/tuned.log
lrwx------. 1 root root 64 Feb 14 10:02 /proc/722/fd/4 -> socket:[16495]
lr-x------. 1 root root 64 Feb 14 10:02 /proc/722/fd/5 -> /dev/urandom
lrwx------. 1 root root 64 Feb 14 10:02 /proc/722/fd/6 -> socket:[17025]
lrwx------. 1 root root 64 Feb 14 10:02 /proc/722/fd/7 -> anon_inode:[eventfd]
lrwx------. 1 root root 64 Feb 14 10:02 /proc/722/fd/8 -> /tmp/#67151050 (deleted)
lrwx------. 1 root root 64 Feb 14 10:02 /proc/722/fd/9 -> anon_inode:[eventfd]
l-wx------. 1 root root 64 Feb 14 10:02 /proc/722/fd/10 -> /dev/cpu_dma_latency
lr-x------. 1 root root 64 Feb 14 10:02 /proc/722/fd/11 -> pipe:[17033]
l-wx------. 1 root root 64 Feb 14 10:02 /proc/722/fd/12 -> pipe:[17033]
lrwx------. 1 root root 64 Feb 14 10:02 /proc/722/fd/13 -> anon_inode:[eventpoll]
lr-x------. 1 root root 64 Feb 14 10:02 /proc/723/fd/0 -> /dev/null
l-wx------. 1 root root 64 Feb 14 10:02 /proc/723/fd/1 -> /dev/null
l-wx------. 1 root root 64 Feb 14 10:02 /proc/723/fd/2 -> /dev/null
lr-x------. 1 root root 64 Feb 14 10:02 /proc/723/fd/3 -> anon_inode:inotify
lrwx------. 1 root root 64 Feb 14 10:02 /proc/723/fd/4 -> socket:[16163]
lr-x------. 1 root root 64 Feb 14 10:02 /proc/723/fd/5 -> /run/log/journal/b15cb2a63d97a044a8065e4083d397c8/system.journal
l-wx------. 1 root root 64 Feb 14 10:02 /proc/723/fd/6 -> /var/log/secure
l-wx------. 1 root root 64 Feb 14 10:02 /proc/723/fd/7 -> /var/log/messages
l-wx------. 1 root root 64 Feb 14 10:02 /proc/723/fd/8 -> /var/log/cron
l-wx------. 1 root root 64 Feb 14 10:02 /proc/723/fd/9 -> /var/log/maillog
lr-x------. 1 root root 64 Feb 14 10:02 /proc/725/fd/0 -> /dev/null
lrwx------. 1 root root 64 Feb 14 10:02 /proc/725/fd/1 -> socket:[16094]
lrwx------. 1 root root 64 Feb 14 10:02 /proc/725/fd/2 -> socket:[16094]
lrwx------. 1 root root 64 Feb 14 10:02 /proc/725/fd/3 -> socket:[16185]
lrwx------. 1 root root 64 Feb 14 10:02 /proc/725/fd/4 -> socket:[16205]
lrwx------. 1 root root 64 Feb 14 10:03 /proc/926/fd/0 -> /dev/null
lrwx------. 1 root root 64 Feb 14 10:03 /proc/926/fd/1 -> /dev/null
lrwx------. 1 root root 64 Feb 14 10:03 /proc/926/fd/2 -> /dev/null
lrwx------. 1 root root 64 Feb 14 10:03 /proc/926/fd/3 -> socket:[16858]
lrwx------. 1 root root 64 Feb 14 10:03 /proc/926/fd/4 -> /dev/null
lr-x------. 1 root root 64 Feb 14 10:03 /proc/926/fd/5 -> pipe:[16984]
lrwx------. 1 root root 64 Feb 14 10:03 /proc/926/fd/6 -> /dev/null
lrwx------. 1 root root 64 Feb 14 10:03 /proc/926/fd/7 -> /dev/null
lrwx------. 1 root root 64 Feb 14 10:03 /proc/926/fd/8 -> /dev/null
lrwx------. 1 root root 64 Feb 14 10:03 /proc/926/fd/9 -> /dev/null
lrwx------. 1 root root 64 Feb 14 10:03 /proc/926/fd/10 -> /var/spool/postfix/pid/master.pid
lrwx------. 1 root root 64 Feb 14 10:03 /proc/926/fd/11 -> /var/lib/postfix/master.lock
lr-x------. 1 root root 64 Feb 14 10:03 /proc/926/fd/12 -> pipe:[16959]
lrwx------. 1 root root 64 Feb 14 10:03 /proc/926/fd/13 -> socket:[16884]
lrwx------. 1 root root 64 Feb 14 10:03 /proc/926/fd/14 -> socket:[16885]
lrwx------. 1 root root 64 Feb 14 10:03 /proc/926/fd/15 -> anon_inode:[eventpoll]
lrwx------. 1 root root 64 Feb 14 10:03 /proc/926/fd/16 -> socket:[16886]
lrwx------. 1 root root 64 Feb 14 10:03 /proc/926/fd/17 -> socket:[16887]
lrwx------. 1 root root 64 Feb 14 10:03 /proc/926/fd/18 -> socket:[16888]
lrwx------. 1 root root 64 Feb 14 10:03 /proc/926/fd/19 -> socket:[16889]
lrwx------. 1 root root 64 Feb 14 10:03 /proc/926/fd/20 -> socket:[16890]
lrwx------. 1 root root 64 Feb 14 10:03 /proc/926/fd/22 -> socket:[16892]
lrwx------. 1 root root 64 Feb 14 10:03 /proc/926/fd/23 -> socket:[16893]
lrwx------. 1 root root 64 Feb 14 10:03 /proc/926/fd/24 -> socket:[16894]
lrwx------. 1 root root 64 Feb 14 10:03 /proc/926/fd/25 -> socket:[16895]
lrwx------. 1 root root 64 Feb 14 10:03 /proc/926/fd/26 -> socket:[16896]
lrwx------. 1 root root 64 Feb 14 10:03 /proc/926/fd/27 -> socket:[16897]
lrwx------. 1 root root 64 Feb 14 10:03 /proc/926/fd/29 -> socket:[16899]
lrwx------. 1 root root 64 Feb 14 10:03 /proc/926/fd/30 -> socket:[16900]
lrwx------. 1 root root 64 Feb 14 10:03 /proc/926/fd/31 -> socket:[16901]
lrwx------. 1 root root 64 Feb 14 10:03 /proc/926/fd/32 -> socket:[16902]
lrwx------. 1 root root 64 Feb 14 10:03 /proc/926/fd/33 -> socket:[16903]
lrwx------. 1 root root 64 Feb 14 10:03 /proc/926/fd/34 -> socket:[16904]
lrwx------. 1 root root 64 Feb 14 10:03 /proc/926/fd/35 -> socket:[16905]
lrwx------. 1 root root 64 Feb 14 10:03 /proc/926/fd/36 -> socket:[16906]
lrwx------. 1 root root 64 Feb 14 10:03 /proc/926/fd/37 -> socket:[16907]
lrwx------. 1 root root 64 Feb 14 10:03 /proc/926/fd/38 -> socket:[16908]
lrwx------. 1 root root 64 Feb 14 10:03 /proc/926/fd/39 -> socket:[16909]
lrwx------. 1 root root 64 Feb 14 10:03 /proc/926/fd/40 -> socket:[16910]
lrwx------. 1 root root 64 Feb 14 10:03 /proc/926/fd/41 -> socket:[16911]
lrwx------. 1 root root 64 Feb 14 10:03 /proc/926/fd/42 -> socket:[16912]
lrwx------. 1 root root 64 Feb 14 10:03 /proc/926/fd/43 -> socket:[16913]
lrwx------. 1 root root 64 Feb 14 10:03 /proc/926/fd/44 -> socket:[16914]
lrwx------. 1 root root 64 Feb 14 10:03 /proc/926/fd/45 -> socket:[16915]
lrwx------. 1 root root 64 Feb 14 10:03 /proc/926/fd/46 -> socket:[16916]
lrwx------. 1 root root 64 Feb 14 10:03 /proc/926/fd/47 -> socket:[16917]
lrwx------. 1 root root 64 Feb 14 10:03 /proc/926/fd/48 -> socket:[16918]
lrwx------. 1 root root 64 Feb 14 10:03 /proc/926/fd/49 -> socket:[16919]
lrwx------. 1 root root 64 Feb 14 10:03 /proc/926/fd/50 -> socket:[16920]
lrwx------. 1 root root 64 Feb 14 10:03 /proc/926/fd/51 -> socket:[16921]
lrwx------. 1 root root 64 Feb 14 10:03 /proc/926/fd/52 -> socket:[16922]
lrwx------. 1 root root 64 Feb 14 10:03 /proc/926/fd/53 -> socket:[16923]
lrwx------. 1 root root 64 Feb 14 10:03 /proc/926/fd/54 -> socket:[16924]
lrwx------. 1 root root 64 Feb 14 10:03 /proc/926/fd/55 -> socket:[16925]
lrwx------. 1 root root 64 Feb 14 10:03 /proc/926/fd/56 -> socket:[16926]
lrwx------. 1 root root 64 Feb 14 10:03 /proc/926/fd/57 -> socket:[16927]
lrwx------. 1 root root 64 Feb 14 10:03 /proc/926/fd/58 -> socket:[16928]
lrwx------. 1 root root 64 Feb 14 10:03 /proc/926/fd/59 -> socket:[16929]
lrwx------. 1 root root 64 Feb 14 10:03 /proc/926/fd/60 -> socket:[16930]
lrwx------. 1 root root 64 Feb 14 10:03 /proc/926/fd/61 -> socket:[16931]
lrwx------. 1 root root 64 Feb 14 10:03 /proc/926/fd/62 -> socket:[16932]
lrwx------. 1 root root 64 Feb 14 10:03 /proc/926/fd/63 -> socket:[16933]
lrwx------. 1 root root 64 Feb 14 10:03 /proc/926/fd/64 -> socket:[16934]
lrwx------. 1 root root 64 Feb 14 10:03 /proc/926/fd/65 -> socket:[16935]
lrwx------. 1 root root 64 Feb 14 10:03 /proc/926/fd/66 -> socket:[16936]
lrwx------. 1 root root 64 Feb 14 10:03 /proc/926/fd/67 -> socket:[16937]
lrwx------. 1 root root 64 Feb 14 10:03 /proc/926/fd/68 -> socket:[16938]
lrwx------. 1 root root 64 Feb 14 10:03 /proc/926/fd/69 -> socket:[16939]
lrwx------. 1 root root 64 Feb 14 10:03 /proc/926/fd/70 -> socket:[16940]
lrwx------. 1 root root 64 Feb 14 10:03 /proc/926/fd/71 -> socket:[16941]
lrwx------. 1 root root 64 Feb 14 10:03 /proc/926/fd/72 -> socket:[16942]
lrwx------. 1 root root 64 Feb 14 10:03 /proc/926/fd/73 -> socket:[16943]
lrwx------. 1 root root 64 Feb 14 10:03 /proc/926/fd/74 -> socket:[16944]
lrwx------. 1 root root 64 Feb 14 10:03 /proc/926/fd/75 -> socket:[16945]
lrwx------. 1 root root 64 Feb 14 10:03 /proc/926/fd/76 -> socket:[16946]
lrwx------. 1 root root 64 Feb 14 10:03 /proc/926/fd/77 -> socket:[16947]
lrwx------. 1 root root 64 Feb 14 10:03 /proc/926/fd/78 -> socket:[16948]
lrwx------. 1 root root 64 Feb 14 10:03 /proc/926/fd/79 -> socket:[16949]
lrwx------. 1 root root 64 Feb 14 10:03 /proc/926/fd/80 -> socket:[16950]
lrwx------. 1 root root 64 Feb 14 10:03 /proc/926/fd/81 -> socket:[16951]
lrwx------. 1 root root 64 Feb 14 10:03 /proc/926/fd/82 -> socket:[16952]
lrwx------. 1 root root 64 Feb 14 10:03 /proc/926/fd/83 -> socket:[16953]
lrwx------. 1 root root 64 Feb 14 10:03 /proc/926/fd/84 -> socket:[16954]
lrwx------. 1 root root 64 Feb 14 10:03 /proc/926/fd/85 -> socket:[16955]
lrwx------. 1 root root 64 Feb 14 10:03 /proc/926/fd/86 -> socket:[16956]
lrwx------. 1 root root 64 Feb 14 10:03 /proc/926/fd/87 -> socket:[16957]
lrwx------. 1 root root 64 Feb 14 10:03 /proc/926/fd/88 -> socket:[16958]
l-wx------. 1 root root 64 Feb 14 10:03 /proc/926/fd/89 -> pipe:[16959]
lr-x------. 1 root root 64 Feb 14 10:03 /proc/926/fd/90 -> pipe:[16960]
l-wx------. 1 root root 64 Feb 14 10:03 /proc/926/fd/91 -> pipe:[16960]
l-wx------. 1 root root 64 Feb 14 10:03 /proc/926/fd/92 -> pipe:[16984]
lrwx------. 1 root root 64 Feb 14 10:03 /proc/943/fd/0 -> /dev/null
lrwx------. 1 root root 64 Feb 14 10:03 /proc/943/fd/1 -> /dev/null
lrwx------. 1 root root 64 Feb 14 10:03 /proc/943/fd/2 -> /dev/null
lr-x------. 1 root root 64 Feb 14 10:03 /proc/943/fd/3 -> pipe:[16960]
l-wx------. 1 root root 64 Feb 14 10:03 /proc/943/fd/4 -> pipe:[16960]
lrwx------. 1 root root 64 Feb 14 10:03 /proc/943/fd/5 -> socket:[16890]
lrwx------. 1 root root 64 Feb 14 10:03 /proc/943/fd/6 -> socket:[16888]
lrwx------. 1 root root 64 Feb 14 10:03 /proc/943/fd/7 -> socket:[17005]
lrwx------. 1 root root 64 Feb 14 10:03 /proc/943/fd/8 -> anon_inode:[eventpoll]
lr-x------. 1 root root 64 Feb 14 10:03 /proc/943/fd/9 -> pipe:[17021]
l-wx------. 1 root root 64 Feb 14 10:03 /proc/943/fd/10 -> pipe:[17021]
l-wx------. 1 root root 64 Feb 14 10:03 /proc/943/fd/92 -> pipe:[16984]
lrwx------. 1 root root 64 Feb 14 10:03 /proc/944/fd/0 -> /dev/null
lrwx------. 1 root root 64 Feb 14 10:03 /proc/944/fd/1 -> /dev/null
lrwx------. 1 root root 64 Feb 14 10:03 /proc/944/fd/2 -> /dev/null
lr-x------. 1 root root 64 Feb 14 10:03 /proc/944/fd/3 -> pipe:[16960]
l-wx------. 1 root root 64 Feb 14 10:03 /proc/944/fd/4 -> pipe:[16960]
lrwx------. 1 root root 64 Feb 14 10:03 /proc/944/fd/5 -> socket:[16897]
lrwx------. 1 root root 64 Feb 14 10:03 /proc/944/fd/6 -> socket:[16895]
lrwx------. 1 root root 64 Feb 14 10:03 /proc/944/fd/7 -> socket:[16986]
lrwx------. 1 root root 64 Feb 14 10:03 /proc/944/fd/8 -> anon_inode:[eventpoll]
lr-x------. 1 root root 64 Feb 14 10:03 /proc/944/fd/11 -> pipe:[17002]
```
</details>


А еще поиграть с реализацией 2 конкурирующих процессов по IO. пробовать запустить с разными ionice

```
[root@otusproc /]# time dd if=/dev/sda of=/dev/null & sleep 5
[root@otusproc /]# time dd if=/dev/sda of=/dev/null &

```
[root@otusproc /]# ionice -c 1 -p 4134
[root@otusproc /]# ionice -c 3 -p 4132

[root@otusproc /]# ionice -p 4134
realtime: prio 4
[root@otusproc /]# ionice -p 4132
idle
```
```
[root@otusproc /]# 83886080+0 records in
83886080+0 records out
42949672960 bytes (43 GB) copied, 295.222 s, 145 MB/s

real    4m55.224s
user    0m15.279s
sys     2m10.994s
83886080+0 records in
83886080+0 records out
42949672960 bytes (43 GB) copied, 296.587 s, 145 MB/s

real    4m56.633s
user    0m15.650s
sys     2m11.939s
```
Видно несущественную разницу в скорости выполнения процесса с повышенным приоритетом.
