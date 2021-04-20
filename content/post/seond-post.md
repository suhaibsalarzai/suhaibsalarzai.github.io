---
title: "32 BIT ARCHITECTURE"
date: 2021-04-15T22:08:41+05:00
draft: false
image: "uploads/header.jpg"
tags: ["project"]
---

# Working and Development

OS is written in C also we need assembly for hardware code.

1. Install Docker which allows us reproducable environment.
2. Install Qemu which allows us to emulate OS

- First we will work in 32 bit architecure.

1. Actual numbers don't matter, just that it's a number
1. Ordered sub-list
1. And another item.

We will be using vs code for development.
Inside the header is magic data which is necessary so that the bootloader can understand that we have an OS that can be run.
Bootloader is the first loader which is use to locate OS, once it finds OS it will be able to start.

main.asm file which is the entry point to our OS.
We have a halt instruction at the end of print to instruct the CPU to freeze and not run any further instructions.


⋅⋅⋅To have a line break without a paragraph, you will need to use two trailing spaces.⋅⋅
⋅⋅⋅Note that this line is separate, but within the same paragraph.⋅⋅
⋅⋅⋅(This is contrary to the typical GFM line break behaviour, where trailing spaces are not required.)

- Unordered list can use asterisks

* Or minuses

- Or pluses

{{<figure src = "/uploads/head.jpg">}}
