# 📚 GUÍA: GitHub + Vercel para PIZZAMICA

## 🎯 Objetivo
Tener tu menú en internet con tu propio link (sin que diga Claude)

---

## PASO 1️⃣: Crear Repositorio en GitHub

### A. Crear cuenta en GitHub (si no tienes)
1. Ve a [github.com](https://github.com)
2. Click en "Sign up"
3. Completa los datos
4. Verifica tu email

### B. Crear nuevo repositorio
1. Ve a [github.com/new](https://github.com/new)
2. Nombre del repo: **menu-pizzamica**
3. Descripción: "Menu digital para Pizzamica Andacollo"
4. Privado o Público (como prefieras)
5. Click "Create repository"

---

## PASO 2️⃣: Subir Archivos a GitHub

Tienes 2 opciones:

### OPCIÓN A: Usando GitHub Desktop (La más fácil)

1. Descarga [GitHub Desktop](https://desktop.github.com)
2. Abre GitHub Desktop e inicia sesión
3. Click "File" → "Clone Repository"
4. Selecciona tu repo "menu-pizzamica"
5. Elige donde guardar la carpeta
6. Abre esa carpeta en tu computadora
7. **Copia aquí TODOS estos archivos:**
   - menu-pizzamica.jsx
   - package.json
   - tailwind.config.js
   - vercel.json
   - .gitignore
   - README.md

8. En GitHub Desktop:
   - Verás los cambios a la izquierda
   - En el campo "Summary", escribe: "Initial commit"
   - Click "Commit to main"
   - Click "Push origin"

¡Listo! Tus archivos están en GitHub.

### OPCIÓN B: Usando Git por Terminal (Si sabes de terminal)

```bash
# Clona el repositorio
git clone https://github.com/TU-USUARIO/menu-pizzamica.git
cd menu-pizzamica

# Copia los archivos aquí

# Sube los cambios
git add .
git commit -m "Initial commit"
git push origin main
```

---

## PASO 3️⃣: Conectar Vercel a GitHub

1. Ve a [vercel.com](https://vercel.com)
2. Click "Sign up"
3. Selecciona "Continue with GitHub"
4. Autoriza Vercel a acceder a GitHub
5. Completa tu perfil

---

## PASO 4️⃣: Desplegar en Vercel

1. En Vercel, click "New Project"
2. Selecciona tu repo "menu-pizzamica"
3. Click "Import"
4. En "Environment Variables" (opcional):
   - Name: `REACT_APP_WHATSAPP_NUMBER`
   - Value: `56950249329`
5. Click "Deploy"

**¡ESPERA 2-3 MINUTOS!**

Vercel desplegará tu proyecto. Verás algo como:

```
✅ Deployment successful!
🌐 Your site is live at: https://menu-pizzamica.vercel.app
```

---

## PASO 5️⃣: Usar tu Propio Dominio (OPCIONAL)

Si compraste un dominio (ej: pizzamica.cl):

1. En Vercel, ve a tu proyecto
2. Click "Settings" → "Domains"
3. Agrega tu dominio personalizado
4. Sigue las instrucciones para apuntar los DNS
5. ¡Listo! Tu link será: `https://pizzamica.cl`

---

## 📱 Ahora Tienes

✅ Tu menú en internet: `https://menu-pizzamica.vercel.app`  
✅ Sin que diga "Claude"  
✅ Link profesional para compartir  
✅ Actualizaciones automáticas con cada push a GitHub  

---

## 🔄 Si Quieres Cambiar Algo

1. Edita el archivo en tu computadora
2. Sube los cambios a GitHub:
   ```bash
   git add .
   git commit -m "Cambio: descripción"
   git push origin main
   ```
3. Vercel se actualiza automáticamente en 2-3 min

---

## ❓ Preguntas Frecuentes

### ¿Puedo cambiar el número de WhatsApp?
Sí, en `menu-pizzamica.jsx` busca:
```javascript
const whatsappNumber = '56950249329';
```
Y cambia el número.

### ¿Cómo cambio los precios?
En `menu-pizzamica.jsx`, busca las constantes al inicio:
```javascript
const pizzaPrice = 10990;
const waffleEntero = 4990;
```

### ¿Vercel es gratis?
Sí, el plan gratuito es perfecto para esto.

### ¿Necesito pagar por el dominio personalizado?
No, es gratis enlazarlo. El dominio mismo (.cl) cuesta $20-50 USD/año en proveedores como Namecheap.

---

¡Tu página estará lista en 15 minutos! 🚀
