---
title: Plantillas
status: active
summary: Plantillas oficiales para mantener una estructura consistente en toda la base de conocimiento.
tags: [templates, contribution]
---

# Plantillas

Estas plantillas definen la estructura recomendada de cada tipo de página. Deben adaptarse al contenido: una sección sin valor informativo puede omitirse, pero no deben inventarse datos para completar la plantilla.

## Metadatos comunes

```yaml
---
title: Nombre legible
slug: identificador-estable
entity: procedure
status: draft
summary: Descripción breve de la página.
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

### Estados

| Estado | Uso |
|---|---|
| `draft` | Contenido inicial e incompleto |
| `review` | Pendiente de contraste o revisión |
| `verified` | Contrastado con fuentes adecuadas |
| `experimental` | Hipótesis, prueba propia o resultado provisional |
| `active` | Plantilla o documento organizativo vigente |

## Tipos de ficha

### Punto de entrada

- [Procedimiento](procedure.md)
- [Vehículo](vehicle.md)

### Knowledge

- [Concepto](concept.md)
- [Producto químico](chemical.md)
- [Lubricante o grasa](lubricant.md)
- [Material](material.md)
- [Componente](component.md)
- [Montaje y sellado](assembly.md)
- [Producto comercial](commercial-product.md)

## Reglas de uso

1. El procedimiento debe ser útil por sí mismo y enlazar a las explicaciones profundas.
2. Una ficha de producto comercial debe enlazar a su categoría técnica.
3. La compatibilidad incierta se marca con `❓`; no se supone.
4. Los precios siempre incluyen fecha, mercado y formato.
5. Las especificaciones críticas indican su fuente y condiciones.

!!! note
    Los metadatos describen hechos estables y estructurables. Las explicaciones, advertencias y matices pertenecen al cuerpo del documento.
