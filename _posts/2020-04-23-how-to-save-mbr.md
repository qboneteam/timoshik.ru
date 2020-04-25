---
layout: post
title: "Как сохранить MBR в файл ивосстановить его"
date: 2020-04-23
---
sfdisk -d /dev/sda >file — сохранить инфу о разделах

sfdisk /dev/sda <file — восстановить (перезаписать) МБР
