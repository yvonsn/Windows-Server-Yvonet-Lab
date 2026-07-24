# 07. Usuarios y Grupos

## Administración de usuarios y grupos

### Introducción

Una vez creada la estructura organizativa del dominio **YVONET.LOCAL**, se procedió a crear las cuentas de usuario necesarias para representar los distintos departamentos de la empresa.

La administración de usuarios mediante **Active Directory** permite gestionar de forma centralizada el acceso a los recursos de la organización, mejorando la seguridad y facilitando la administración del dominio.

---

# Creación de usuarios

Se creó un conjunto de usuarios distribuidos entre las diferentes Unidades Organizativas definidas previamente.

La siguiente tabla muestra la organización de los usuarios:

| Unidad Organizativa | Usuarios |
|---------------------|----------|
| Archivo | Leo, Chispita |
| Personal | Negro, Samba |
| Seguridad | Nina |
| Administración | Qori |
| RRHH | Chaska |

Cada usuario fue creado utilizando la consola **Usuarios y equipos de Active Directory** y ubicado dentro de la Unidad Organizativa correspondiente.

---

## Captura de creación de un usuario

**Imagen 07.1 - Creación de un usuario en Active Directory**

![Creación de usuario](capturas/crear-usuario.png)

---

# Organización de los usuarios

La estructura del dominio quedó organizada de la siguiente manera:

```text
YVONET.LOCAL
│
├── Archivo
│   ├── Leo
│   └── Chispita
│
├── Personal
│   ├── Negro
│   └── Samba
│
├── Seguridad
│   └── Nina
│
├── Administración
│   └── Qori
│
└── RRHH
    └── Chaska
```

Esta organización facilita la administración y localización de los usuarios dentro del dominio.

---

## Captura de la estructura de usuarios

**Imagen 07.2 - Usuarios organizados por Unidades Organizativas**

![Usuarios por OU](capturas/usuarios-ou.png)

---

# Creación de grupos de seguridad

Además de los usuarios, se crearon grupos de seguridad para administrar el acceso a los recursos compartidos.

La utilización de grupos permite asignar permisos de forma más eficiente, evitando configurar permisos individualmente para cada usuario.

Los grupos se organizaron según las necesidades de cada departamento y posteriormente se utilizarán para controlar el acceso a las carpetas compartidas del servidor.

---

## Captura de creación de un grupo

**Imagen 07.3 - Creación de un grupo de seguridad**

![Creación de grupo](capturas/crear-grupo.png)

---

# Buenas prácticas aplicadas

Durante la configuración se siguieron las siguientes recomendaciones:

- Organizar los usuarios por departamentos mediante Unidades Organizativas.
- Utilizar grupos de seguridad para la asignación de permisos.
- Evitar asignar permisos directamente a usuarios individuales.
- Mantener una estructura clara y fácilmente administrable.
- Facilitar el crecimiento futuro de la infraestructura.

---

# Herramientas utilizadas

Para la creación y administración de usuarios y grupos se utilizaron las siguientes herramientas:

- Administrador del servidor (Server Manager).
- Usuarios y equipos de Active Directory.

---

# Comandos utilizados

## Comprobar el usuario autenticado

```cmd
whoami
```

Permite verificar el usuario con el que se ha iniciado sesión en el dominio.

---

## Comprobar el nombre del equipo

```cmd
hostname
```

Permite comprobar el nombre del equipo desde el que se está trabajando.

---

# Evidencias de configuración

Durante la administración de usuarios y grupos se recopilaron las siguientes capturas:

| Captura | Descripción |
|----------|-------------|
| Imagen 07.1 | Creación de un usuario mediante Active Directory. |
| Imagen 07.2 | Organización de los usuarios dentro de las Unidades Organizativas. |
| Imagen 07.3 | Creación de un grupo de seguridad. |

---

# Resultado

El dominio **YVONET.LOCAL** quedó configurado con los usuarios y grupos necesarios para representar la estructura de la empresa.

La organización mediante Unidades Organizativas y grupos de seguridad facilitará la administración de permisos y el acceso a los recursos compartidos, permitiendo una gestión centralizada, ordenada y segura de toda la infraestructura.

El siguiente paso consistirá en la creación y configuración de los **recursos compartidos** del servidor.
