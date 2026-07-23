# Instalación de Windows Server 2022

## Introducción

En esta fase se realiza la instalación inicial del sistema operativo Windows Server 2024 que será utilizado como servidor principal del laboratorio YVONET.

El objetivo es preparar la máquina virtual para posteriormente configurar los servicios de infraestructura necesarios, como Active Directory y DNS.

---

## Creación de la máquina virtual

La máquina virtual del servidor fue creada utilizando Oracle VirtualBox.

Configuración asignada:

- Sistema operativo: Windows Server 2022
- Nombre del equipo: YVONET
- Memoria RAM: 4 GB
- Procesadores: 2 núcleos
- Almacenamiento: 80 GB

---

## Instalación del sistema operativo

Se realizó una instalación limpia de Windows Server 2022 utilizando la imagen ISO correspondiente.

Durante el proceso se configuraron:

- Idioma y región.
- Particionado del disco virtual.
- Instalación del sistema operativo.
- Creación de la contraseña inicial del administrador local.

### Evidencia 1. Selección del idioma y configuración regional

Antes de iniciar la instalación se seleccionó el idioma, el formato regional y la distribución del teclado.

<a href="../screenshots/03-01-idioma.png">
    <img src="../screenshots/03-01-idioma.png"
         alt="Selección del idioma durante la instalación"
         title="Presione para ampliar"
         width="400">
</a>

*Figura 1. Selección del idioma y configuración regional.*

### Evidencia 2. Selección de la edición

Durante la instalación se seleccionó la edición **Windows Server 2022 Standard Evaluation (Experiencia de escritorio)**.

<a href="../screenshots/03-02-seleccion_edicion.png">
    <img src="../screenshots/03-02-seleccion_edicion.png"
         alt="Selección de la edición de Windows Server 2022"
         title="Presione para ampliar"
         width="400">
</a>

*Figura 2. Selección de la edición de Windows Server 2022.*


## Configuración inicial del servidor

Después de completar la instalación se realizaron las tareas iniciales:

- Inicio de sesión con el usuario administrador local.
- Revisión del estado del sistema.
- Instalación de actualizaciones disponibles.
- Configuración básica del entorno.

### Evidencia 3. Primer inicio de Windows Server

<a href="../screenshots/03-03-primer_inicio.png">
  <img src="../screenshots/03-03-primer_inicio.png"
       alt="Primer inicio de Windows Server 2022"
       title="Presione para ampliar"
       width="400">
</a>

*Figura 3. Primer inicio de Windows Server 2022 tras completar la instalación.*

---

## Identificación del servidor

Se estableció el nombre del equipo: SVR-YVONET

Este nombre permitirá identificar el servidor dentro de la infraestructura del laboratorio.

---

## Estado actual

El servidor Windows Server 2022 queda preparado para continuar con la configuración de red y la instalación de roles necesarios para crear el dominio YVONET.LOCAL.
