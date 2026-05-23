# 💰 Guía Paso a Paso: Subir a GitHub y Activar Google AdSense

> Esta guía te llevará desde tener el proyecto en tu PC hasta cobrar con AdSense.

---

## 📦 PARTE 1: Subir el proyecto a GitHub

### Paso 1: Crear cuenta de GitHub

1. Ve a **[github.com](https://github.com)** y crea una cuenta gratis.
2. Verifica tu email.

### Paso 2: Crear el repositorio

1. Pulsa el botón verde **"New"** o el `+` arriba a la derecha → **"New repository"**.
2. Rellena:
   - **Repository name:** `financeworld-pro`
   - **Description:** "Portal financiero global"
   - **Visibility:** Public (necesario para GitHub Pages gratis)
   - **NO marques** "Add a README" (ya lo tienes)
3. Pulsa **"Create repository"**.

### Paso 3: Subir los archivos

**Opción A — Desde la web (más fácil):**

1. En tu repositorio nuevo verás `uploading an existing file`. Pulsa ahí.
2. Arrastra **TODOS los archivos** de la carpeta `financeworld-pro/`:
   - `index.html`
   - `privacidad.html`
   - `terminos.html`
   - `sobre-nosotros.html`
   - `contacto.html`
   - `404.html`
   - `ads.txt`
   - `robots.txt`
   - `sitemap.xml`
   - `README.md`
   - `GUIA_ADSENSE.md`
3. Abajo escribe `Initial commit` y pulsa **"Commit changes"**.

**Opción B — Con Git desde terminal:**

```bash
cd C:\Users\34642\financeworld-pro
git init
git add .
git commit -m "Initial commit"
git branch -M main
git remote add origin https://github.com/TU-USUARIO/financeworld-pro.git
git push -u origin main
```

### Paso 4: Activar GitHub Pages

1. En tu repositorio ve a **Settings** (icono de engranaje arriba).
2. En el menú lateral izquierdo pulsa **"Pages"**.
3. En **Source** selecciona:
   - Branch: `main`
   - Folder: `/ (root)`
4. Pulsa **"Save"**.
5. Espera 1-3 minutos.
6. Verás un mensaje verde con tu URL: `https://TU-USUARIO.github.io/financeworld-pro/`

🎉 **¡Tu web ya está en internet!**

---

## 🔧 PARTE 2: Personalizar antes de pedir AdSense

### Paso 5: Reemplazar "TU-USUARIO" en todos los archivos

Busca y reemplaza `TU-USUARIO` por tu usuario real de GitHub en:

- `index.html`
- `robots.txt`
- `sitemap.xml`
- `README.md`

**Cómo hacerlo en GitHub:**
1. Abre cada archivo en GitHub
2. Pulsa el icono del lápiz ✏️ (Edit)
3. Pulsa `Ctrl+H` (Find & Replace) o usa el buscador
4. Sustituye `TU-USUARIO` por tu usuario
5. Pulsa "Commit changes"

### Paso 6: Configurar tu dominio personalizado (OPCIONAL pero recomendado para AdSense)

> 💡 **AdSense aprueba más fácil sitios con dominio propio.** Un `.com` cuesta unos 10€/año.

1. Compra un dominio en **Namecheap**, **GoDaddy** o **Google Domains**.
2. En tu repositorio, crea un archivo llamado `CNAME` (sin extensión) con tu dominio dentro:
   ```
   tudominio.com
   ```
3. En el panel de tu proveedor de dominio, añade estos registros DNS:
   ```
   A    @    185.199.108.153
   A    @    185.199.109.153
   A    @    185.199.110.153
   A    @    185.199.111.153
   CNAME www TU-USUARIO.github.io
   ```
4. En GitHub: Settings → Pages → Custom domain → introduce tu dominio.

---

## 💰 PARTE 3: Solicitar Google AdSense

### Paso 7: Esperar antes de solicitar

⚠️ **MUY IMPORTANTE:** Espera al menos **2-4 semanas** después de publicar la web. AdSense rechaza webs muy nuevas.

Durante este tiempo:
- ✅ Comparte tu web en redes sociales
- ✅ Pide a amigos que la visiten
- ✅ Intenta tener algo de tráfico orgánico
- ✅ Asegúrate que todos los enlaces funcionan

### Paso 8: Crear cuenta en AdSense

1. Ve a **[adsense.google.com](https://adsense.google.com)**.
2. Pulsa **"Empezar"** y entra con tu cuenta de Google.
3. Introduce:
   - **URL de tu sitio web:** `https://TU-USUARIO.github.io/financeworld-pro/` (o tu dominio)
   - **País:** España
   - **Acepta** los términos.
4. Configura cómo quieres cobrar (cuenta bancaria, IBAN, etc.).

### Paso 9: Verificar la propiedad del sitio

AdSense te dará un **código de verificación** que parece esto:
```html
<meta name="google-adsense-account" content="ca-pub-1234567890123456">
```

1. **Copia tu Publisher ID** (el `ca-pub-XXXXXXXXXXXXXXXX`).
2. En GitHub, abre `index.html` y reemplaza **TODAS las apariciones** de `ca-pub-XXXXXXXXXXXXXXXX` por tu ID real.

   📍 Hay que reemplazarlo en:
   - El script `<script async src="https://pagead2.googlesyndication.com/...">`
   - El `<meta name="google-adsense-account">`
   - Los 4 bloques de anuncios `data-ad-client`

3. Abre `ads.txt` y reemplaza `pub-XXXXXXXXXXXXXXXX` por tu ID (sin el "ca-").

4. Commit los cambios y espera unos minutos para que se publique.

### Paso 10: Esperar la revisión

⏰ La revisión de AdSense tarda entre **1 día y 4 semanas**. Te llegará un email con la respuesta:
- ✅ **Aprobado:** Ya puedes empezar a ver anuncios.
- ❌ **Rechazado:** Te dirán el motivo. Soluciónalo y vuelve a solicitar.

### Razones comunes de rechazo y soluciones:

| Razón | Solución |
|-------|----------|
| Contenido insuficiente | Añade más artículos al sitio |
| Sitio muy nuevo | Espera 2-4 semanas más |
| Falta política privacidad | ✅ Ya la tienes incluida |
| Falta página About | ✅ Ya la tienes |
| Falta contacto | ✅ Ya la tienes |
| Navegación difícil | ✅ Ya tienes menú |
| Contenido duplicado | Asegúrate que es original |

---

## 🎯 PARTE 4: Una vez aprobado

### Paso 11: Crear las unidades de anuncios

1. En AdSense ve a **"Anuncios" → "Por unidad de anuncio"**.
2. Crea 4 unidades de anuncio:
   - Banner superior (display, responsive)
   - Entre secciones (display, responsive)
   - Después de noticias (display, responsive)
   - Sidebar (display, rectangle)
3. Cada una te dará un `data-ad-slot="XXXXXXXXXX"` (un número).
4. En `index.html` reemplaza los slots:
   - `data-ad-slot="1234567890"` → Banner superior
   - `data-ad-slot="2345678901"` → Entre secciones
   - `data-ad-slot="3456789012"` → Después de noticias
   - `data-ad-slot="4567890123"` → Sidebar

### Paso 12: Optimización

- **Más contenido = más dinero.** Añade nuevos artículos regularmente.
- **SEO:** Registra tu sitio en [Google Search Console](https://search.google.com/search-console).
- **Sitemap:** Envía `https://TU-USUARIO.github.io/financeworld-pro/sitemap.xml` a Search Console.
- **Mide:** Usa [Google Analytics](https://analytics.google.com) para ver visitantes.

---

## 💸 ¿Cuándo cobro?

- Necesitas acumular **70€ (umbral en España)** en tu cuenta de AdSense.
- Una vez alcanzado, Google te paga del 21 al 26 de cada mes.
- Te ingresan por transferencia bancaria (SEPA en España).

---

## 📊 Estimación realista de ingresos

| Visitas/mes | Ingresos aproximados |
|-------------|---------------------|
| 1.000 | 1-5 € |
| 10.000 | 15-50 € |
| 50.000 | 75-250 € |
| 100.000 | 150-500 € |
| 500.000 | 750-2.500 € |

> Los ingresos dependen del nicho (financiero suele pagar bien), país de visitantes y CTR.

---

## ❓ Preguntas frecuentes

### ¿Necesito ser empresa o autónomo?
No para empezar. Si superas 1.000€/año en España debes declarar ingresos.

### ¿Puedo usar AdSense con GitHub Pages?
Sí, perfectamente. Muchas webs aprobadas usan GitHub Pages.

### ¿Puedo tener AdSense en localhost?
No. Tu web debe estar publicada con dominio público.

### ¿Cuántos anuncios puedo poner por página?
Sin límite oficial, pero **calidad > cantidad**. 3-4 anuncios bien colocados rinden más que 10 mal puestos.

### ¿Pierdo dinero si rechazan?
No. Es gratis volver a intentarlo cuando soluciones los problemas.

---

## 📞 ¿Necesitas ayuda?

- 📚 [Centro de ayuda AdSense](https://support.google.com/adsense)
- 💬 [Comunidad AdSense](https://support.google.com/adsense/community)
- 📖 [GitHub Pages docs](https://docs.github.com/en/pages)

---

## ✅ Checklist final antes de pedir AdSense

- [ ] Sitio publicado y funcionando en internet
- [ ] Todas las páginas accesibles (Inicio, About, Contacto, Privacidad, Términos)
- [ ] Banner de cookies funcionando
- [ ] Disclaimer financiero visible
- [ ] `ads.txt` con tu publisher ID
- [ ] `robots.txt` y `sitemap.xml` con tu URL correcta
- [ ] Web tiene al menos 2 semanas de antigüedad
- [ ] Has compartido la web y tiene algunas visitas
- [ ] El contenido es original (no copiado)
- [ ] Todos los enlaces funcionan

🎉 **¡Cuando todo esté ✅, solicita AdSense!**
