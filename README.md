# Lightweight Container Runtime (OS Mini Project)

## 📌 Overview

This project implements a lightweight container runtime in C using Linux
system calls. It demonstrates core Operating System concepts such as
process isolation, inter-process communication, synchronization, and
kernel interaction.

## 🚀 Features

-   Process isolation using Linux namespaces (PID, UTS, Mount)
-   Filesystem isolation using chroot()
-   Supervisor-based container management
-   Logging system using pipes
-   Producer--consumer synchronization
-   Kernel module using ioctl

## 📂 Project Structure

. ├── engine.c ├── monitor.c ├── monitor_ioctl.h ├── cpu_hog.c ├──
memory_hog.c ├── io_pulse.c ├── Makefile

## ⚙️ Build & Run

make sudo insmod monitor.ko sudo ./engine start alpha ./engine logs
alpha sudo ./engine stop alpha

## 📁 Root Filesystem Setup

Root filesystem not included due to size. Use Alpine Linux minirootfs.

## 👨‍💻 Authors

-   Akshat Kumar (PES2UG24CS046)
-   A S Vincent (PES2UG24CS002)
