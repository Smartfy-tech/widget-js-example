# Smartfy Product Widget 

Este es un ejemplo funcional de cómo integrar el widget de productos de Smartfy en cualquier sitio web.


## 🚀 Ejecutar el ejemplo

### 1. Abrir el archivo localmente

No se requiere compilación. Simplemente abre el archivo `index.html` en tu navegador o sírvelo con un servidor local para evitar problemas de CORS.

### 2. Configura el `clientSecret`

Abre `index.html` y reemplaza `"CLIENT_SECRET"` con tu valor real proporcionado por Smartfy:

```js
widget.mount({
  clientSecret: "TU_CLIENT_SECRET_AQUI",
  limit: 8,
  selector: '#app',
  onLoaded: () => console.log("Widget cargado"),
  onError: (err) => console.error("Error:", err)
});
```

---

## ✅ Prerrequisitos

Antes de comenzar, asegúrate de tener:

- Tu `clientSecret` de Smartfy.
- Un entorno local o web para servir el HTML.

---

## 🧩 Incluir el widget

En `index.html`, ya está incluido el script necesario:

```html
<script src="https://static.smartfy.tech/widget/product.js"></script>
```

Y el contenedor para montarlo:

```html
<div id="app"></div>
```

---

## 🌐 Producción

Para usar este widget en producción:

- Asegúrate de usar tu `clientSecret` real.
- Puedes incluir el widget directamente desde: `https://static.smartfy.tech/widget/product.js`
- Asegúrate de que tu dominio tenga acceso a los recursos necesarios (fuentes, estilos, etc.).

---
