---
title: "64 Bit OS"
date: 2021-04-16T19:20:53+05:00
draft: false
tags: ["project"]
---

# Working and Development

In this part we modified the already created 32 bit OS.

First we will be setting up stack which is crucial to allow us to link in with C code. After that we will switch OS to 64 bit mode.

- We will write C code to print any text to the screen. As I have printed SEECS created from special characters.

As stack stores functions and variable used in code, we will create stacks. We will also check for different functions like CPID to check whether it support long mode or not. If LN bit is set long mode is available.

We typically work with virtual addresses and will implement virtual memory in order to enter 64 bit long mode through paging process. Paging allows us to map virtual address to physical address and we do this by creating page tables. Each table is 4 KBytes.

Paging will be enable as soon as we enable long mode we have to pass page table location to the CPU. The CPU looks for it in cr3 register.

To enter 64 bit mode we need global descriptor table after enabling paging we can load local descriptor table and then the code segment in code selector. We eill create kernel function in C and call it in assembly..
We will set color for foreground and background.

Finally we will make some changes to the makeFile that we created in 32 bit mode where we will create some variable for C source file and object files also for kernel source file and object file. We will update build commands also and include kernel objects as well.

{{<figure src = "/uploads/64.jpg">}}
