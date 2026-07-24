# 06. Unidades Organizativas (OU)

## Creación de Unidades Organizativas (OU)

### Introducción

Una vez configurado el dominio **YVONET.LOCAL**, se procedió a organizar la estructura lógica de la empresa mediante la creación de **Unidades Organizativas (Organizational Units - OU)**.

Las Unidades Organizativas permiten organizar usuarios, grupos y equipos de forma estructurada, facilitando la administración de los recursos del dominio y la aplicación de directivas de grupo (GPO).

---

# Estructura de la empresa

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

Cada Unidad Organizativa representa un departamento de la empresa y servirá como contenedor para los usuarios, grupos y equipos correspondientes.

---

# Procedimiento

Las Unidades Organizativas fueron creadas utilizando la consola:

```text
Usuarios y equipos de Active Directory
```

El procedimiento realizado fue el siguiente:

1. Abrir la consola **Usuarios y equipos de Active Directory**.
2. Seleccionar el dominio **YVONET.LOCAL**.
3. Hacer clic con el botón derecho sobre el dominio.
4. Seleccionar **Nuevo → Unidad organizativa**.
5. Introducir el nombre de la Unidad Organizativa.
6. Repetir el proceso para cada uno de los departamentos definidos.

---

## Captura de creación de las Unidades Organizativas

**Imagen 06.1 - Creación de una Unidad Organizativa**

![Creación de una OU](capturas/crear-ou.png)

---

# Organización del dominio

Una vez creadas todas las Unidades Organizativas, la estructura del dominio quedó organizada de la siguiente manera:

```text
YVONET.LOCAL
│
├── Archivo
├── Personal
├── Seguridad
├── RRHH
└── Administración
```

Esta organización facilitará la administración de usuarios, grupos y equipos dentro del dominio.

---

## Captura de la estructura del dominio

**Imagen 06.2 - Estructura de las Unidades Organizativas**

![Estructura de las OU](capturas/estructura-ou.png)

---

# Objetivos de las Unidades Organizativas

La utilización de Unidades Organizativas proporciona las siguientes ventajas:

- Organizar los diferentes departamentos de la empresa.
- Facilitar la administración de usuarios y equipos.
- Organizar los grupos de seguridad.
- Permitir la aplicación de directivas de grupo (GPO).
- Mejorar la organización y el mantenimiento del dominio.

---

# Herramienta utilizada

Para la creación y administración de las Unidades Organizativas se utilizó la consola:

```text
Usuarios y equipos de Active Directory
```

Esta herramienta permite administrar todos los objetos del dominio, incluyendo usuarios, grupos, equipos y Unidades Organizativas.

---

# Evidencias de configuración

Durante la creación de la estructura organizativa se obtuvieron las siguientes capturas:

| Captura | Descripción |
|----------|-------------|
| Imagen 06.1 | Creación de una Unidad Organizativa mediante la consola Usuarios y equipos de Active Directory. |
| Imagen 06.2 | Estructura completa de las Unidades Organizativas creadas en el dominio YVONET.LOCAL. |

---

# Resultado

El dominio **YVONET.LOCAL** quedó organizado mediante las siguientes Unidades Organizativas:

- Archivo
- Personal
- Seguridad
- RRHH
- Administración

Esta estructura constituye la base para la administración centralizada del dominio y permitirá, en los siguientes apartados, crear usuarios, grupos y aplicar políticas específicas a cada departamento.

El siguiente paso consistirá en la creación y administración de los **usuarios y grupos** del dominio.
