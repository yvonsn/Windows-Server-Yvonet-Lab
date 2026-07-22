# Configuración de permisos NTFS

## Introducción

Después de crear los recursos compartidos de la empresa YVONET, se procedió a configurar los permisos NTFS para controlar el acceso de los usuarios a las carpetas departamentales.

Los permisos NTFS permiten establecer qué acciones puede realizar cada usuario sobre los archivos y carpetas almacenados en el servidor.

---

## Objetivo

Configurar el acceso a las carpetas departamentales asignando permisos específicos según el usuario y el departamento correspondiente.

---

## Estructura de carpetas

La estructura utilizada fue:

```text
C:\Departamentos

├── Archivo
├── Personal
├── Seguridad
├── Administración
└── RRHH
```

---

## Usuarios y permisos asignados

Los permisos se asignaron directamente sobre cada carpeta departamental y sobre los usuarios correspondientes, con el objetivo de garantizar el acceso correcto a cada recurso.

| Carpeta | Usuarios con acceso |
|---|---|
| Archivo | Leo, Chispita |
| Personal | Negro, Samba |
| Seguridad | Nina |
| Administración | Qori |
| RRHH | Chaska |

---

## Permisos aplicados

Los permisos NTFS fueron configurados utilizando las opciones disponibles en Windows Server:

- Modificar
- Lectura y ejecución
- Mostrar el contenido de la carpeta
- Lectura
- Escritura

Estos permisos permiten controlar las acciones que cada usuario puede realizar sobre los archivos y carpetas del servidor.

La asignación se realizó de forma individual sobre cada carpeta departamental y cada usuario debido a los problemas encontrados durante la configuración inicial.

---

## Procedimiento realizado

La configuración se realizó mediante:

**Propiedades de carpeta → Seguridad → Editar permisos**

Para cada carpeta departamental se añadieron los usuarios correspondientes y se asignaron los permisos necesarios.

---

## Pruebas realizadas

La validación se realizó desde el equipo cliente Windows 11 iniciando sesión con diferentes usuarios del dominio.

Pruebas realizadas:

- Acceso a carpetas compartidas.
- Verificación de permisos asignados.
- Comprobación de capacidad de lectura y modificación.

Durante la práctica se realizaron pruebas completas con algunos usuarios y posteriormente se continuó con la revisión del resto de accesos.

---

## Incidencias encontradas

Durante la configuración inicial surgieron problemas relacionados con el acceso a determinadas carpetas.

Fue necesario revisar:

- Permisos asignados.
- Usuarios autorizados.
- Configuración de seguridad de las carpetas.

Como solución se procedió a revisar y asignar los permisos directamente sobre cada carpeta y usuario.

---

## Herramientas utilizadas

- Explorador de archivos de Windows Server.
- Propiedades de seguridad de carpetas.
- Equipo cliente Windows 11.

---

## Comandos utilizados

Durante esta configuración no se utilizaron comandos.

La administración se realizó mediante la interfaz gráfica de Windows.

---

## Resultado

Los usuarios quedaron configurados con acceso controlado a los recursos departamentales, permitiendo simular una estructura empresarial con diferentes niveles de acceso.
