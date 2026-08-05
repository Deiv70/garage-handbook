---
title: Filosofía del proyecto
summary: Principios que definen Garage Handbook como base de conocimiento técnico.
status: verified
tags:
  - project
  - architecture
---

# Filosofía del proyecto

Garage Handbook es una base de conocimiento técnico sobre automoción orientada a resolver trabajos reales de mantenimiento, reparación, diagnóstico, limpieza, montaje y mejora.

No pretende sustituir la documentación oficial del fabricante, los manuales de taller, las fichas técnicas ni las fichas de datos de seguridad. Su función es organizar conocimiento reutilizable y práctico, relacionarlo con vehículos concretos y presentarlo mediante procedimientos fáciles de consultar.

## Principios

### El usuario entra por los procedimientos

La mayoría de lectores buscarán cómo realizar un trabajo concreto. Por ello, **Procedimientos** es la principal puerta de entrada de la web.

Cada procedimiento debe incluir un resumen operativo suficiente para ejecutar el trabajo y enlazar a las fichas técnicas correspondientes cuando el lector quiera profundizar.

### Una única fuente de verdad

Cada concepto debe explicarse en un único lugar. Los procedimientos y las páginas de vehículos enlazan a esa explicación en lugar de duplicarla.

### Conceptos antes que marcas

La documentación define primero la familia técnica —por ejemplo, APC, limpiafrenos o grasa de silicona— y después incorpora productos comerciales que cumplen esa función.

### Conocimiento general y aplicación específica

- **Knowledge** contiene conceptos reutilizables.
- **Vehicles** contiene particularidades de fabricantes, plataformas y modelos.
- **Procedures** combina ambos para realizar trabajos concretos.

### Información basada en evidencia

Las afirmaciones importantes deben distinguir entre documentación oficial, normas, pruebas propias, consenso profesional e hipótesis pendientes de verificar.

### Arquitectura preparada para crecer

Añadir un vehículo, producto o procedimiento nuevo no debe obligar a reorganizar el proyecto ni a duplicar información existente.

## Regla de oro

> El usuario entra por **Procedures**; el conocimiento vive en **Knowledge**.
