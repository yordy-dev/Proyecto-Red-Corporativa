# Seguridad y Segmentación de la Red

## Enfoque de Seguridad
Implementé una estrategia de seguridad basada en segmentación por VLANs
combinada con ACLs extendidas, con el objetivo de limitar el acceso entre
departamentos según su función.

## Políticas Aplicadas
- Administración tiene acceso completo a todos los segmentos.
- TI tiene acceso completo para tareas de soporte y monitoreo.
- Ventas no puede acceder a las VLAN de Administración ni de TI.
- Invitados no tiene acceso a ninguna red interna.

## Implementación
Las ACLs fueron configuradas como listas extendidas y aplicadas en sentido
inbound sobre las subinterfaces del router, siguiendo buenas prácticas de
seguridad en redes empresariales.
