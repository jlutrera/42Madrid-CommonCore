# 🚀 42 Common Core Projects

This repository gathers the projects developed during the **42 Common Core**.  
Each project explores a different area of programming, systems, and algorithms.

---

## 📑 Table of Contents
- [📚 Libft](#-libft)
- [🖨️ ft_printf](#️-ft_printf)
- [📄 Get_next_line](#-get_next_line)
- [🛡️ Born2beroot](#️-born2beroot)
- [🔢 Push_swap](#-push_swap)
- [📡 Minitalk](#-minitalk)
- [🕸️ FDF](#fdf)
- [🤔 Philosophers](#-philosophers)
- [💻 Minishell](#-minishell)
- [🌌 MiniRT](#-minirt)
- [🌐 NetPractice](#-netpractice)
- [⚙️ CPP 00–04](#️-cpp-0004)
- [⚙️ CPP 05–09](#️-cpp-0509)
- [🐳 Inception](#-inception)
- [🌍 Webserv](#-webserv)
- [🏓 Transcendence](#-transcendence)

---

## 📚 Libft
General-purpose C library with custom implementations of standard functions.

---

## 🖨️ ft_printf
Reimplementation of the standard `printf()` function in C.

---

## 📄 Get_next_line
Function that returns a line from a file descriptor.

---

## 🛡️ Born2beroot
Systems administration exercise focused on virtualization and Linux basics.

---

## 🔢 Push_swap
Stack sorting algorithm with minimal operations.

---

## 📡 Minitalk
Data exchange between processes using **UNIX signals**.

---

## 🕸️ FDF
3D wireframe rendering project.

---

## 🤔 Philosophers
Thread synchronization project using **mutexes**.

### ⚠️ Performance Notes
The project initially showed some delays due to message formatting.  
The solution was to simplify the output, adding a `-v` flag to toggle between two modes:

- **Visual mode (less efficient):**
  ```bash
  ./philo -v arg1 arg2 arg3 arg4 [arg5]

- **No visual mode (more eficiente):**
  ```bash
  ./philo arg1 arg2 arg3 arg4 [arg5]

With the -v flag, the program displays the original formatted output. Without it, execution is faster and the algorithm performs better.

---

## 💻 Minishell
Implementation of a simple shell that reproduces basic Bash behavior. Includes process management, redirections, pipes, and built-in commands.

---

## 🌌 MiniRT
Basic ray tracing renderer. Generates realistic images from geometric objects and light sources.

---

## 🌐 NetPractice
Practical networking exercises to understand:
- IP addressing.
- Subnetting.
- Basic routing.

---

## ⚙️ CPP 00–04
C++ modules covering the fundamentals of object-oriented programming:
- Classes and objects.
- Constructors and destructors.
- Operator overloading.
- Encapsulation.

---

## ⚙️ CPP 05–09
Advanced C++ modules with:
- Inheritance and polymorphism.
- Templates.
- Exception handling.
- Abstraction-oriented programming.

---

## 🐳 Inception
System administration project using Docker. Goal: deploy services in containers (WordPress, MariaDB, Nginx) with automated configuration. 
More details in its [readme.md](https://github.com/jlutrera/42Madrid-CommonCore/blob/main/C5_Inception/readme.md)

---

## 🌍 Webserv
Implementation of an HTTP server in C++. 
Supports multiple connections, GET/POST requests, and CGI execution.

---

## 🏓 Transcendence
Full web application for a Pong tournament. Features:
- User authentication.
- Real-time chat.
- Integration with external APIs.
- Modern, responsive interface.

More details in its [readme.md](C6_ft_transcendence/readme.md)

✨ Este es el **último proyecto** del 42 Common Core.

