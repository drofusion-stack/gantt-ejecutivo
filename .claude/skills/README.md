# Skills del proyecto

Skills copiados de [nextlevelbuilder/ui-ux-pro-max-skill](https://github.com/nextlevelbuilder/ui-ux-pro-max-skill)
(v2.13.0, commit `09170eec67eefd46a7ae85de61b40c194020f997`), licencia MIT (ver `LICENSE-ui-ux-pro-max`).

- `ui-ux-pro-max` — base de estilos, paletas, tipografías, gráficos y guías UX (búsqueda local, sin red)
- `design-system`, `ui-styling`, `brand`, `design`, `banner-design`, `slides`

## Cambio respecto al original

En `ui-ux-pro-max/SKILL.md` la ruta `${CLAUDE_PLUGIN_ROOT}/.claude/skills/...` se cambió a
`${CLAUDE_PLUGIN_ROOT:-$(git rev-parse --show-toplevel)}/.claude/skills/...`, porque
`CLAUDE_PLUGIN_ROOT` solo existe cuando se instala como plugin. El resto de archivos es idéntico al original.

## Notas

- Los generadores de imágenes de `design` (`logo/generate.py`, `icon/generate.py`, `cip/generate.py`)
  llaman a APIs externas (Gemini, Atlas Cloud, MuAPI) y solo funcionan con `GEMINI_API_KEY` u otra clave configurada.
- 4 módulos de prueba de `ui-ux-pro-max/scripts/tests` dependen de scripts de mantenimiento del repo original
  y no se pueden ejecutar aquí; el resto (137 pruebas) pasa.
