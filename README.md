# Fundación Rincón

Página web moderna para la Fundación Rincón con diseño responsive y carrusel automático.

## Características

- ✨ **Carrusel automático**: Imágenes que cambian automáticamente cada 5 segundos
- 🎨 **Diseño moderno**: Colores azul oscuro y blanco
- 📱 **Responsive**: Adaptable a todos los dispositivos
- 🚀 **Rendimiento optimizado**: Carga rápida y animaciones suaves
- ♿ **Accesible**: Navegación intuitiva y estructura semántica

## Estructura del Proyecto

```
Fundacion Rincon/
├── index.html      # Estructura HTML principal
├── styles.css      # Estilos y diseño
├── script.js       # Funcionalidad del carrusel y navegación
└── README.md       # Este archivo
```

## Uso

Simplemente abre `index.html` en tu navegador para ver la página web.

## Personalización

### Cambiar imágenes del carrusel

Edita las URLs de las imágenes en `index.html` en las secciones `.slide-image`:

```html
<div class="slide-image" style="background-image: url('TU_IMAGEN_AQUI');"></div>
```

### Modificar colores

Los colores principales están definidos en `styles.css` como variables CSS:

```css
:root {
    --primary-blue: #0a2540;
    --dark-blue: #051a2e;
    --light-blue: #1a4d7a;
    --white: #ffffff;
}
```

### Cambiar velocidad del carrusel

En `script.js`, modifica el valor de `autoPlayDelay`:

```javascript
this.autoPlayDelay = 5000; // Cambiar a milisegundos deseados
```

## Tecnologías Utilizadas

- HTML5
- CSS3 (con variables CSS y animaciones)
- JavaScript (ES6+)
- Sin dependencias externas

## Licencia

© 2024 Fundación Rincón. Todos los derechos reservados.
