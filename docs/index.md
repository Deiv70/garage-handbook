---
title: Garage Handbook
status: active
tags:
  - index
---

# Garage Handbook

Base de conocimiento técnica de automoción orientada a **decidir qué hacer, qué producto utilizar y por qué**.

## Cómo usar esta documentación

1. Empieza por un [procedimiento](procedures/index.md) cuando tengas una tarea concreta.
2. Consulta el **core** para entender productos químicos, lubricantes, materiales y fijadores.
3. Entra en [Vehículos](vehicles/index.md) para especificaciones, compatibilidades y particularidades de un modelo.

```mermaid
flowchart LR
    A[Tarea o problema] --> B[Procedimiento]
    B --> C[Conceptos del core]
    B --> D[Datos del vehículo]
    C --> E[Producto o método recomendado]
    D --> E
```

## Principios

- **Una única fuente de verdad:** cada concepto se documenta una sola vez.
- **Procedimientos primero:** resumen la tarea y enlazan a las fichas técnicas relacionadas.
- **Conceptos antes que marcas:** las marcas son ejemplos dentro de su familia técnica.
- **Información estructurada:** las páginas incorporan metadatos para facilitar búsquedas y futuras automatizaciones.
- **Evidencia visible:** se diferencia entre documentación oficial, pruebas, consenso e hipótesis.

!!! warning "Uso responsable"
    Confirma siempre las instrucciones del fabricante, la ficha técnica y la ficha de datos de seguridad antes de aplicar un producto o ejecutar un procedimiento.

## Estado del proyecto

La documentación se encuentra en fase inicial. Las páginas marcadas como `draft` pueden contener apartados incompletos.
