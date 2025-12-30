# SSAssault - Proyecto Memorias

> Informacion del proyecto para futuras sesiones de trabajo

---

## Arquitectura de Archivos

| Archivo                 | Proposito                                     |
|-------------------------|-----------------------------------------------|
| `ssassault.html`        | Version PRODUCCION (imagenes base64 embebidas) |
| `ssassault_editable.html` | Version DESARROLLO (refs externas a `levels/`) |
| `levels/*.jpg`          | Imagenes de fondo para version desarrollo     |
| `screenshots/`          | Capturas de pantalla para README              |

---

## Historial de Cambios Importantes

### Commit e7a67bb (2025-12-27)
**"docs: add development version and update project structure"**

| Archivo                 | Cambio                                        |
|-------------------------|-----------------------------------------------|
| README.md               | Actualizado con nueva estructura del proyecto |
| ssassault.html          | Modificado (version produccion)               |
| ssassault_editable.html | Agregado (version desarrollo)                 |

**Descripcion:**
- El README ahora documenta las dos versiones del juego
- `ssassault.html` - Produccion (imagenes base64 embebidas, ~1.3MB, sin dependencias)
- `ssassault_editable.html` - Desarrollo (referencias a archivos externos en `levels/`)

---

## Workflow de Desarrollo

```
1. Editar ssassault_editable.html (desarrollo)
2. Probar cambios localmente
3. Cuando este listo para produccion:
   - Convertir imagenes externas a base64
   - Actualizar ssassault.html
4. Commit y push
```

---

## Notas Tecnicas

- **Stack:** HTML5 + CSS3 + Vanilla JavaScript (sin dependencias)
- **Rendering:** Canvas API 2D
- **Persistencia:** LocalStorage (high scores)
- **Niveles:** 5 (Space, Jungle, Islands, Ocean, Inferno)
- **Tamaño produccion:** ~1.3MB (todo embebido)
