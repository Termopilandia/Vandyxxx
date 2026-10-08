# VANDYXX — Sitio Web / Website

Prototipo de sitio web bilingüe (Español / English) para el dúo de DJs **VANDYXX**
([@thevandyxx](https://www.instagram.com/thevandyxx/)).
Diseño dark + neón inspirado en [DJ Z-Trip](https://www.djztrip.com) y
[Tritonal](https://tritonalmusic.com). Listo para subir a **Netlify**.

> Bilingual (Spanish / English) prototype for the DJ duo **VANDYXX**. Dark + neon
> design, ready to deploy on **Netlify**.

---

## 📁 Estructura / Structure

```
Web DJ/
├── index.html                 ← TODO en un solo archivo (HTML + CSS + JS embebidos)
├── netlify.toml               ← configuración Netlify / Netlify config
├── assets/images/             ← AQUÍ van las fotos / PUT photos HERE (ver README.txt)
├── vandyxx_marketing_plan.html ← plan de marketing 12 meses (aparte)
└── README.md
```

> **Archivo único:** todo el CSS y el JavaScript están embebidos dentro de
> `index.html` (en `<style>` y `<script>`). No hay carpetas `css/` ni `js/`.

## 🖼️ Paso 1 — Agregar fotos / Add photos

Ya hay 2 fotos reales puestas (`duo-1.jpg`, `duo-2.jpg`, `hero.jpg`, `og-image.jpg`).
Para mejorar, agrega retratos solos `noelia.jpg` / `essie.jpg` (ver `assets/images/README.txt`).
Sin una foto, el sitio muestra un degradado de relleno (no se rompe).

## 🌐 Paso 2 — Subir a Netlify / Deploy to Netlify

**Opción A — Arrastrar y soltar (la más fácil):**
1. Entra a <https://app.netlify.com/drop>
2. Arrastra **toda la carpeta `Web DJ`** a la ventana.
3. ¡Listo! Netlify te da una URL pública en segundos.

**Opción B — Sitio conectado a Git:**
1. Sube la carpeta a un repo de GitHub.
2. En Netlify: *Add new site → Import from Git* → elige el repo.
3. Publish directory: `.` — Build command: *(vacío)*.

## ✉️ Formularios / Forms

Los formularios de **Booking** y **Newsletter** ya están listos para
**Netlify Forms** (`data-netlify="true"`). Tras el deploy, los mensajes aparecen
en el panel de Netlify → *Forms*. No requieren backend.

## ✏️ Personalizar / Customize

Todo se edita dentro de **`index.html`** (un solo archivo):

| Qué / What | Dónde / Where (dentro de index.html) |
|---|---|
| Textos en 2 idiomas | `<script>` → objeto `I18N` |
| Colores / paleta | `<style>` → `:root` (variables) |
| Video destacado (Reels) | `<script>` → línea `FEATURED_VIDEO` (pega un link de YouTube) |
| Fechas de gira / Tour dates | sección `#tour` |
| Lanzamientos / Releases | sección `#music` |
| Redes sociales / Socials | `footer__socials` |
| Email de booking | `thevandyxx@gmail.com` |

## 🎨 Características / Features

- 🌗 Tema oscuro + acentos neón (magenta / violeta / cian / naranja)
- 🌍 Bilingüe EN/ES con un clic (recuerda el idioma elegido)
- ✨ Animaciones: preloader, glow del cursor, parallax, reveal al scroll, contadores
- 📱 100% responsive (móvil, tablet, escritorio) + menú hamburguesa
- 🎵 Secciones: Hero · About · Music · **Reels** · Tour · Gallery · Booking · Newsletter
- 🔗 Enlaces oficiales del dúo: IG [@thevandyxx](https://www.instagram.com/thevandyxx/) · YT [@TheVandyxx](https://www.youtube.com/@TheVandyxx) · TikTok [@the.vandyxx](https://www.tiktok.com/@the.vandyxx) · [SoundCloud](https://soundcloud.com/the-vandyxx) · [Mixcloud](https://www.mixcloud.com/thevandyxx/)
- ⚡ Un solo archivo, sin dependencias ni build — abre `index.html` y listo

---

Prototipo por **MVP Cluster El Salvador**.
