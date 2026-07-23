# Creación de Unidades Organizativas (OU)

## Introducción

Una vez configurado el dominio **YVONET.LOCAL**, se procedió a organizar la estructura lógica de la empresa mediante la creación de **Unidades Organizativas (Organizational Units - OU)**.

Las OU permiten organizar usuarios, grupos y equipos de forma estructurada, facilitando la administración y la aplicación de políticas en entornos empresariales.

---

## Estructura de la empresa

Para el laboratorio se definieron las siguientes Unidades Organizativas:

```text
YVONET.LOCAL
│
├── Archivo
├── Personal
├── Seguridad
├── RRHH
└── Administración
```

---

## Procedimiento

Las OU fueron creadas utilizando la consola:

**Active Directory Users and Computers**

Ruta:

```
YVONET.LOCAL
```

Posteriormente se creó una Unidad Organizativa para cada departamento de la empresa.

---

## Objetivo

La organización mediante OU permite:

- Separar los distintos departamentos.
- Facilitar la administración de usuarios.
- Organizar grupos de seguridad.
- Aplicar políticas de grupo (GPO) en el futuro.
- Mejorar la administración del dominio.

---

## Resultado

El dominio quedó organizado en distintas Unidades Organizativas, proporcionando una estructura clara para la administración de usuarios y recursos.

---

## Herramienta utilizada

- Active Directory Users and Computers
