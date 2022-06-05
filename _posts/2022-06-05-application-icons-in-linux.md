---
layout: post
title: "Application icons in linux"
date: 2022-06-05 15:06:17 +0530
tags: linux tech
---

The premise is that I wanted to show `VirtualBox` icons in a notification which is shown when I start/stop a VM. This led me to find where the app icons are located in general, which can be used with `notify-send` to display them in the notifications.

# Conclusion

Turns out the app icons are located at `/usr/share/pixmaps`.

![]({{site.baseurl}}assets/img/notif-icon.webp)

Cheers.
