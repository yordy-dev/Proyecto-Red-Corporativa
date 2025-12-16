# Arquitectura de la Red Corporativa

## Objetivo
En este proyecto diseñé e implementé una red corporativa segmentada mediante
VLANs, con enrutamiento inter-VLAN, servicios de red y controles básicos de
seguridad, simulando un entorno empresarial real.

## Topología
La red está compuesta por:
- 1 Router Cisco configurado como Router-on-a-Stick
- 1 Switch Layer 2
- 4 VLANs correspondientes a diferentes áreas de la empresa

## VLANs Implementadas
- VLAN 10: Administración
- VLAN 20: Ventas
- VLAN 30: Invitados
- VLAN 40: TI

## Diseño de Red
Conecté el router al switch mediante un enlace trunk 802.1Q.  
El enrutamiento entre VLANs se realiza a través de subinterfaces configuradas
en el router, permitiendo la comunicación controlada entre los distintos
segmentos de la red.

## Direccionamiento IP
| VLAN|      Área      |      Red      |  Gateway   |
|-----|----------------|---------------|------------|
| 10  | Administración | 10.10.10.0/24 | 10.10.10.1 |
| 20  | Ventas         | 10.10.20.0/24 | 10.10.20.1 |
| 30  | Invitados      | 10.10.30.0/24 | 10.10.30.1 |
| 40  | TI             | 10.10.40.0/24 | 10.10.40.1 |
