# Instrucciones para agentes

Este repo es la marca del Jara (Asociación Jara Club), un club de tiempo libre de Madrid para chicos de 10 a 18 años y sus familias. Úsalo para escribir textos o hacer piezas del club: webs, carteles, posts, presentaciones, correos o merch.

## Qué leer
1. **[JARA-MARCA.md](JARA-MARCA.md):** la guía completa: nombre, voz, escudo, color, letra y fotografía. Léela entera antes de hacer nada.
2. **[jara-tokens.json](jara-tokens.json):** los colores con RGB, CMYK y Pantone, las tipografías y las medidas del logo, en formato máquina.
3. **[logos/](logos/):** los SVG. Úsalos tal cual.
4. **[CAMBIOS.md](CAMBIOS.md):** qué ha cambiado en cada versión de la marca.

No abras [index.html](index.html) para informarte. Es el manual visual para personas y pesa unos 370 KB, casi todo fuentes en base64. No contiene nada que no esté en JARA-MARCA.md.

No modifiques los archivos de `logos/` ni de `fuentes/`.

## Versiones
Cada proyecto que usa esta marca anota en su `AGENTS.md` o `CLAUDE.md` la versión que tiene aplicada, con una línea así: `Marca: jara-brand 2.0`. Si tiene alguna excepción decidida por el club, va en la misma sección. Por ejemplo: «sin escudo ni palabra hasta nueva orden».

Cada vez que te pidan algo en un proyecto que use esta marca, empieza por aquí:
1. Compara la versión anotada en el proyecto con `version` en [jara-tokens.json](jara-tokens.json). Si el proyecto no tiene anotada ninguna, tómalo como versión 0.
2. Si la versión mayor es distinta, es que han cambiado logos, colores o tipografías. Antes de hacer el encargo, cuéntale a quien te lo pide qué cambia, según [CAMBIOS.md](CAMBIOS.md), y pregúntale si lo aplicas. No lo apliques por tu cuenta.
3. Si dice que sí, aplícalo y sube la versión anotada. Si dice que no, sube igualmente la versión anotada y apunta como excepción lo que no se aplica, para no volver a preguntarlo.
4. Si solo cambia la versión menor, aplica lo nuevo en lo que toques y sube la versión anotada.

Respeta las excepciones de cada proyecto, aunque contradigan esta guía.

## Para código
Fuentes (Google Fonts):

```html
<link rel="preconnect" href="https://fonts.googleapis.com">
<link rel="preconnect" href="https://fonts.gstatic.com" crossorigin>
<link rel="stylesheet" href="https://fonts.googleapis.com/css2?family=Barlow:wght@400;600;700&family=Barlow+Condensed:wght@700&family=Big+Shoulders+Display:wght@800;900&display=swap">
```

Variables CSS:

```css
:root {
  --jara-rojo: #DF171A;
  --jara-blanco: #FFFFFF;
  --jara-marino: #14213D;
  --jara-amarillo: #FFC629;
  --jara-verde: #2F4A3A;
  --jara-rojo-10: color-mix(in srgb, #DF171A 10%, #FFFFFF); /* cajas destacadas */

  --jara-titular: 'Big Shoulders Display', 'Arial Narrow', Arial, sans-serif; /* 800-900, mayúscula */
  --jara-texto: 'Barlow', Arial, sans-serif;                                 /* 400, 600, 700 */
  --jara-etiqueta: 'Barlow Condensed', 'Arial Narrow', Arial, sans-serif;    /* 700, mayúscula, letter-spacing .1em */
}
```

Logos desde otro proyecto (URL directas):

| Pieza | URL |
|---|---|
| Escudo, rojo | https://raw.githubusercontent.com/jaraclub/jara-brand/main/logos/jara-escudo.svg |
| Escudo, blanco | https://raw.githubusercontent.com/jaraclub/jara-brand/main/logos/jara-escudo-blanco.svg |
| Escudo con placa | https://raw.githubusercontent.com/jaraclub/jara-brand/main/logos/jara-escudo-placa.svg |
| La jara, rojo | https://raw.githubusercontent.com/jaraclub/jara-brand/main/logos/jara-flor.svg |
| La jara, blanco | https://raw.githubusercontent.com/jaraclub/jara-brand/main/logos/jara-flor-blanco.svg |
| Palabra, rojo | https://raw.githubusercontent.com/jaraclub/jara-brand/main/logos/jara-palabra.svg |
| Palabra, blanco | https://raw.githubusercontent.com/jaraclub/jara-brand/main/logos/jara-palabra-blanco.svg |

Para una web en producción, descarga el SVG y guárdalo en el proyecto en vez de enlazarlo a raw.githubusercontent.com.

## Qué logo usar
| Fondo | Pieza |
|---|---|
| Blanco | Escudo rojo |
| Rojo o marino | Escudo blanco |
| Foto o color revuelto | Escudo con placa |
| Avatar, favicon, menos de 64 px de alto | La jara, sobre fondo rojo en blanco o sobre blanco en rojo |
| Cabecera estrecha, pie, cierre de vídeo | Palabra |

## Comprobación final
Antes de entregar, revisa:
- [ ] No aparece «Asociación Juvenil». «Asociación Jara Club» solo sale en textos legales.
- [ ] En los textos se dice «el Jara», con artículo y en masculino. Nunca «Club Jara» ni «la Jara».
- [ ] Solo se usan los cinco colores. Nada de naranja, de rojos rosados ni de otros tonos.
- [ ] Sobre marino, el rojo solo va en titulares, franjas o gráficos. El texto pequeño va en blanco o amarillo.
- [ ] El escudo está entero: no se ha partido, recortado, deformado ni girado, y no lleva sombras.
- [ ] JARA no está reescrito con ninguna tipografía: es siempre el SVG.
- [ ] Los titulares van en Big Shoulders Display, en mayúscula. El texto, en Barlow.
- [ ] El texto tutea, da primero lo práctico (qué, cuándo, dónde, cuánto) y no usa palabras de dentro como «preceptuación», «convivencia» o «plática».
- [ ] Si hay fotos de chicos: tienen autorización, no llevan nombre y apellido junto a la cara y no son de banco de imágenes.
