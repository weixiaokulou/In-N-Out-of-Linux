# Weekly plan for In-N-Out of Linux

Weekly plan with clear deliverables based on 2-month schedule, organized to help develop an in-depth understanding of OS internals (focusing on Linux) while giving  several projects to publish on GitHub.

## Week 1-2: Operating System Fundamentals (Theory + Practice)  
### Focus:  
Learn key OS concepts such as processes, memory management, I/O, and file systems.
Get familiar with system calls and process management in Linux.  
### Tasks:  
Study: Read chapters from "Operating Systems: Three Easy Pieces" (focus on processes, memory management, I/O).  
### Practical:  
Use Linux tools like strace, lsof, and ps to inspect system calls and process states.
Write simple programs using system calls (fork(), exec(), wait(), etc.) to manipulate processes.  
Document: Take notes on your learnings and code snippets.  
### Deliverables (for GitHub):  
Project Folder: os-fundamentals/  
Code: Upload your process management programs that demonstrate fork(), exec(), etc.
README.md: Write a brief explanation of each program and how system calls work in Linux.  
## Week 3-4: Linux Kernel Build and Modification
### Focus:
Build your own Linux kernel, learn how it works, and make simple modifications.  
Tasks:    
Kernel Build: Download and compile the Linux kernel from the official source.  
Modify Kernel: Apply simple patches to:  
Add a custom printk() message during boot.  
Modify scheduling parameters or any basic kernel-level feature.  
Testing: Run your custom kernel in a virtual machine (QEMU or VirtualBox).  
Document: Write a patch and explain your kernel modifications.  
### Deliverables (for GitHub):
Project Folder: custom-linux-kernel/
Patch File: Include your kernel modification as a .patch file.
README.md: Instructions on how to compile and test the modified Linux kernel.
Screenshots: Show the kernel booting with your changes.
## Week 5-6: Writing Linux Kernel Modules
### Focus:
Write and test Linux kernel modules, like device drivers and memory management modules.
### Tasks:
Module Development:  
Write a basic "Hello, World" kernel module.  
Develop a more advanced module, like a simple character device driver or memory management interaction.  
Testing: Load your modules using insmod, and verify their behavior with dmesg.
Document: Explain the purpose and functionality of each module.  
Deliverables (for GitHub):  
Project Folder: linux-kernel-modules/  
**hello-world-module/`: Code and instructions for a basic "Hello, World" module.  
**custom-driver/`: A simple custom driver or memory management module.  
README.md: How to compile, install, and test each module with insmod and rmmod.  
## Week 7: Xv6 Operating System Exploration
### Focus:
Study and modify a simple operating system (Xv6), which provides a minimalistic view of core OS functions.
### Tasks:
Xv6 Exploration: Download and explore the Xv6 source code.
Modify Xv6:  
Implement a new system call.  
Modify the scheduling algorithm.  
Testing: Run your modified Xv6 on QEMU.  
Document: Explain the changes you made and their effects.  
### Deliverables (for GitHub):
Project Folder: xv6-custom/  
Source Code: Include your modified Xv6 source code.  
README.md: Detailed explanation of the system call or scheduling modification and instructions for running Xv6 on QEMU.
## Week 8: Writing a Simple Bootloader and Minimal OS (Optional)
### Focus:
Write a basic bootloader in assembly and a minimal OS in C.
### Tasks:
Bootloader: Write a bootloader that prints text and switches to protected mode.
Kernel: Write a minimal kernel in C that handles basic tasks (e.g., printing to the screen).  
Testing: Run your bootloader and kernel in QEMU.  
Document: Explain the boot process, how the kernel is initialized, and the flow of execution.  
### Deliverables (for GitHub):
Project Folder: simple-bootloader/  
bootloader.asm: Your assembly code for the bootloader.  
kernel.c: Your minimal kernel code.  
README.md: How to build and run the bootloader and kernel on QEMU.  
Additional Resources to Publish  
Comprehensive Documentation:  

In each week's repository, include detailed notes and explanations as markdown files or blog posts.
Document your thought process, challenges faced, and insights gained.
## Project Portfolio:

Once the 2 months are over, you can bundle all your projects under one GitHub repository with submodules for each week's deliverables.  
Create a top-level README.md explaining your overall learning journey and linking to individual projects.  

## Deliverables Outline:
os-fundamentals/:

System call examples and process management programs.
custom-linux-kernel/:

A patch for a custom Linux kernel and instructions for running it.
linux-kernel-modules/:

Kernel modules (e.g., "Hello, World", device drivers) with installation instructions.
xv6-custom/:

Modifications to Xv6 (e.g., new system calls, scheduling) with explanations.
simple-bootloader/ (optional):

Basic bootloader and kernel written in assembly and C.