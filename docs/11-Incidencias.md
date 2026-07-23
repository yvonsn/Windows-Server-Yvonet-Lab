# Incidencias y resolución de problemas

## Introducción

Durante la implementación del laboratorio YVONET se produjeron algunas incidencias relacionadas con la configuración del entorno virtual y la administración de permisos.

La resolución de estos problemas permitió comprender la importancia del diagnóstico paso a paso en la administración de sistemas.

---

# Incidencia 1: Problemas de virtualización con VirtualBox

## Descripción del problema

Durante la instalación y configuración del laboratorio mediante VirtualBox aparecieron problemas al iniciar correctamente las máquinas virtuales.

El entorno estaba configurado sobre un equipo físico con Windows 11.

---

## Entorno afectado

Equipo físico:

- Sistema operativo: Windows 11
- Hipervisor utilizado: VirtualBox

Máquinas virtuales:

- Windows Server
  - RAM: 4 GB
  - CPU: 2 núcleos
  - Disco: 80 GB

- Windows 11 Cliente
  - RAM: 4 GB
  - CPU: 2 núcleos
  - Disco: 64 GB

---

## Diagnóstico realizado

Se realizaron las siguientes comprobaciones:

- Verificación de virtualización VT-x/AMD-V en BIOS.
- Revisión de la configuración de VirtualBox.
- Revisión de características de virtualización activadas en Windows.

---

## Solución aplicada

Se identificó que una característica de Windows estaba interfiriendo con VirtualBox.

Después de desactivar la opción correspondiente desde:

```
Panel de control
→ Programas
→ Activar o desactivar las características de Windows
```

las máquinas virtuales pudieron funcionar correctamente.

---

# Incidencia 2: Problemas con permisos de carpetas compartidas

## Descripción del problema

Durante las pruebas de acceso a los recursos compartidos algunos usuarios no podían acceder correctamente a las carpetas asignadas.

---

## Diagnóstico realizado

Se revisaron:

- Usuarios configurados en Active Directory.
- Permisos NTFS.
- Configuración de seguridad de las carpetas.
- Acceso desde el equipo cliente Windows 11.

---

## Solución aplicada

Se ajustaron los permisos directamente sobre cada carpeta y usuario hasta conseguir el acceso esperado.

---

## Pruebas realizadas

Se realizaron comprobaciones desde el cliente Windows 11 utilizando usuarios del dominio.

Se verificó:

- Acceso a recursos compartidos.
- Permisos de lectura.
- Permisos de escritura y modificación.

---

## Herramientas utilizadas

- VirtualBox
- Windows 11
- Windows Server
- Active Directory Users and Computers
- Propiedades de seguridad de carpetas

---

## Comandos utilizados

Durante la resolución se utilizaron comandos de comprobación de red:

```cmd
ping
```

Para verificar la comunicación entre equipos.

```cmd
ipconfig
```

Para revisar la configuración de red.

---

## Resultado

Las incidencias fueron resueltas mediante un proceso de diagnóstico y comprobación, dejando el laboratorio operativo y preparado para continuar con la administración del dominio YVONET.LOCAL.
