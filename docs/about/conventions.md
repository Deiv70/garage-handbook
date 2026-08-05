---
title: Convenciones
summary: Reglas de nombres, metadatos, estados y estilo de Garage Handbook.
status: verified
tags:
  - project
  - conventions
---

# Convenciones

## Idioma

- Carpetas, archivos y claves de metadatos: **inglés**.
- Contenido visible: **español**.
- Acrónimos técnicos reconocidos, como VAG, PSA, EPDM o APC, conservan su forma habitual.

## Nombres de archivos

Usar minúsculas y guiones:

```text
brake-cleaners.md
iron-removers.md
threadlockers.md
```

Evitar espacios, CamelCase y guiones bajos en archivos de contenido general.

Los directorios de vehículos son la excepción y usan nombres descriptivos:

```text
Seat-Leon_1M
VW-Golf_IV
Peugeot-307_T5
```

## Front matter mínimo

```yaml
---
title: Título visible
summary: Resumen breve de la página.
status: draft
tags:
  - example
---
```

## Estados

| Estado | Significado |
|---|---|
| `verified` | Revisado y respaldado por documentación técnica suficiente |
| `review` | Utilizable, pero pendiente de una revisión adicional |
| `draft` | Contenido inicial incompleto |
| `experimental` | Hipótesis, prueba propia o conclusión provisional |

## Evidencia

Cuando sea relevante, indicar el origen de la información:

| Tipo | Uso |
|---|---|
| Documentación oficial | Manuales, TDS, SDS, ELSA, documentación del fabricante |
| Norma técnica | ISO, DIN, SAE u otra norma aplicable |
| Prueba propia | Observación o ensayo documentado |
| Consenso profesional | Práctica ampliamente aceptada sin una fuente única |
| Hipótesis | Inferencia pendiente de verificar |

## Commits

Usar Conventional Commits cuando sea posible:

```text
docs(chemicals): add brake cleaner overview
docs(vag): add Seat Leon 1M brake variants
refactor(structure): replace core with knowledge
build(mkdocs): update navigation
```

## Redacción

- Priorizar instrucciones concretas y advertencias claras.
- Separar hechos, recomendaciones e hipótesis.
- No presentar compatibilidad como absoluta cuando depende de concentración, temperatura o tiempo de contacto.
- Enlazar al concepto principal en vez de repetir explicaciones extensas.
