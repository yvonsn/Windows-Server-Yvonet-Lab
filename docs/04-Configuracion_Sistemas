# 04. Configuración de los sistemas

## Configuración inicial del servidor

### Introducción

Después de instalar Windows Server 2022 se realizó la configuración inicial del servidor antes de instalar los roles necesarios para la infraestructura **YVONET**.

Esta fase incluye la configuración de red, identificación del equipo y comprobaciones básicas de conectividad dentro del entorno virtualizado.

---

## Configuración de red del servidor

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

El nombre asignado al servidor es:

**SVR-YVONET**

Este nombre permite identificar el equipo dentro de la infraestructura y será utilizado posteriormente como servidor principal del dominio.

**Captura realizada:**

- Nombre del equipo configurado en Windows Server.

---

## Configuración inicial del cliente

Después de instalar el sistema operativo cliente, se realizó la configuración inicial del equipo que formará parte de la infraestructura **YVONET**.

El objetivo de esta configuración es preparar la máquina para su comunicación con el servidor y su posterior incorporación al dominio mediante Active Directory.

---

## Configuración de red del cliente

El equipo cliente se configuró dentro de la misma red interna de VirtualBox utilizada por el servidor.

Esta configuración permite la comunicación directa entre ambos equipos dentro del entorno de laboratorio.

Configuración utilizada:

| Parámetro | Valor |
|---|---|
| Tipo de red VirtualBox | Red interna |
| Red utilizada | 192.168.10.0/24 |
| Dirección IP | 192.168.10.20 |
| Máscara de red | 255.255.255.0 |
| Puerta de enlace | No configurada |
| Servidor DNS preferido | 192.168.10.10 |

El servidor DNS se establece apuntando al servidor **SVR-YVONET**, ya que posteriormente será el encargado de gestionar la resolución de nombres del dominio **YVONET.LOCAL**.

---

## Identificación del cliente

El nombre asignado al equipo cliente es:

**PC-YVONET01**

Este nombre permite identificar la máquina dentro de la infraestructura y facilitará su administración una vez sea agregada al dominio.

**Captura realizada:**

- Nombre del equipo cliente configurado en Windows.

---

# Comprobaciones de conectividad

Una vez configurados ambos equipos, se realizó una prueba de comunicación para comprobar que existe conectividad dentro de la red interna.

La prueba se realizó desde el equipo cliente hacia el servidor mediante el comando:

```cmd
ping 192.168.10.10
