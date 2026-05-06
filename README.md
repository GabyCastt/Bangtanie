# ARMY Galaxy ✦

App hecha para Salo, Marjuri y Víctor 💜🩷🩵

---

## Estructura de carpetas

```
army-galaxy/
├── index.html          ← archivo principal (no tocar)
├── music/
│   ├── mikrokosmos.mp3  ← canción de Salo ✅ ya incluida
│   ├── so_what.mp3      ← canción de Marjuri ✅ ya incluida
│   └── victor.mp3       ← ⬅ AGREGAR cuando Víctor diga su canción
└── img/
    ├── hobi/
    │   ├── 1.jpg        ← ⬅ foto de Hobi para puzzle 1 de Salo
    │   ├── 2.jpg        ← ⬅ foto de Hobi para puzzle 2 de Salo
    │   └── 3.jpg        ← ⬅ foto de Hobi para puzzle 3 de Salo
    ├── jimin/
    │   ├── 1.jpg        ← ⬅ foto de Jimin para puzzle 1 de Marjuri
    │   ├── 2.jpg        ← ⬅ foto de Jimin para puzzle 2 de Marjuri
    │   └── 3.jpg        ← ⬅ foto de Jimin para puzzle 3 de Marjuri
    └── yoongi/
        ├── 1.jpg        ← ⬅ foto de Yoongi para puzzle 1 de Víctor
        ├── 2.jpg        ← ⬅ foto de Yoongi para puzzle 2 de Víctor
        └── 3.jpg        ← ⬅ foto de Yoongi para puzzle 3 de Víctor
```

> Las imágenes pueden ser .jpg o .png — si usas .png solo cambia la extensión
> en index.html (busca `img/hobi/1.jpg` y cambia según corresponda).

---

## Agregar la canción de Víctor (cuando la diga)

**Opción A — archivo mp3 (recomendado):**
1. Pon el archivo en `/music/victor.mp3`
2. Abre `index.html` y busca este comentario:
   ```
   ✂ <audio id="audio-victor" src="music/victor.mp3" ...
   ```
3. Descomenta esa línea (quita los `<!--` y `-->`)
4. Borra el bloque `<div class="upload-area">` que está debajo

**Opción B — dejar que Víctor lo cargue él mismo:**
Ya funciona así. Cuando entre a su sección verá un botón "subir"
para cargar su canción desde el celular. Suena mientras juega.

---

## Subir a GitHub Pages

1. Crea un repositorio en GitHub (puede ser privado o público)
2. Sube toda la carpeta `army-galaxy/` tal cual
3. Ve a **Settings → Pages → Source → main branch → / (root)**
4. GitHub te da un link tipo `https://tuusuario.github.io/army-galaxy/`
5. Compártelo con tus amigos 🚀

---

## Editar los mensajes de felicitación

Abre `index.html` y busca la sección `MENSAJES DE FELICITACIÓN`.
Cada persona tiene 3 mensajes (uno por puzzle completado):

```js
const MESSAGES = {
  salo: [
    { emoji: '💜', heading: '...', text: '...' },  // al terminar nivel 1
    { emoji: '☀️', heading: '...', text: '...' },  // al terminar nivel 2
    { emoji: '🌟', heading: '...', text: '...' }   // al terminar nivel 3
  ],
  ...
}
```

---

Hecho con 💜 para el squad ARMY
