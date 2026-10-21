# Portal Minero

Sitio estático (sin servidor). Se publica con GitHub Pages.

- `index.html`: la página.
- `media/`: videos y portadas de la sección «En uso».
- `library/`: material de la Biblioteca técnica. Cada archivo se lista en `library/library.json`.

## Agregar material a la biblioteca

1. Sube el PDF (o imagen) a la carpeta `library/`.
2. Abre `library/library.json` y agrega un bloque como este, separado por coma del anterior:

```json
{
  "title": "Nombre que se ve en la tarjeta",
  "topic": "Tema",
  "file": "library/nombre-del-archivo.pdf",
  "type": "application/pdf",
  "size": 123456,
  "date": "2026-10-21"
}
```

`size` es el peso en bytes (solo informativo). Para una portada, agrega `"cover": "library/portada.jpg"` y `"pages": 7`.
