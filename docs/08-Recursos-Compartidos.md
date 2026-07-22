# Recursos compartidos

## Introducción

Una vez creada la estructura del dominio y configurados los usuarios, se procedió a crear los recursos compartidos que utilizarían los distintos departamentos de la empresa **YVONET**.

Los recursos compartidos permiten que varios usuarios accedan a la misma información desde diferentes equipos de la red.

---

## Objetivo

Crear una estructura organizada de carpetas compartidas para cada departamento de la empresa y preparar el entorno para la posterior asignación de permisos NTFS.

---

## Procedimiento

Se creó una carpeta principal denominada:

```text
C:\Departamentos
```

Dentro de ella se crearon las siguientes subcarpetas:

```text
Departamentos
│
├── Archivo
├── Personal
├── Seguridad
├── Administración
└── RRHH
```

Posteriormente se compartió la carpeta **Departamentos** para permitir el acceso desde los equipos pertenecientes al dominio.

La configuración de los permisos específicos se realizó posteriormente mediante permisos NTFS.

---

## Herramientas utilizadas

- Explorador de archivos de Windows
- Server Manager
- Administración de carpetas compartidas

---

## Comandos utilizados

Durante este procedimiento no fue necesario utilizar comandos desde la consola.

Toda la configuración se realizó mediante las herramientas gráficas de Windows Server.

#### **Nota:** Aunque la configuración se realizó mediante la interfaz gráfica de Windows Server, la administración de recursos compartidos también puede realizarse mediante PowerShell, una opción habitual en entornos empresariales.
---

## Resultado

La infraestructura quedó preparada para que los distintos departamentos pudieran acceder a los recursos compartidos una vez configurados los permisos correspondientes.

---

## Evidencias

Las capturas de pantalla de esta configuración se incorporarán en una revisión posterior del proyecto.
