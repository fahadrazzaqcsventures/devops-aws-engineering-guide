# What Is an Operating System (OS)

## Purpose

This document explains **what an operating system is, why it exists, and what responsibilities it owns** in any computing environment.

Before learning Linux commands, cloud services, or DevOps tools, you must understand the OS as the **control plane between hardware and applications**. Every production incident ultimately involves OS behavior.

---

## Definition

An **Operating System (OS)** is system software that:

* Manages hardware resources
* Provides a runtime environment for applications
* Enforces security and isolation
* Abstracts hardware complexity from users and programs

Without an OS, applications cannot run reliably or safely on shared hardware.

---

## Core Responsibilities of an OS

### 1. Process Management

The OS:

* Creates, schedules, and terminates processes
* Allocates CPU time
* Handles multitasking and concurrency

Production relevance:

* High CPU usage
* Hung or zombie processes
* Load and performance tuning

---

### 2. Memory Management

The OS:

* Allocates RAM to processes
* Manages virtual memory and swapping
* Prevents one process from accessing another’s memory

Production relevance:

* Out-of-memory (OOM) kills
* Application crashes
* Performance degradation

---

### 3. Storage & Filesystem Management

The OS:

* Manages disks and filesystems
* Controls file permissions and ownership
* Handles I/O operations

Production relevance:

* Disk full incidents
* Data corruption
* Log management

---

### 4. Device Management

The OS:

* Controls hardware via drivers
* Abstracts devices as files or interfaces

Production relevance:

* Network interfaces
* Storage devices
* Virtual devices in cloud environments

---

### 5. Networking

The OS:

* Implements network stacks (TCP/IP)
* Manages ports and sockets
* Enforces firewall rules

Production relevance:

* Service connectivity
* Port conflicts
* Network troubleshooting

---

### 6. Security & Access Control

The OS:

* Authenticates users
* Authorizes actions
* Isolates processes

Production relevance:

* Least privilege
* Service accounts
* Breach containment

---

## Kernel vs User Space

### Kernel

* Core of the OS
* Runs with highest privilege
* Manages CPU, memory, devices

### User Space

* Where applications and services run
* Limited access to hardware

> All application requests to hardware go **through the kernel**.

---

## OS Types (High-Level)

| Type     | Examples              | Usage               |
| -------- | --------------------- | ------------------- |
| Desktop  | Windows, macOS        | End-user systems    |
| Server   | Linux, Windows Server | Data centers, cloud |
| Embedded | RTOS, embedded Linux  | IoT, devices        |
| Mobile   | Android, iOS          | Smartphones         |

---

## Why OS Knowledge Matters in DevOps

DevOps engineers:

* Debug OS-level issues
* Tune performance
* Secure systems
* Operate containers and cloud instances

Containers, Kubernetes, and cloud services **do not remove the OS** — they sit on top of it.

---

## Key Takeaway

> Applications do not run on servers.
> **They run on operating systems.**

If you do not understand the OS, you are operating blind.