# Introducción y Arquitectura

La administración segura de servidores Linux es un pilar crítico en cualquier infraestructura IT moderna. Un sistema recién instalado suele incluir servicios innecesarios o configuraciones por defecto orientadas a la compatibilidad más que a la seguridad.

## Principios fundamentales del Hardening

1. **Principio de mínimo privilegio:** Cada usuario y servicio debe disponer únicamente de los permisos estrictamente necesarios.
2. **Reducción de la superficie de ataque:** Desactivar puertos, demonios y paquetes que no cumplan una función activa.
3. **Defensa en profundidad:** Combinar múltiples capas de seguridad (cortafuegos, autenticación por clave pública y monitorización de registros).

## Esquema de arquitectura segura

En el siguiente diagrama se muestra el flujo de filtrado de tráfico antes de alcanzar los servicios internos del servidor:

![Esquema de arquitectura del servidor](img/arquitectura.png)

??? note "Ver detalles sobre los puertos estándar monitorizados"
    * **Puerto 22/TCP (SSH):** Administración remota cifrada (se recomienda cambiarlo a un puerto alto no estándar).
    * **Puerto 80/TCP (HTTP):** Tráfico web inicial redirigido automáticamente a HTTPS.
    * **Puerto 443/TCP (HTTPS):** Tráfico web cifrado mediante certificados TLS.

Para ampliar información oficial sobre estándares de seguridad, consulta la [documentación oficial de Ubuntu Server](https://ubuntu.com/server/docs).
