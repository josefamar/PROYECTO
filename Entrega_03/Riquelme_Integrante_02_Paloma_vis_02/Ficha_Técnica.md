# Ficha Técnica 

**Fuente:** Empresa de Ferrocarriles del Estado (EFE) – Anuarios 2019–2024  
**Cobertura temporal:** 2019–2024  
**Cobertura geográfica:** Nacional (Chile)

## Variables incorporadas

| Variable | Descripción |
|-----------|--------------|
| categoria | Clasificación de edad, franja horaria o día de la semana |
| fallecidos_año | Número de fallecidos por tipo y año |
| graves_año | Número de heridos graves por tipo y año |
| leves_año | Número de heridos leves por tipo y año |
| estado | Indica si hubo o no registros ese año ("Con registros" / "Sin accidentes reportados") |

## Observaciones
- El año **2021** y algunos valores intermedios aparecen con cero, debido a ausencia de registros oficiales. Esto fue señalado explícitamente como **“Sin accidentes reportados”** en la visualización.
- Las bases no comparten columna de unión, por lo tanto, se trabajaron **por separado** (edad, horario y día) como conjuntos individuales de datos.

