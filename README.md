# Marca Jara

Manual de identidad del Jara (Asociación Jara Club), el club de tiempo libre de Menéndez Pidal, en Madrid, para chicos de 10 a 18 años y sus familias.

- [index.html](index.html): el manual completo. Ábrelo en el navegador. Funciona sin conexión porque las fuentes van incluidas.
- [JARA-MARCA.md](JARA-MARCA.md): resumen del manual para quien escriba o diseñe piezas, y para agentes de IA.
- [jara-tokens.json](jara-tokens.json): colores, tipografías y medidas del logotipo.
- [logos/](logos/): escudo, jara y palabra en SVG, en rojo y en blanco.
- [fuentes/](fuentes/): las imágenes originales de las que salen los logotipos y la flor antigua, como archivo.
- [AGENTS.md](AGENTS.md): instrucciones para agentes de IA. Qué leer, variables CSS, URL de los logos y una comprobación final.
- [skills/jara-marca/](skills/jara-marca/): skill para Claude. Cópiala en `~/.claude/skills/` y se activará sola cada vez que pidas algo del Jara, aunque estés en otro proyecto.

## Para usarlo con un agente
Basta con darle la URL del repo: lo primero que leerá es `AGENTS.md`. Si usas Claude Code, instala la skill una vez:

macOS o Linux:

```sh
git clone https://github.com/pfaraluce/jara-brand
mkdir -p ~/.claude/skills
cp -r jara-brand/skills/jara-marca ~/.claude/skills/
```

Windows (PowerShell):

```powershell
git clone https://github.com/pfaraluce/jara-brand
New-Item -ItemType Directory -Force "$HOME\.claude\skills" | Out-Null
Copy-Item -Recurse -Force jara-brand\skills\jara-marca "$HOME\.claude\skills\"
```

Para actualizarla más adelante, haz `git pull` en el repo y repite la copia.

Versión 2.0 · octubre de 2026.
