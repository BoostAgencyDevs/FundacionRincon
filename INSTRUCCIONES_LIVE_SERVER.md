# Cómo ver la página en Live Server

## Opción 1: Usando la extensión Live Server en VS Code (Recomendado)

### Paso 1: Instalar la extensión
1. Abre VS Code
2. Ve a la pestaña de **Extensiones** (Ctrl+Shift+X)
3. Busca **"Live Server"** de Ritwick Dey
4. Haz clic en **Instalar**

### Paso 2: Usar Live Server
1. Abre el archivo `index.html` en VS Code
2. Haz **clic derecho** en el archivo `index.html`
3. Selecciona **"Open with Live Server"**
   - O presiona **Alt+L, Alt+O** (atajo de teclado)
   - O haz clic en el botón **"Go Live"** en la barra inferior de VS Code

### Paso 3: Ver tu página
- Se abrirá automáticamente en tu navegador (generalmente en `http://127.0.0.1:5500`)
- La página se recargará automáticamente cuando guardes cambios en los archivos

## Opción 2: Usando Python (si tienes Python instalado)

### En la terminal:
```powershell
# Navega a la carpeta del proyecto
cd "E:\Fundacion Rincon"

# Python 3
python -m http.server 8000

# O Python 2
python -m SimpleHTTPServer 8000
```

Luego abre en tu navegador: `http://localhost:8000`

## Opción 3: Usando Node.js (si tienes Node.js instalado)

### Instalar http-server globalmente:
```powershell
npm install -g http-server
```

### Ejecutar:
```powershell
cd "E:\Fundacion Rincon"
http-server
```

Luego abre en tu navegador la URL que te muestre (generalmente `http://localhost:8080`)

## Opción 4: Abrir directamente en el navegador

Simplemente haz doble clic en `index.html` para abrirlo en tu navegador predeterminado.

**Nota**: Este método no recarga automáticamente cuando haces cambios, tendrás que refrescar manualmente (F5).

---

## Recomendación
La **Opción 1 (Live Server)** es la más fácil y práctica para desarrollo, ya que:
- ✅ Recarga automáticamente al guardar cambios
- ✅ Funciona con hot-reload
- ✅ Muy fácil de usar
- ✅ No requiere configuración adicional

