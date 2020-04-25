---
layout: post
title: "Как сохранить MBR в файл и восстановить его"
date: 2020-04-23
---
sfdisk -d /dev/sda >file — сохранить инфу о разделах

sfdisk /dev/sda <file — восстановить (перезаписать) МБР
