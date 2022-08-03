---
layout: post
title: "Fix for pacman corrupted package error"
date: 2022-08-03 22:08:21 +0530
tags: linux tech arch-linux
---

So at times, especially if you haven't been updating on a daily basis
(*naughty*), when you update using the good ol' `sudo pacman -Syu`, you will
eventually be faced with this error:
```shell
error: failed to commit transaction (invalid or corrupted package)
Errors occurred, no packages were upgraded.
```

In times like this what one must do is to update the `archlinux-keyring` package
first and then update the other packages. So you do
```shell
sudo pacman -Sy archlinux-keyring
```
and then do the usual `sudo pacman -Syu`, and all your problems would be solved.

Cheers.