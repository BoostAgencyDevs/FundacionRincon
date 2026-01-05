# 📸 Cómo Agregar Fotos al Carrusel

## Método 1: Forma Simple (Recomendado)

### Paso 1: Coloca tus imágenes
1. Abre la carpeta `images/` en tu proyecto
2. Copia y pega tus fotos ahí

### Paso 2: Nombra las imágenes
Renombra tus fotos con estos nombres exactos:
- `imagen1.jpg` → Primera slide (la que aparece primero)
- `imagen2.jpg` → Segunda slide
- `imagen3.jpg` → Tercera slide

### Paso 3: Formatos soportados
- ✅ `.jpg` o `.jpeg`
- ✅ `.png`
- ✅ `.webp`

### Paso 4: Tamaño recomendado
- **Ancho**: 1920px o más
- **Alto**: 1080px o más
- **Formato**: Horizontal (landscape)

---

## Método 2: Usar tus propios nombres

Si tus imágenes tienen otros nombres (ej: `foto-fundacion.jpg`), necesitas editar el archivo `index.html`:

### Encuentra estas líneas en `index.html`:

```html
<!-- Primera slide (línea ~38) -->
<div class="slide-image" style="background-image: url('images/imagen1.jpg');"></div>

<!-- Segunda slide (línea ~47) -->
<div class="slide-image" style="background-image: url('images/imagen2.jpg');"></div>

<!-- Tercera slide (línea ~56) -->
<div class="slide-image" style="background-image: url('images/imagen3.jpg');"></div>
```

### Cambia los nombres:
Reemplaza `imagen1.jpg`, `imagen2.jpg`, `imagen3.jpg` con los nombres de tus archivos.

**Ejemplo:**
```html
<div class="slide-image" style="background-image: url('images/foto-fundacion.jpg');"></div>
<div class="slide-image" style="background-image: url('images/comunidad.jpg');"></div>
<div class="slide-image" style="background-image: url('images/evento-2024.jpg');"></div>
```

---

## Método 3: Agregar más slides (más de 3 imágenes)

Si quieres agregar una 4ta, 5ta imagen, etc., necesitas:

1. **Agregar el slide en el HTML** (después de la línea 63):
```html
<div class="slide">
    <div class="slide-image" style="background-image: url('images/imagen4.jpg');"></div>
    <div class="slide-overlay"></div>
    <div class="slide-content">
        <h2>Tu Título Aquí</h2>
        <p>Tu descripción aquí</p>
        <a href="#contacto" class="btn-primary">Tu botón</a>
    </div>
</div>
```

2. **Agregar el indicador** (después de la línea 69):
```html
<span class="indicator" data-slide="3"></span>
```

3. **Actualizar el JavaScript** - El código detectará automáticamente las nuevas slides.

---

## Ejemplo Visual de la Estructura

```
Fundacion Rincon/
├── images/
│   ├── imagen1.jpg  ← Primera foto del carrusel
│   ├── imagen2.jpg  ← Segunda foto del carrusel
│   └── imagen3.jpg  ← Tercera foto del carrusel
├── index.html
├── styles.css
└── script.js
```

---

## 💡 Tips

- **Mejor calidad**: Usa imágenes de alta resolución (1920x1080 o más)
- **Peso del archivo**: Comprime las imágenes si son muy pesadas (usa herramientas como TinyPNG)
- **Consistencia**: Trata de que todas las imágenes tengan el mismo tamaño y orientación
- **Formato horizontal**: Las imágenes horizontales se ven mejor en el carrusel

---

## ❓ Problemas Comunes

### Las imágenes no aparecen
- ✅ Verifica que los nombres coincidan exactamente (mayúsculas/minúsculas importan)
- ✅ Verifica que las imágenes estén en la carpeta `images/`
- ✅ Verifica que la ruta en el HTML sea correcta: `images/tu-imagen.jpg`

### Las imágenes se ven cortadas
- ✅ Usa imágenes con relación de aspecto 16:9 (horizontal)
- ✅ Asegúrate de que las imágenes tengan al menos 1920px de ancho

### Quiero cambiar el texto sobre las imágenes
- Edita el contenido dentro de `<div class="slide-content">` en cada slide

