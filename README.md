# Tickets
Ticket App

## Estados del ticket y transiciones permitidas
- **Abierto**: creado y pendiente de clasificación o asignación.
- **En Proceso**: asignado y en atención.
- **Cerrado**: resuelto y finalizado (puede habilitar encuesta).

Transiciones permitidas:
- **Abierto ➜ En Proceso**
- **En Proceso ➜ Cerrado**
- **Cerrado ➜ En Proceso** (reapertura)

## Roles
- **Colaborador**: crea y consulta tickets.
- **TI**: atiende, asigna y cambia el estado de los tickets.

## Permisos por rol
| Acción | Colaborador | TI |
| --- | --- | --- |
| Crear | ✅ | ✅ |
| Comentar | ✅ | ✅ |
| Adjuntar | ✅ | ✅ |
| Cerrar | ❌ | ✅ |
| Reabrir | ❌ | ✅ |
| Asignar | ❌ | ✅ |

## Métricas del dashboard general
- Conteo por estado (Abierto, En Proceso, Cerrado).
- Cumplimiento de SLA (porcentaje dentro/fuera de plazo).
- Tiempo medio de resolución.
- Backlog (tickets abiertos y en proceso).

## Flujo del ticket
Creación ➜ Clasificación ➜ Asignación ➜ Atención ➜ Cierre ➜ Encuesta
