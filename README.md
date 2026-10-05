# ecos-parches

Parches hot-update (`.pck`) para el juego **Ecos**.

La APK consulta `version.json` al arrancar y, si hay una versión mayor, descarga el `.pck` correspondiente.

## version.json

```json
{
  "version": 0,
  "url": "https://github.com/nesty21/ecos-parches/releases/download/vN/ecos_parche.pck",
  "notas": "..."
}
```

- `version`: entero; la APK base arranca en `0`.
- `url`: enlace directo al asset del release (sigue redirecciones HTTPS).
- Los releases se etiquetan `v1`, `v2`, …

Para publicar un parche desde el proyecto: `tools/publicar_parche.sh`.
