\# Uso y Funcionamiento



En esta sección se detallan las configuraciones prácticas para blindar los accesos remotos y filtrar las conexiones entrantes.



\## 1. Configuración del cortafuegos (UFW)



Definimos una política restrictiva por defecto (denegar todo el tráfico entrante y permitir el saliente) y abrimos únicamente los servicios autorizados:



```bash

sudo ufw default deny incoming

sudo ufw default allow outgoing

sudo ufw allow 22/tcp

sudo ufw allow 80/tcp

sudo ufw allow 443/tcp

sudo ufw enable

