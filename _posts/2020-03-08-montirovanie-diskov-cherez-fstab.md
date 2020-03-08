---
layout: post
title: "Монтирование дисков через fstab"
date: 2020-03-08
---
```
# nano /etc/fstab
```

Пример файла fstab:
```
UUID=8c2ceb4c-b553-4429-9850-5c3deaf0fd63 /               ext3    errors=remount-ro 0       1
UUID=7b82ee46-8123-42d0-b8d5-f5779ebec1e4 /boot           ext3    defaults        0       2
UUID=3a16e2e5-a8f0-42c6-bd76-7802b86a1cd1 /home           ext3    defaults        0       2
UUID=2545715c-343a-42dd-ac26-bab384ff6f20 none            swap    sw              0       0
UUID=4C3255C73255B6A4   /mnt/DiskC      ntfs-3g rw      0       0
UUID=40177D977561BB95   /mnt/DiskD      ntfs-3g rw      0       0
```

Разделы жестких дисков указываются названиями устройств (/dev/sdc1), или через UUID , которые можно получить командой:
```
# blkid
```
