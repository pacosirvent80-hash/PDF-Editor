# Editor PDF Pro

Editor de PDF 100% client-side (sin servidor). Inspirado en https://www.itnove.com/recursos/editor-pdf y construido desde cero con más features.

## Stack
- **PDF.js** (v3.11.174) — renderizado de páginas
- **pdf-lib** (v1.17.1) — modificación y exportación del PDF
- Sin frameworks, sin build step, HTML/CSS/JS puro

## Estructura
```
editor PDF/
├── src/               ← fuente de desarrollo
│   └── editor-pdf.html
├── dist/              ← versión lista para usar/desplegar
│   └── editor-pdf.html
├── assets/
│   ├── icons/         ← iconos propios si los hubiera
│   └── samples/       ← PDFs de prueba
└── docs/              ← notas, capturas, documentación
```

## Uso rápido
Abrir `dist/editor-pdf.html` directamente con el navegador (doble clic). No necesita servidor.

## Features implementadas
- Añadir / editar texto (fuente, tamaño, color, negrita, cursiva)
- Pluma / dibujo libre con borrador real (destination-out)
- Formas: rectángulo, elipse, línea, flecha
- Resaltado de área con color y opacidad configurables
- Corrector blanco (whiteout)
- Insertar imágenes con redimensionado
- Firma dibujada (modal con soporte táctil)
- Sellos predefinidos (BORRADOR, APROBADO, CONFIDENCIAL…)
- Deshacer / Rehacer (historial completo)
- Zoom (botones + Ctrl+scroll)
- Sidebar de miniaturas con navegación
- Atajos de teclado (V, T, P, E, R, C, L, H, W, I, S)
- Descarga PDF con todos los cambios embebidos

## Atajos de teclado
| Tecla | Herramienta |
|-------|-------------|
| V | Seleccionar/mover |
| T | Texto |
| P | Pluma |
| E | Borrador |
| R | Rectángulo |
| C | Círculo/elipse |
| L | Línea |
| H | Resaltado |
| W | Corrector blanco |
| I | Insertar imagen |
| S | Firma |
| Ctrl+Z | Deshacer |
| Ctrl+Y | Rehacer |
| Ctrl+S | Descargar PDF |
| Ctrl+scroll | Zoom |
| Supr | Borrar elemento seleccionado |

## Mejoras pendientes / roadmap
- [x] Editar texto existente del PDF — doble clic sobre cualquier texto del PDF en modo Seleccionar/Texto
- [ ] Gestión de páginas (reordenar, duplicar, eliminar)
- [ ] Exportar página individual como imagen
- [ ] Campos de formulario (checkbox, input)
- [ ] Fuentes embebidas adicionales (para no-latinos)
- [ ] Modo oscuro / claro para el visor
- [ ] Soporte móvil completo (touch en canvas)
