---
title: Plantillas
status: active
tags: [templates, contribution]
---

# Plantillas

Estas plantillas definen la estructura minima de cada tipo de pagina.

## Metadatos comunes

```yaml
---
title: Nombre legible
slug: identificador-estable
status: draft # draft | reviewed | verified | experimental
last_reviewed: YYYY-MM-DD
evidence:
  - official-documentation
  - technical-data-sheet
  - safety-data-sheet
  - workshop-manual
  - own-test
  - professional-consensus
tags: []
---
```

## Tipos de ficha

- [Producto quimico](chemical.md)
- [Lubricante o grasa](lubricant.md)
- [Procedimiento](procedure.md)
- [Vehiculo o componente](vehicle.md)

!!! note
    Los metadatos deben describir hechos estables y estructurables. Las explicaciones, advertencias y matices pertenecen al cuerpo del documento.
