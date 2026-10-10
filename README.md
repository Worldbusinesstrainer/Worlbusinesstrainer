# World Business Trainer — Sitio Web

Sitio web estático (HTML, CSS y JavaScript) para World Business Trainer, agencia de diseño y desarrollo web en Costa Rica especializada en clínicas dentales y agentes inmobiliarios.

---

## 📁 Estructura del proyecto

```
world-business-trainer/
├── index.html
├── README.md
├── css/styles.css
├── js/main.js
└── assets/
    ├── favicon.svg
    └── hero.svg
```

---

## ⚙️ Cómo editar textos, colores, correo y WhatsApp

### 1. Número de WhatsApp y correo electrónico

Abrí el archivo `js/main.js` y modificá las primeras líneas:

```js
const WHATSAPP_NUMBER = "50600000000"; // ⚙️ Reemplazar por tu número real
const CONTACT_EMAIL   = "contacto@tudominio.com"; // ⚙️ Reemplazar
```

Reglas del número:
- Formato internacional, sin `+`, sin espacios, sin guiones.
- Costa Rica usa el prefijo `506`.
- Ejemplo: `50688887777`.

Además, reemplazá manualmente los enlaces visibles en `index.html`:

- Los enlaces con atributo `data-wa` se actualizan automáticamente desde `js/main.js`.
- El correo aparece como texto: buscá `contacto@tudominio.com` en `index.html` y cambialo.
- El teléfono visible: buscá `+506 0000 0000` y cambialo por tu número con formato legible.

### 2. Colores de marca

Abrí `css/styles.css` y editá las variables al inicio del archivo:

```css
:root {
  --color-primary: #0B2545;   /* Azul oscuro principal */
  --color-accent:  #1FA2A6;   /* Turquesa */
  --color-accent-2:#4FC3F7;   /* Azul claro */
  ...
}
```

### 3. Textos generales

Todos los textos están directamente en `index.html`, organizados por secciones comentadas:
`HEADER`, `HERO`, `PROBLEMAS`, `SERVICIOS`, `CLÍNICAS DENTALES`, `INMOBILIARIO`, `PROCESO`, `PAQUETES`, `FAQ`, `CONTACTO`, `FOOTER`.

---

## 🚀 Publicar gratis en GitHub Pages

### Paso 1 — Crear el repositorio
1. Ingresá a [github.com](https://github.com) y creá una cuenta si no tenés.
2. Hacé clic en **New repository**.
3. Nombre sugerido: `world-business-trainer`.
4. Marcalo como **Public**.
5. Clic en **Create repository**.

### Paso 2 — Subir los archivos
Opción A (interfaz web, más simple):
1. En el repositorio, clic en **Add file → Upload files**.
2. Arrastrá todos los archivos y carpetas del proyecto (`index.html`, `css/`, `js/`, `assets/`, `README.md`).
3. Clic en **Commit changes**.

Opción B (línea de comandos):
```bash
git init
git add .
git commit -m "Sitio web World Business Trainer"
git branch -M main
git remote add origin https://github.com/TU-USUARIO/world-business-trainer.git
git push -u origin main
```

### Paso 3 — Activar GitHub Pages
1. Entrá al repositorio en GitHub.
2. Ir a **Settings → Pages**.
3. En **Source**, seleccioná **Deploy from a branch**.
4. Branch: **main**, carpeta: **/ (root)**.
5. Clic en **Save**.
6. Esperá 1–2 minutos. Tu sitio quedará publicado en:

```
https://TU-USUARIO.github.io/world-business-trainer/
```

### Paso 4 — Dominio propio (opcional)
1. Comprá un dominio (por ejemplo `worldbusinesstrainer.com`).
2. En **Settings → Pages → Custom domain**, ingresá el dominio.
3. Configurá los registros DNS con tu proveedor:
   - Tipo `A` apuntando a `185.199.108.153`, `185.199.109.153`, `185.199.110.153`, `185.199.111.153`.
   - O tipo `CNAME` para `www` apuntando a `TU-USUARIO.github.io`.

---

## 🔧 Funciones que necesitan configuración adicional

Estas funciones están **preparadas pero requieren conexión externa** para funcionar al 100%:

1. **Formulario de contacto** — Actualmente abre WhatsApp con los datos precargados. Para envío por correo real, integrá un servicio como [Formspree](https://formspree.io), [Getform](https://getform.io) o [Web3Forms](https://web3forms.com) modificando el `<form>` en `index.html` y su `action` en `js/main.js`.
2. **Analítica web** — Se recomienda agregar Google Analytics o Plausible antes de `</head>` en `index.html`.
3. **SEO avanzado** — Reemplazar URLs canónicas, generar `sitemap.xml` y `robots.txt` con tu dominio final.
4. **Correo comercial** — El correo mostrado es un placeholder. Configurá tu dirección real (por ejemplo con Zoho Mail gratis o Google Workspace).
5. **Mapa de ubicación** — Si querés mostrar un mapa en la sección de contacto, agregá un `<iframe>` de Google Maps.
6. **Favicon y Open Graph** — Reemplazar por imágenes de marca definitivas cuando estén disponibles.

---

## ✅ Verificaciones finales

- [x] Enlaces internos funcionales (`#top`, `#servicios`, `#clinicas`, `#inmobiliario`, `#contacto`).
- [x] Diseño responsive (móvil, tablet, escritorio).
- [x] Botón flotante de WhatsApp operativo.
- [x] Formulario con validación básica en JavaScript.
- [x] Sin claves ni datos sensibles en el código.
- [x] Optimizado para GitHub Pages (sin build, sin dependencias).

---

## 📄 Licencia

© World Business Trainer. Todos los derechos reservados.
