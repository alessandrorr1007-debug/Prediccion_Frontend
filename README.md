# AulaPredict - Frontend (Interfaz Web)

Interfaz institucional y sobria para detección automática de rostro y predicción emocional para acompañamiento tutorial.

---

## 🚀 Despliegue en Render (Static Site)

Para desplegar este frontend en [Render](https://dashboard.render.com):

1. Haz clic en **New +** ➔ **Static Site**.
2. Conecta este repositorio: `https://github.com/alessandrorr1007-debug/Prediccion_Frontend`.
3. Configuración del sitio:
   - **Name:** `prediccion-frontend` (o el nombre que elijas)
   - **Branch:** `main`
   - **Build Command:** *(dejar vacío)*
   - **Publish Directory:** `.` *(un solo punto para la raíz)*
4. Haz clic en **Create Static Site**.

---

## 🔗 Conexión con el Backend en Render

Por defecto en local se conecta a `http://localhost:8000`.

En producción, la aplicación busca automáticamente tu backend en Render. Si tu backend tiene una URL personalizada, puedes indicarla en la línea 22 de `app.js`:

```javascript
BACKEND_URL: (window.location.hostname === 'localhost' || window.location.hostname === '127.0.0.1')
  ? 'http://localhost:8000'
  : 'https://tu-backend.onrender.com'
```
