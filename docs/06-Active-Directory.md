# Instalación y configuración de Active Directory

## Introducción

Una vez finalizada la configuración inicial del servidor, se procedió a instalar el rol **Active Directory Domain Services (AD DS)**.

Este servicio permite administrar de forma centralizada usuarios, equipos, grupos y recursos de una red empresarial.

---

## Instalación del rol AD DS

La instalación se realizó desde el **Administrador del servidor** mediante el asistente **Agregar roles y características**.

Rol instalado:

- Active Directory Domain Services (AD DS)

Durante la instalación también se añadieron automáticamente las herramientas de administración necesarias.

---

## Promoción del servidor

Una vez instalado el rol, el servidor fue promovido a **Controlador de Dominio**.

Se creó un nuevo bosque con el dominio:

```
YVONET.LOCAL
```

El servidor pasó a ser el primer controlador de dominio de la infraestructura.

---

## Configuración del dominio

Configuración utilizada:

| Parámetro | Valor |
|---|---|
| Dominio | YVONET.LOCAL |
| Servidor | SVR-YVONET |
| Tipo | Nuevo bosque |
| DNS | Instalado junto con AD DS |

---

## Reinicio del servidor

Después de finalizar la promoción del controlador de dominio, el servidor se reinició automáticamente para aplicar la nueva configuración.

A partir de este momento el inicio de sesión pasó a realizarse utilizando las credenciales del dominio.

---

## Comprobaciones realizadas

Tras completar la instalación se verificó:

- Correcta instalación de Active Directory.
- Funcionamiento del servicio DNS.
- Acceso a las herramientas administrativas.
- Correcto funcionamiento del controlador de dominio.

---

## Comandos utilizados

### Información de red

```cmd
ipconfig /all
```

Permite verificar la configuración IP y el servidor DNS.

### Comprobación del nombre del equipo

```cmd
hostname
```

Muestra el nombre del servidor.

### Verificación del dominio

```cmd
whoami
```

Permite comprobar el usuario autenticado en el dominio.

---

## Resultado

El servidor quedó configurado como controlador de dominio de **YVONET.LOCAL**, preparado para la creación de usuarios, grupos y unidades organizativas.
