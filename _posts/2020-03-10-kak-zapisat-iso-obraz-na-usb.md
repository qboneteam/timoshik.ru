---
layout: post
title: "Как записать ISO образ на USB-флэшку"
date: 2020-03-10
---
```
# dd if=<downloaded image>.iso of=/dev/<output device> bs=4M && sync
```
