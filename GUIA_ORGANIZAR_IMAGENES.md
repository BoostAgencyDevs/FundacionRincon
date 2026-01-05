# 📋 Guía para Organizar tus Imágenes del Carrusel

## Opción 1: Renombrar tus imágenes (MÁS FÁCIL)

### Paso 1: Elige 3 imágenes
Selecciona las 3 mejores imágenes de tu carpeta `images/` que quieres mostrar en el carrusel.

### Paso 2: Renómbralas así:
- **Primera imagen** → `imagen1.jpg` (aparecerá primero)
- **Segunda imagen** → `imagen2.jpg` (aparecerá segunda)
- **Tercera imagen** → `imagen3.jpg` (aparecerá tercera)

### Paso 3: Listo
El carrusel las mostrará automáticamente.

---

## Opción 2: Editar el HTML (Si quieres usar nombres personalizados)

### Paso 1: Elige tus 3 imágenes
Decide cuáles quieres usar y anota sus nombres exactos.

### Paso 2: Abre el archivo `index.html`

### Paso 3: Busca estas líneas (alrededor de la línea 38, 47, 56):

```html
<!-- Primera slide -->
<div class="slide-image" style="background-image: url('images/PORTADA.jpg');"></div>

<!-- Segunda slide -->
<div class="slide-image" style="background-image: url('images/480465867_1448438452980321_3138386363642871049_n.jpg');"></div>

<!-- Tercera slide -->
<div class="slide-image" style="background-image: url('images/473023411_1137776934613576_3138229888630982744_n.jpg');"></div>
```

### Paso 4: Cambia los nombres
Reemplaza los nombres dentro de `url('images/AQUI.jpg')` con los nombres de tus imágenes.

**Ejemplo:**
Si quieres usar `LOGO.jpg`, `PORTADA.jpg` y otra imagen, cambia a:
```html
<div class="slide-image" style="background-image: url('images/LOGO.jpg');"></div>
<div class="slide-image" style="background-image: url('images/PORTADA.jpg');"></div>
<div class="slide-image" style="background-image: url('images/472863182_1417583252732508_2774133065196179199_n.jpg');"></div>
```

---

## 📝 Resumen Rápido

### Método Recomendado (Más Fácil):
1. Elige 3 imágenes
2. Renómbralas: `imagen1.jpg`, `imagen2.jpg`, `imagen3.jpg`
3. ¡Listo!

### Método Alternativo:
1. Elige 3 imágenes
2. Abre `index.html`
3. Busca las líneas con `background-image: url('images/...')`
4. Cambia los nombres por los de tus imágenes
5. Guarda el archivo

---

## 💡 Tips

- **Importante**: Los nombres deben coincidir EXACTAMENTE (mayúsculas y minúsculas importan)
- **Formato**: Puedes usar `.jpg`, `.jpeg`, `.png` o `.webp`
- **Orden**: La primera imagen será la que aparezca al cargar la página
- **Cantidad**: Actualmente el carrusel tiene 3 slides. Si quieres más, avísame y te ayudo a agregarlas.

---

## 🎯 Ejemplo Visual

**Estructura de carpetas:**
```
images/
  ├── imagen1.jpg  ← Tu mejor foto (primera)
  ├── imagen2.jpg  ← Tu segunda mejor foto
  ├── imagen3.jpg  ← Tu tercera mejor foto
  └── (otras imágenes que no se usarán en el carrusel)
```

