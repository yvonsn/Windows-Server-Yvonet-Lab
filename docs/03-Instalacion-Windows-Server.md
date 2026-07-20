# Instalación de Windows Server 2024

## Introducción

En esta fase se realiza la instalación inicial del sistema operativo Windows Server 2024 que será utilizado como servidor principal del laboratorio YVONET.

El objetivo es preparar la máquina virtual para posteriormente configurar los servicios de infraestructura necesarios, como Active Directory y DNS.

---

## Creación de la máquina virtual

La máquina virtual del servidor fue creada utilizando Oracle VirtualBox.

Configuración asignada:

- Sistema operativo: Windows Server 2024
- Nombre del equipo: SVR-YVONET
- Memoria RAM: 4 GB
- Procesadores: 2 núcleos
- Almacenamiento: 80 GB

---

## Instalación del sistema operativo

Se realizó una instalación limpia de Windows Server 2024 utilizando la imagen ISO correspondiente.

Durante el proceso se configuraron:

- Idioma y región.
- Particionado del disco virtual.
- Instalación del sistema operativo.
- Creación de la contraseña inicial del administrador local.

---

## Configuración inicial del servidor

Después de completar la instalación se realizaron las tareas iniciales:

- Inicio de sesión con el usuario administrador local.
- Revisión del estado del sistema.
- Instalación de actualizaciones disponibles.
- Configuración básica del entorno.

---

## Identificación del servidor

Se estableció el nombre del equipo: SVR-YVONET

Este nombre permitirá identificar el servidor dentro de la infraestructura del laboratorio.

---

## Estado actual

El servidor Windows Server 2024 queda preparado para continuar con la configuración de red y la instalación de roles necesarios para crear el dominio YVONET.LOCAL.
