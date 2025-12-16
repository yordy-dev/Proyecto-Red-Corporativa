# Monitoreo de Red con SNMP

## Protocolo Utilizado
Configuré SNMP versión 2c en modo solo lectura.

## Objetivo
Implementé SNMP para monitorear el estado del router y las interfaces de red,
permitiendo una supervisión básica del rendimiento y la disponibilidad del
sistema.

## Información Monitoreada
- Estado de las interfaces
- Disponibilidad del router
- Tráfico de red
- Eventos de subida y caída de enlaces (traps)

## Control de Acceso
Restringí el acceso SNMP mediante una ACL que permite únicamente consultas
desde la VLAN de TI.
