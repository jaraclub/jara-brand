---
name: jara-marca
description: Marca del Jara (Jara Club, Asociación Jara Club), club de tiempo libre de Madrid para chicos de 10 a 18 años y sus familias. Úsala siempre que haya que escribir un texto o hacer una pieza del Jara (web, cartel, post, story, presentación, correo, circular, WhatsApp a familias, merch, firma), aunque no se mencione la marca. Da el nombre correcto, la voz, el escudo, los colores, las tipografías y una comprobación final.
---

# Marca del Jara

Fuente completa: https://github.com/jaraclub/jara-brand. Si necesitas más detalle del que hay aquí, lee `JARA-MARCA.md` en https://raw.githubusercontent.com/jaraclub/jara-brand/main/JARA-MARCA.md. No abras `index.html`: pesa 370 KB y no aporta nada para un agente.

## Versión (antes de nada)
Si trabajas en un proyecto (web, app…), busca en su `AGENTS.md` o `CLAUDE.md` la línea `Marca: jara-brand X.Y` y compárala con `version` en https://raw.githubusercontent.com/jaraclub/jara-brand/main/jara-tokens.json. Si no hay línea, la versión del proyecto es 0.

- **Si cambia la versión mayor**, han cambiado logos, colores o tipografías. Antes de hacer el encargo, cuenta qué cambia según https://raw.githubusercontent.com/jaraclub/jara-brand/main/CAMBIOS.md y pregunta si se aplica. No lo apliques sin un sí.
- **Si cambia solo la versión menor**, aplica lo nuevo en lo que toques.
- En los dos casos, actualiza la línea del proyecto. Si no se aplica algo, apúntalo como excepción.
- Las excepciones del proyecto, por ejemplo «sin escudo hasta nueva orden», mandan sobre esta guía.

## Lo esencial
- **El club:** de tiempo libre, para chicos de 10 a 18 años y sus familias. Está en C/ Menéndez Pidal, 35, 28036 Madrid, existe desde 1957 y su web es jaraclub.com. El club es de las familias: lo dirigen padres de socios.
- **Nombre:** «el Jara» en los textos, con artículo y en masculino. «Jara Club» para presentarnos. «Asociación Jara Club» solo en lo legal. Nunca «Asociación Juvenil», «Club Jara» ni «la Jara».
- **Lema (propuesta):** «Aquí se crece.»
- **Voz:** como un padre en la puerta del colegio. Se tutea a todos y se da primero lo práctico (qué, cuándo, dónde, cuánto). Con humor, sin mayúsculas a gritos ni filas de emojis. Sin palabras de dentro: «preceptuación» pasa a «conversaciones con su preceptor», y «convivencia» a «días fuera» o «campamento».

## Visual
- **Colores (solo estos cinco):** rojo #DF171A, blanco #FFFFFF, marino #14213D, amarillo #FFC629, verde #2F4A3A.
- **Proporción:** blanco 50 %, marino 22 %, rojo 18 %, amarillo y verde 5 % cada uno.
- **Cajas destacadas:** rojo al 10 %.
- **Sobre marino:** el rojo solo en titulares y gráficos; el texto pequeño, en blanco o amarillo.
- **Letra:** Big Shoulders Display (800-900, mayúscula) para titulares, Barlow (400/600/700) para texto y Barlow Condensed (700, mayúscula) para etiquetas. Si no están disponibles, Arial Narrow y Arial.

```html
<link rel="stylesheet" href="https://fonts.googleapis.com/css2?family=Barlow:wght@400;600;700&family=Barlow+Condensed:wght@700&family=Big+Shoulders+Display:wght@800;900&display=swap">
```

**Logos** (base: `https://raw.githubusercontent.com/jaraclub/jara-brand/main/logos/`):

| Archivo | Uso |
|---|---|
| `jara-escudo.svg` | Sobre blanco. Es la marca principal |
| `jara-escudo-blanco.svg` | Sobre rojo o marino |
| `jara-escudo-placa.svg` | Sobre foto |
| `jara-flor.svg`, `jara-flor-blanco.svg` | Avatar, favicon, menos de 64 px |
| `jara-palabra.svg`, `jara-palabra-blanco.svg` | Cabeceras estrechas, pies, cierre de vídeo |

El escudo no se parte, no se recorta, no se gira y no lleva sombras. JARA es un dibujo: nunca se reescribe con una tipografía.

**Dos registros:**
- **1.ª equipación (10 a 14 años y familias):** fondo blanco y mucho aire.
- **2.ª equipación (14 a 18 años):** fondo marino, collage, formato vertical y frases cortas.

## Comprobación final
- [ ] Sin «Asociación Juvenil», y «el Jara» bien escrito.
- [ ] Solo los cinco colores, y nada de rojo en texto pequeño sobre marino.
- [ ] Escudo entero y JARA siempre como SVG.
- [ ] Tipografías correctas.
- [ ] Texto tuteado, práctico y sin jerga interna.
- [ ] Fotos de menores con autorización, sin nombre y apellido junto a la cara, y sin bancos de imágenes.
