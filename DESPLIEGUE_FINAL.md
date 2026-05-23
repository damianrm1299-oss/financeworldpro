# 🚀 DESPLIEGUE FINAL — Lista de pasos exactos

> **Tu proyecto está 100% listo localmente.** Solo te queda hacer 6 acciones concretas en plataformas externas. Tiempo total estimado: **15 minutos**.

---

## ✅ Lo que YA está hecho (no toques nada)

- ✅ 11 archivos HTML, MD y de configuración listos
- ✅ Diseño editorial profesional aplicado
- ✅ SEO meta tags, Open Graph, Schema.org
- ✅ Scripts de AdSense con placeholders en posiciones óptimas
- ✅ Banner de cookies RGPD
- ✅ Disclaimer financiero "Nota del Editor"
- ✅ Páginas legales (privacidad, términos, sobre nosotros, contacto)
- ✅ ads.txt, robots.txt, sitemap.xml
- ✅ Repositorio Git inicializado con commit inicial
- ✅ ZIP de despliegue en `C:\Users\34642\financeworld-pro-GITHUB.zip`

---

## 📦 Lo que tienes preparado para subir

```
financeworld-pro/
├── index.html                ← Editorial + AdSense (página principal)
├── privacidad.html           ← Política RGPD
├── terminos.html             ← Términos y condiciones
├── sobre-nosotros.html       ← About
├── contacto.html             ← Formulario contacto
├── 404.html                  ← Página de error
├── ads.txt                   ← Verificación AdSense
├── robots.txt                ← Para crawlers
├── sitemap.xml               ← Mapa del sitio
├── README.md                 ← Documentación
└── GUIA_ADSENSE.md           ← Guía paso a paso
```

---

# 🎯 LOS 6 PASOS QUE FALTAN

## PASO 1 — Crear cuenta de GitHub (3 min)

Si ya tienes cuenta, **salta al paso 2**.

1. Ve a 👉 **https://github.com/signup**
2. Email: `damianrm1299@gmail.com`
3. Contraseña fuerte (apúntala bien)
4. Username sugerido: `damianrm` o `damianrm1299` (elige el que esté libre)
5. Verifica el email que te enviarán

**📌 Apunta tu username. Lo usarás en el paso 4.**

---

## PASO 2 — Crear el repositorio (1 min)

1. Inicia sesión en https://github.com
2. Pulsa el botón verde **"New"** (o el `+` arriba a la derecha → "New repository")
3. Rellena:
   ```
   Repository name: financeworld-pro
   Description:     Portal editorial de mercados financieros globales
   ◉ Public           ← OBLIGATORIO para GitHub Pages gratuito
   ☐ Add README       ← NO marcar (ya lo tienes)
   ☐ Add .gitignore   ← NO marcar (ya lo tienes)
   ☐ License          ← NO marcar
   ```
4. Pulsa el botón verde **"Create repository"**

---

## PASO 3 — Subir los archivos (3 min)

### MÉTODO MÁS FÁCIL — Drag & Drop

1. En tu repositorio nuevo verás un enlace que dice: **"uploading an existing file"**
2. Pulsa ese enlace
3. **Abre el Explorador de Windows** y ve a `C:\Users\34642\financeworld-pro\`
4. Selecciona **TODOS los archivos** (Ctrl+A) — **excepto la carpeta `backup/`**
5. **Arrástralos a la zona de GitHub** que dice "Drag files here..."
6. Espera a que carguen
7. En el mensaje de commit pon: `Initial commit`
8. Pulsa el botón verde **"Commit changes"**

### MÉTODO ALTERNATIVO — Con ZIP

Si arrastrar muchos archivos da problemas, **descomprime primero el ZIP**:
- ZIP: `C:\Users\34642\financeworld-pro-GITHUB.zip`
- Doble clic → Extraer en una carpeta
- Arrastra los archivos extraídos a GitHub

> ⚠️ GitHub NO acepta ZIPs directamente. Tienes que descomprimirlo y subir los archivos sueltos.

---

## PASO 4 — Activar GitHub Pages (1 min)

1. En tu repositorio, pulsa la pestaña **"Settings"** (arriba)
2. En el menú lateral izquierdo busca y pulsa **"Pages"**
3. En **"Build and deployment"** → **"Source"** selecciona:
   ```
   Branch:  main
   Folder:  / (root)
   ```
4. Pulsa **"Save"**
5. **Espera 2-3 minutos** y refresca la página
6. Verás un mensaje verde con tu URL:
   ```
   ✅ Your site is live at https://TU-USUARIO.github.io/financeworld-pro/
   ```

🎉 **¡Tu web ya está online!** Cualquier persona en el mundo puede entrar.

---

## PASO 5 — Reemplazar `TU-USUARIO` en los archivos

Tienes que reemplazar `TU-USUARIO` por tu usuario real de GitHub.

### Archivos donde hay que cambiarlo:

| Archivo | Ocurrencias |
|---------|-------------|
| `index.html` | 3 veces |
| `robots.txt` | 1 vez |
| `sitemap.xml` | 5 veces |
| `README.md` | 2 veces |

### Cómo hacerlo desde GitHub (sin descargar nada):

1. Abre cada archivo en GitHub
2. Pulsa el icono del **lápiz ✏️** (arriba a la derecha del archivo)
3. Usa **Ctrl+F** para buscar `TU-USUARIO`
4. Sustitúyelo por tu username real (ejemplo: si tu user es `damianrm`, queda `damianrm`)
5. Abajo del todo: **"Commit changes"**

Repite para los 4 archivos.

---

## PASO 6 — Solicitar Google AdSense (DESPUÉS DE 2-4 SEMANAS)

⚠️ **MUY IMPORTANTE:** AdSense **rechaza webs muy nuevas**. Espera al menos **2 semanas** antes de solicitar. Durante ese tiempo:

- ✅ Comparte tu web en redes sociales
- ✅ Pide a amigos que la visiten
- ✅ Intenta tener algo de tráfico orgánico

### Cuando llegue el momento:

1. Ve a 👉 **https://adsense.google.com**
2. **"Empezar"** → Entra con tu cuenta Google (`damianrm1299@gmail.com`)
3. Introduce:
   - URL del sitio: `https://TU-USUARIO.github.io/financeworld-pro/`
   - País: España
4. Acepta términos
5. Configura tu cuenta bancaria (IBAN español) para cobrar
6. Google te dará tu **Publisher ID** con formato `ca-pub-1234567890123456`

### Cómo conectar AdSense con tu web:

En tu repo de GitHub, edita `index.html`:

1. **Reemplaza TODAS las ocurrencias** de `ca-pub-XXXXXXXXXXXXXXXX` por tu Publisher ID real
2. Hazlo también en `ads.txt` (allí va sin el "ca-", solo `pub-XXXX...`)
3. Commit cambios

Espera la aprobación de AdSense (1 día a 4 semanas).

---

# 📋 CHECKLIST FINAL DEL DESPLIEGUE

Marca cada paso a medida que lo completes:

- [ ] **1.** Cuenta de GitHub creada
- [ ] **2.** Repositorio `financeworld-pro` creado (Public)
- [ ] **3.** Los 11 archivos subidos al repositorio
- [ ] **4.** GitHub Pages activado, URL funcionando
- [ ] **5.** `TU-USUARIO` reemplazado en index.html, robots.txt, sitemap.xml, README.md
- [ ] **6.** Web compartida en redes durante 2-4 semanas
- [ ] **7.** Cuenta de AdSense creada
- [ ] **8.** Publisher ID obtenido (`ca-pub-XXXXXXXX`)
- [ ] **9.** Publisher ID reemplazado en index.html y ads.txt
- [ ] **10.** AdSense aprobado y mostrando anuncios

---

# 💰 Ingresos estimados (referencia realista)

| Visitas/mes | Ingresos aproximados (nicho financiero) |
|-------------|-----------------------------------------|
| 1.000 | 2 – 8 € |
| 10.000 | 20 – 80 € |
| 50.000 | 100 – 400 € |
| 100.000 | 200 – 800 € |
| 500.000 | 1.000 – 4.000 € |

> El nicho financiero (CPM alto) paga 2-3× más que la media. Una sola visita de calidad puede valer 0.20–0.50 €.

---

# 🆘 Si te bloqueas en algún paso

Dime exactamente en qué paso estás y qué ves en pantalla. Te ayudo a desbloquear ese paso concreto.

Ejemplos:
- *"He llegado al paso 3 pero no me deja subir los archivos"*
- *"GitHub Pages dice que mi site está live pero veo error 404"*
- *"AdSense me ha rechazado, qué hago"*

---

# 🎯 Resumen ejecutivo

**Tu proyecto está al 100% listo en local.** Solo necesitas:

1. 🌐 **Crear cuenta GitHub** (3 min) — `https://github.com/signup`
2. 📦 **Subir archivos** desde `C:\Users\34642\financeworld-pro\` (3 min)
3. ⚡ **Activar GitHub Pages** en Settings → Pages (1 min)
4. ✏️ **Reemplazar `TU-USUARIO`** en 4 archivos (2 min)
5. ⏳ **Esperar 2-4 semanas** con algo de tráfico
6. 💰 **Solicitar AdSense** y reemplazar Publisher ID (5 min)

**= 15 minutos de trabajo activo + 2-4 semanas de espera técnica de Google.**

🚀 ¡Mucha suerte!
