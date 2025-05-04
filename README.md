# Proyecto de Red con Subredes y Servidor de Intranet

Equipo 3
Curso: IMPL SOLUC PLATAF MULTIUSUARIO

Integrantes:
ERIK MAGBIS LEONARDO CALLE
CARLOS WOLLEY LA TORRE MACHADO
CARLOS ALBERTO ACEDO RUGEL
RENATO LUIS YANAMANGO CASANA

Este proyecto simula una red dividida en múltiples subredes con control de acceso y un servidor de intranet accesible desde todas las subredes. Se utilizó **Cisco Packet Tracer** para la implementación.


## 📌 Objetivos

- Dividir la red en subredes controladas por VLANs.
- Permitir comunicación entre routers usando RIP.
- Conectar un servidor de intranet accesible desde todas las subredes.
- Restringir comunicación entre subredes excepto hacia el servidor.

## 🔧 Tecnologías y herramientas

- Cisco Packet Tracer
- Calculadora de subredes (https://www.subnet-calculator.com/)
- Routers y switches Cisco
- Servidor local (para la intranet)

## 📁 Estructura de la red

- **Router 1**: 5 subredes
- **Router 2**: 5 subredes + 1 red pública para la intranet
- **RIP v2** habilitado para el enrutamiento dinámico entre routers
- **ACLs** aplicadas para restringir comunicación entre subredes

## 🖥️ Configuración del servidor

- IP: `192.168.3.194`
- Gateway: `192.168.3.193`
- Servicio: HTTP (Intranet)

## 🔄 Configuración básica RIP

```bash
router rip
version 2
network 192.168.20.0
network 192.168.30.0
