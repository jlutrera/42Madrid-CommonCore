# 🚀 42 Common Core Projects

Este repositorio recopila los proyectos realizados durante el **42 Common Core**.  
Cada proyecto aborda un área distinta de programación, sistemas y algoritmos.

---

## 📑 Table of Contents
- [📚 Libft](#-libft)
- [🖨️ ft_printf](#️-ft_printf)
- [📄 get_next_line](#-get_next_line)
- [🛡️ Born2beroot](#️-born2beroot)
- [🔢 push_swap](#-push_swap)
- [📡 Minitalk](#-minitalk)
- [🕸️ FDF](#-fdf)
- [🤔 Philosophers](#-philosophers)
- [💻 minishell](#-minishell)
- [🌌 miniRT](#-minirt)
- [🌐 NetPractice](#-netpractice)
- [⚙️ CPP 00–04](#️-cpp-0004)
- [⚙️ CPP 05–09](#️-cpp-0509)
- [🐳 Inception](#-inception)
- [🌍 webserv](#-webserv)
- [🏓 ft_transcendence](#-ft_transcendence)

---

## 📚 Libft
General-purpose C library with custom implementations of standard functions.

---

## 🖨️ ft_printf
Reimplementation of the standard `printf()` function in C.

---

## 📄 get_next_line
Function that returns a line from a file descriptor.

---

## 🛡️ Born2beroot
Systems administration exercise focused on virtualization and Linux basics.

---

## 🔢 push_swap
Stack sorting algorithm with minimal operations.

---

## 📡 Minitalk
Data exchange between processes using **UNIX signals**.

---

## 🕸️ FDF
3D wireframe rendering project.

---

## 🤔 Philosophers
Proyecto de sincronización de **hilos** y uso de **mutex**.

### ⚠️ Notas de rendimiento
El proyecto presentaba cierto retraso en la ejecución debido al formato de los mensajes.  
La solución fue simplificar la salida, añadiendo un flag `-v` para alternar entre los dos modos:

- **Modo con formato (menos eficiente):**
  ```bash
  ./philo -v arg1 arg2 arg3 arg4 [arg5]
- **Modo sin formato (más eficiente):**
  ```bash
  ./philo arg1 arg2 arg3 arg4 [arg5]

Con el flag -v se muestra el programa con el formato original. Sin este flag, el programa gana en eficiencia y el algoritmo funciona mejor.

---

## 💻 minishell
Implementación de un **shell simple** que reproduce el comportamiento básico de Bash.  
Incluye gestión de procesos, redirecciones, pipes y comandos internos.

---

## 🌌 miniRT
Renderizador básico de escenas 3D mediante **ray tracing**.  
Permite generar imágenes realistas a partir de objetos geométricos y fuentes de luz.

---

## 🌐 NetPractice
Ejercicios prácticos de **networking** para comprender:
- Direccionamiento IP.
- Subnetting.
- Enrutamiento básico.

---

## ⚙️ CPP 00–04
Módulos de C++ que cubren los fundamentos de la **programación orientada a objetos**:
- Clases y objetos.
- Constructores y destructores.
- Sobrecarga de operadores.
- Encapsulación.

---

## ⚙️ CPP 05–09
Módulos avanzados de C++ con:
- **Herencia** y polimorfismo.
- Templates.
- Manejo de excepciones.
- Programación más orientada a abstracción.

---

## 🐳 Inception
Proyecto de administración de sistemas utilizando **Docker**.  
Objetivo: desplegar servicios en contenedores (WordPress, MariaDB, Nginx) con configuración automatizada.
Tienes más contenido en su [readme.md](https://github.com/jlutrera/42Madrid-CommonCore/blob/main/C5_Inception/readme.md)

---

## 🌍 webserv
Implementación de un **servidor HTTP** en C++.  
Compatible con múltiples conexiones, manejo de peticiones GET/POST y soporte para CGI.

---

## 🏓 ft_transcendence
Aplicación web completa para un **torneo de Pong**.  
Incluye:
- Autenticación de usuarios.
- Chat en tiempo real.
- Integración con API externas.
- Interfaz moderna y responsive.

Tienes más información en su [readme.md](C6_ft_transcendence/readme.md)

✨ Este es el **último proyecto** del 42 Common Core.

