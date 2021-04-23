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

We will be using vs code for development.
Inside the header is magic data which is necessary so that the bootloader can understand that we have an OS that can be run.
Bootloader is the first loader which is use to locate OS, once it finds OS it will be able to start.

main.asm file which is the entry point to our OS.
We have a halt instruction at the end of print to instruct the CPU to freeze and not run any further instructions.

**Linker**
tells how to link our OS together first section in linker is multiboot loader and then there is text section.

**ISO** is common format to hold OS.
We write build commands in makeFile and create object file in makeFile where first we will make sure directory exists and then we will use linker to link our object files.

{{<figure src = "/uploads/screenshot.jpg">}}
