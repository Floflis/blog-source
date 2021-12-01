---
author: "Daniell Mesquita"
title: ISO of 17.4 GB! We need to compress it
date: 2019-07-01T16:13:27-04:00
tags: ["development", "logs"]
categories: ["logs"]
---

![](/blog/img/posts/iso-of-17gb-we-need-to-compress-it.png)

After deciding to start Floflis as a live distro/OS (bootable and usable right after recording it on flash drives), it needs to not be heavyweight. And after tunning it in upcoming builds (being even smaller), make it lightweight and modular, which will be explained in the next post (Floflis' Layers).

I've scanned `bin, etc, lib, lib64, opt, root, sbin, srv, usr, var` root directories, which will be used by `live-linux` scriptset to build the ISO.
17.4 GB is very challenging, as the maximum threshold I'm defining for the distribution .ISO is 3,5 GB. I'll work on that by removing some uneed software (OBS, Audacity - making them available to download in feature packs), removing binaries of Electron apps (Arbore, Siderus Orion, Balena Etcher - using just one Electron binary, preparing it for HTML5Apps Platform) and by compressing all installable files and extracting when need to install.
