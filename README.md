# FNF Psych Playground

Un playground web para inspeccionar personajes y stages de mods de Friday Night Funkin' con formato Psych Engine.

## Abrir

GitHub Pages publica automáticamente la versión web al actualizar `main`:

https://10574084-cmd.github.io/FnfPlayGroundMods/

## Cómo usarlo

1. Abre el sitio en Chrome.
2. Importa un mod con **Elegir ZIP** o **Elegir carpeta**.
3. Selecciona el personaje que quieras previsualizar.
4. Importa el audio de chromatic por separado desde el panel de audio si tu mod no lo incluye como archivo compatible.
5. Activa **2 Players** para usar ambos personajes en la vista previa.

## Controles predeterminados

- Player 1: flechas del teclado.
- Player 2: A / S / W / D.
- Q / E: cambiar el personaje seleccionado de Player 1.
- Los controles se pueden reasignar desde las opciones.

## Compatibilidad

El playground interpreta datos de personajes Psych, atlas Sparrow/TexturePacker y algunos atlas de Adobe Animate. La vista de stages y los scripts Lua/HScript tienen compatibilidad parcial; no es un reemplazo del motor completo de Psych Engine.

## GitHub Actions

El workflow `.github/workflows/deploy.yml` reconstruye `dist/index.html`, valida el JavaScript y publica GitHub Pages en cada push a `main`.

Para mantener pequeño el contenido del repositorio, el HTML de publicación se guarda comprimido y dividido en `.site-source/`; Actions lo recompone antes de publicar. Los mods y audios se importan en el navegador y no se suben al repositorio.
