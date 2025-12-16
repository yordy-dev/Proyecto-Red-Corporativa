# VPN de Acceso Remoto

## Tipo de VPN
Implementé una VPN IPsec de acceso remoto.

## Objetivo
Permitir que usuarios externos puedan conectarse de forma segura a la red
corporativa desde ubicaciones remotas, garantizando confidencialidad e
integridad de la información.

## Funcionamiento
- El router actúa como servidor VPN.
- Los usuarios se autentican mediante credenciales locales.
- Se asignan direcciones IP dinámicas desde el pool 172.16.100.0/24.
- Todo el tráfico entre el cliente remoto y la red interna se transmite
  cifrado.

## Seguridad
Utilicé cifrado AES y autenticación mediante clave precompartida para asegurar
la comunicación.
