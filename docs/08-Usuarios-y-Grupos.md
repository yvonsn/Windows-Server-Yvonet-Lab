# Administración de usuarios y grupos

## Introducción

Una vez creada la estructura organizativa del dominio **YVONET.LOCAL**, se procedió a crear las cuentas de usuario necesarias para representar los distintos departamentos de la empresa.

La administración de usuarios mediante Active Directory permite gestionar el acceso a los recursos de forma centralizada y segura.

---

## Usuarios creados

| Unidad Organizativa | Usuarios |
|---|---|
| Archivo | Leo, Chispita |
| Personal | Negro, Samba |
| Seguridad | Nina |
| Administración | Qori |
| RRHH | Chaska |

Cada usuario fue ubicado dentro de la Unidad Organizativa correspondiente.

---

## Organización de usuarios

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

---

## Administración de grupos

Se utilizaron grupos de seguridad para facilitar la asignación de permisos sobre los recursos compartidos.

Esta metodología permite administrar el acceso a los recursos mediante grupos, evitando asignar permisos directamente a cada usuario.

---

## Buenas prácticas aplicadas

Durante la configuración se siguieron las siguientes recomendaciones:

- Organizar los usuarios por departamentos mediante OU.
- Utilizar grupos de seguridad para la asignación de permisos.
- Mantener una estructura clara y fácil de administrar.
- Facilitar el crecimiento futuro del dominio.

---

## Herramientas utilizadas

- Server Manager
- Active Directory Users and Computers

---

## Comandos utilizados

### Comprobar el usuario autenticado

```cmd
whoami
```

### Comprobar el nombre del equipo

```cmd
hostname
```

---

## Resultado

La infraestructura quedó preparada para administrar el acceso a los recursos compartidos mediante usuarios y grupos de seguridad.
