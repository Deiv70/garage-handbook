---
title: Plantillas
status: active
summary: Plantillas oficiales para mantener una estructura consistente en toda la base de conocimiento.
tags: [templates, contribution]
---

# Plantillas

Estas plantillas definen la estructura recomendada de cada tipo de página. Deben adaptarse al contenido: una sección sin valor informativo puede omitirse, pero no deben inventarse datos para completar la plantilla.

El contrato completo se documenta en [Esquema de metadatos](../about/metadata-schema.md).

## Metadatos comunes

```yaml
---
title: Nombre legible
summary: Descripción breve de la página.
type: procedure
status: draft
contexts: []
aliases: []
last_reviewed: null
evidence: []
related: []
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

### Acceso y aplicación

- [Quick Reference](quick-reference.md)
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

1. Quick Reference resume otras fichas y nunca sustituye a sus fuentes.
2. El procedimiento debe ser útil por sí mismo y enlazar a las explicaciones profundas.
3. Una ficha de producto comercial debe enlazar a su categoría técnica.
4. La compatibilidad incierta se marca como `unknown`; no se supone.
5. Los precios siempre incluyen fecha, mercado y formato.
6. Las especificaciones críticas indican su fuente y condiciones.

!!! note
    Los metadatos describen hechos estables y estructurables. Las explicaciones, advertencias y matices pertenecen al cuerpo del documento.
