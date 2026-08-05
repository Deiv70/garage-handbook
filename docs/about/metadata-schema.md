---
title: Esquema de metadatos
summary: Contrato YAML común y campos específicos por tipo de documento.
status: review
tags:
  - project
  - metadata
  - data-model
---

# Esquema de metadatos

El front matter YAML describe datos estables y estructurables. El cuerpo Markdown conserva explicaciones, advertencias, excepciones y razonamiento técnico.

## Campos comunes

```yaml
---
title: Título visible
summary: Resumen breve y autosuficiente.
type: chemical
status: draft
contexts:
  - detailing
  - workshop
aliases: []
tags: []
last_reviewed: null
evidence: []
related: []
---
```

| Campo | Obligatorio | Descripción |
|---|:---:|---|
| `title` | Sí | Nombre visible de la página |
| `summary` | Sí | Resumen corto para índices y búsquedas |
| `type` | Sí | Tipo de entidad definido en el modelo de datos |
| `status` | Sí | `draft`, `review`, `verified` o `experimental` |
| `contexts` | No | Contextos de uso, principalmente `detailing` y `workshop` |
| `aliases` | No | Sinónimos y nombres habituales |
| `tags` | No | Etiquetas de búsqueda; no sustituyen a la estructura |
| `last_reviewed` | No | Fecha ISO `YYYY-MM-DD` de la última revisión técnica |
| `evidence` | No | Tipos de evidencia usados |
| `related` | No | Rutas relativas a documentos directamente relacionados |

## Reglas generales

- Usar listas incluso cuando inicialmente exista un único valor si el campo admite varios elementos.
- Usar `null` cuando el dato no se conozca todavía y omitir el campo cuando no sea aplicable al tipo de entidad.
- No almacenar párrafos ni advertencias largas en YAML.
- No duplicar en metadatos información que solo puede interpretarse con contexto.
- Las rutas de relación deben ser relativas a `docs/` y no incluir el dominio de GitHub Pages.

## Tipos y campos específicos

### `concept`

```yaml
type: concept
scope: cleaning
symbols: []
units: []
```

### `chemical`

```yaml
type: chemical
chemical_family: solvent-cleaner
water_based: false
ph:
  value: null
  range: null
  applicability: not-applicable
aggressiveness: 4
cleaning_targets:
  - oils
compatible_sprayers:
  - ik-hc
material_compatibility: {}
protection_compatibility: {}
```

`aggressiveness` representa riesgo global de uso, no potencia de limpieza. Las compatibilidades usan `compatible`, `conditional`, `incompatible`, `unknown` o `not-applicable`.

### `lubricant`

```yaml
type: lubricant
lubricant_form: grease
base_oil: null
thickener: null
nlgi: null
temperature_c:
  min: null
  max: null
solid_lubricants: []
material_compatibility: {}
```

### `material`

```yaml
type: material
material_family: elastomer
common_names: []
resistance:
  hydrocarbons: unknown
  acids: unknown
  alkalis: unknown
```

### `component`

```yaml
type: component
system: braking
functions: []
common_failures: []
```

### `assembly`

```yaml
type: assembly
assembly_family: threadlocker
curing_mechanism: anaerobic
strength: medium
service_temperature_c:
  min: null
  max: null
```

### `commercial-product`

```yaml
type: commercial-product
brand: null
product_name: null
implements: []
manufacturer_part_number: null
region: eu
```

`implements` enlaza la familia técnica principal, por ejemplo `knowledge/chemicals/cleaners/apc.md`.

### `vehicle`

```yaml
type: vehicle
manufacturer: Seat
model: Leon
generation: 1M
platform: 1J
production_years:
  from: null
  to: null
engine_codes: []
```

### `procedure`

```yaml
type: procedure
contexts:
  - workshop
difficulty: medium
estimated_time_minutes:
  min: null
  max: null
applies_to: []
works_on: []
uses: []
```

### `quick-reference`

```yaml
type: quick-reference
format: cheatsheet
scope: cleaning
summarizes: []
manual_sync_required: true
```

Formatos admitidos inicialmente: `cheatsheet`, `decision-tree`, `compatibility`, `comparison`, `checklist` y `torque-table`.

## Evolución

Añadir un campo solo cuando:

1. tenga un significado inequívoco;
2. vaya a reutilizarse en varias páginas;
3. permita búsqueda, validación, generación o filtrado real;
4. no obligue a inventar valores que todavía no conocemos.
