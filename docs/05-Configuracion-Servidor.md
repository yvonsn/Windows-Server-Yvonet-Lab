# Configuración inicial del servidor

## Introducción

Después de instalar Windows Server 2022 se realizó la configuración inicial del servidor antes de instalar los roles necesarios para la infraestructura YVONET.

Esta fase incluye la configuración de red, identificación del equipo y comprobaciones básicas de conectividad.

---

## Configuración de red

Para el laboratorio se utilizó una red interna de VirtualBox.

Este tipo de configuración permite la comunicación entre las máquinas virtuales del laboratorio sin exponerlas directamente a la red externa.

Configuración utilizada:

| Parámetro | Valor |
|---|---|
| Tipo de red VirtualBox | Red interna |
| Red utilizada | 192.168.10.0/24 |
| Dirección IP | 192.168.10.10 |
| Máscara de red | 255.255.255.0 |
| Puerta de enlace | No configurada |

---

## Identificación del servidor

El nombre asignado al servidor es: SVR-YVONET

Este nombre permite identificar el equipo dentro de la infraestructura y será utilizado posteriormente como servidor principal del dominio.

---

## Comprobaciones realizadas

Se realizaron comprobaciones básicas para verificar el correcto funcionamiento de la configuración:

- Verificación de la configuración IP mediante `ipconfig`.
- Comprobación de comunicación entre máquinas virtuales.
- Validación de la conectividad dentro de la red interna.

---

## Estado actual

El servidor queda preparado para la instalación y configuración de los servicios de infraestructura:

- Active Directory Domain Services (AD DS).
- DNS.
- Dominio YVONET.LOCAL.
