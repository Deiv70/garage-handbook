# Garage Handbook

Manual técnico y base de conocimiento de automoción orientado a procedimientos, mantenimiento, reparación, productos químicos, lubricación, compatibilidad de materiales y montaje.

[![Documentation](https://img.shields.io/badge/docs-GitHub%20Pages-blue)](https://deiv70.github.io/garage-handbook/)

> [!WARNING]
> Esta documentación es una referencia práctica. Antes de aplicar un producto o realizar una intervención, confirma siempre la documentación técnica, la ficha de datos de seguridad y las instrucciones del fabricante del vehículo o componente.

## Índice

1. [Procedimientos](docs/procedures/index.md)
2. [Vehículos](docs/vehicles/index.md)
3. [Knowledge](docs/knowledge/index.md)
   - [Conceptos](docs/knowledge/concepts/index.md)
   - [Productos químicos](docs/knowledge/chemicals/index.md)
   - [Lubricantes y grasas](docs/knowledge/lubricants/index.md)
   - [Materiales](docs/knowledge/materials/index.md)
   - [Componentes](docs/knowledge/components/index.md)
   - [Montaje y sellado](docs/knowledge/assembly/index.md)
   - [Productos comerciales](docs/knowledge/commercial-products/index.md)
4. [Acerca del proyecto](docs/about/index.md)
5. [Plantillas](docs/templates/index.md)

## Principios de organización

- Los **procedimientos** son la principal puerta de entrada y resumen qué hace falta, cómo hacerlo y qué precauciones tomar.
- **Knowledge** contiene la explicación reutilizable de conceptos, productos químicos, lubricantes, materiales, componentes y soluciones de montaje.
- **Vehicles** contiene únicamente información específica de grupos, plataformas, modelos, motorizaciones y configuraciones concretas.
- Los **productos comerciales** se documentan como ejemplos o implementaciones de una categoría técnica, no como sustitutos del concepto.
- La información se enlaza en lugar de duplicarse.

## Estructura

```text
docs/
├── procedures/
├── vehicles/
│   ├── VAG/
│   └── PSA/
├── knowledge/
│   ├── concepts/
│   ├── chemicals/
│   ├── lubricants/
│   ├── materials/
│   ├── components/
│   ├── assembly/
│   └── commercial-products/
├── about/
└── templates/
```

## Desarrollo y publicación

- `develop`: documentación en desarrollo.
- `main`: versión publicada.
- GitHub Actions compila MkDocs y publica GitHub Pages al actualizar `main`.

Sitio publicado: <https://deiv70.github.io/garage-handbook/>

## Leyenda de compatibilidad

| Símbolo | Significado |
|---|---|
| ✅ | Compatible en uso normal siguiendo las instrucciones |
| ⚠️ | Compatible con condiciones, prueba previa o exposición limitada |
| ❌ | Evitar |
| ❓ | Depende de la formulación; consultar al fabricante |

## Escala de agresividad

| Nivel | Interpretación |
|---:|---|
| 1/5 | Muy suave; mantenimiento habitual |
| 2/5 | Suave, pero puede degradar protecciones con uso repetido |
| 3/5 | Limpieza intensa; controlar dilución y tiempo de contacto |
| 4/5 | Agresivo; uso localizado y prueba previa |
| 5/5 | Muy agresivo o industrial; requiere compatibilidad confirmada y EPI adecuados |
