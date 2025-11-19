# 🔒 Guía Completa - Página de Early Access / Coming Soon

Esta guía te explica cómo usar y configurar la página de password protection para crear una landing page profesional de "Coming Soon" o "Early Access" para tu tienda Thrive.

---

## 📋 Tabla de Contenidos

1. [¿Qué es y para qué sirve?](#qué-es-y-para-qué-sirve)
2. [Activar la Password Protection](#activar-la-password-protection)
3. [Configuración desde el Theme Editor](#configuración-desde-el-theme-editor)
4. [Opciones de Video de Fondo](#opciones-de-video-de-fondo)
5. [Integración de Email Marketing](#integración-de-email-marketing)
6. [Ejemplos de Configuración](#ejemplos-de-configuración)
7. [Preguntas Frecuentes](#preguntas-frecuentes)

---

## 🎯 ¿Qué es y para qué sirve?

La **Password Page** es una página especial que bloquea el acceso a toda tu tienda y muestra una landing page personalizable. Es perfecta para:

- ✅ **Pre-lanzamiento** - Crear expectativa antes de lanzar tu tienda
- ✅ **Mantenimiento** - Mostrar un mensaje mientras haces cambios importantes
- ✅ **Eventos especiales** - Lanzamientos exclusivos con acceso VIP
- ✅ **Recolección de emails** - Construir tu lista de clientes antes del lanzamiento
- ✅ **Countdown** - Crear urgencia con un contador regresivo

### Características incluidas:

- 🎥 **Video de fondo** (YouTube, Vimeo o subido)
- ⏰ **Countdown timer** en tiempo real
- 📧 **Recolección de emails** (Shopify, Klaviyo, Mailchimp)
- 🔗 **Links sociales** (Instagram, TikTok, Twitter, Facebook)
- 🔑 **Entrada con contraseña** para acceso VIP
- 🎨 **Totalmente personalizable** desde el Theme Editor
- 📱 **100% responsive** en todos los dispositivos

---

## 🔓 Activar la Password Protection

### Paso 1: Activar en Shopify Admin

1. Ve a **Shopify Admin**
2. Click en **Online Store** → **Preferences**
3. Scroll hasta la sección **"Password protection"**
4. ☑️ Activa **"Restrict access to visitors with the password"**
5. **Configura la contraseña:**
   - **Para acceso VIP:** Pon una contraseña que solo tú conoces
   - **Solo para mostrar la página:** Deja el campo vacío o usa una genérica
6. Click en **Save**

### Paso 2: Personalizar la Página

1. Ve a **Online Store** → **Themes**
2. Click en **Customize** en tu tema activo
3. En el dropdown de páginas, selecciona **"Password"**
4. Ahora verás todas las opciones de personalización ⚙️

---

## ⚙️ Configuración desde el Theme Editor

Una vez en el Theme Editor en la página de Password, verás estas secciones:

### 🖼️ **Logo**

| Opción | Descripción |
|--------|-------------|
| **Show Logo** | Activa/desactiva el logo |
| **Logo Image** | Sube tu logo (PNG transparente recomendado) |
| **Logo Width** | Ancho del logo en píxeles (100-400px) |

💡 **Tip:** Si no subes logo, se mostrará el nombre de tu tienda automáticamente.

---

### 🎥 **Background Video/Image**

| Opción | Descripción | Cuándo usar |
|--------|-------------|-------------|
| **Background Type** | Tipo de fondo a mostrar | - |
| - Upload Video | Video subido a Shopify | Mejor calidad, control total |
| - YouTube | Video de YouTube | Fácil de usar, no consume espacio |
| - Vimeo | Video de Vimeo | Profesional, sin ads |
| - Image Only | Solo imagen estática | Más rápido de cargar |
| **Video URL** | URL del video subido | Sube a Shopify Files primero |
| **YouTube Video ID** | ID del video de YouTube | Ejemplo: `dQw4w9WgXcQ` |
| **Vimeo Video ID** | ID del video de Vimeo | Ejemplo: `123456789` |
| **Background Image** | Imagen de fondo | Fallback si no hay video |
| **Video Poster** | Imagen mientras carga el video | Mejora la experiencia |
| **Dark Overlay Opacity** | Opacidad de la capa oscura (0-90%) | Para mejor legibilidad |

#### 📹 Cómo subir video a Shopify:

1. Ve a **Settings** → **Files**
2. Click en **Upload files**
3. Sube tu video (.mp4 recomendado, máx 20MB)
4. Una vez subido, click derecho → **Copy link**
5. Pega el link en **Video URL**

#### 🎬 Cómo obtener YouTube Video ID:

De esta URL: `https://www.youtube.com/watch?v=dQw4w9WgXcQ`
El ID es: `dQw4w9WgXcQ` (lo que viene después de `v=`)

#### 📺 Cómo obtener Vimeo Video ID:

De esta URL: `https://vimeo.com/123456789`
El ID es: `123456789` (los números finales)

---

### ✏️ **Content**

| Opción | Descripción | Ejemplo |
|--------|-------------|---------|
| **Heading** | Título principal | "THRIVE Coming Soon" |
| **Subheading** | Subtítulo descriptivo | "Something extraordinary is on the way" |
| **Text Color** | Color del texto | `#ffffff` (blanco) |

---

### ⏰ **Countdown Timer**

| Opción | Descripción | Valor recomendado |
|--------|-------------|-------------------|
| **Show Countdown** | Activa/desactiva el contador | ☑️ Activado |
| **Launch Date** | Fecha y hora del lanzamiento | `2025-12-31T23:59:59` |
| **Days Label** | Etiqueta de "días" | "Días" |
| **Hours Label** | Etiqueta de "horas" | "Horas" |
| **Minutes Label** | Etiqueta de "minutos" | "Minutos" |
| **Seconds Label** | Etiqueta de "segundos" | "Segundos" |
| **Countdown Expired Text** | Texto cuando termine | "¡Ya estamos en vivo!" |

#### 📅 Formato de fecha:

```
YYYY-MM-DDTHH:MM:SS
```

Ejemplos:
- `2025-12-31T23:59:59` → 31 de diciembre 2025, 11:59:59 PM
- `2025-06-15T12:00:00` → 15 de junio 2025, 12:00:00 PM (mediodía)
- `2025-01-01T00:00:00` → 1 de enero 2025, 12:00:00 AM (medianoche)

💡 **Tip:** El countdown se actualiza cada segundo automáticamente.

---

### 📧 **Email Collection**

Esta es una de las partes más importantes: recolectar emails de clientes potenciales.

#### Opciones generales:

| Opción | Descripción |
|--------|-------------|
| **Show Email Form** | Activa/desactiva el formulario |
| **Email Service** | Servicio de email a usar |
| **Form Text** | Texto encima del formulario |
| **Email Placeholder** | Placeholder del input |
| **Button Text** | Texto del botón |
| **Success Message** | Mensaje al suscribirse |
| **Button Color** | Color de fondo del botón |
| **Button Text Color** | Color del texto del botón |

#### Servicios disponibles:

##### 1️⃣ **Shopify (Built-in)** - RECOMENDADO PARA EMPEZAR

✅ **Ventajas:**
- No requiere configuración adicional
- Gratis
- Los emails se guardan en Shopify Admin

📍 **Dónde ver los emails recolectados:**
1. Ve a **Customers** en Shopify Admin
2. Verás todos los emails que se suscribieron
3. Puedes exportarlos a CSV

⚙️ **Configuración:**
- Solo selecciona "Shopify (Built-in)" y listo

---

##### 2️⃣ **Klaviyo** - PARA MARKETING AVANZADO

✅ **Ventajas:**
- Herramienta profesional de email marketing
- Automatizaciones potentes
- Segmentación avanzada
- Análisis detallados

📍 **Cómo configurar:**

1. **Obtener API Key:**
   - Ve a [Klaviyo](https://www.klaviyo.com)
   - Click en **Settings** → **API Keys**
   - Copia tu **Private API Key**

2. **Obtener List ID:**
   - Ve a **Lists & Segments**
   - Click en la lista donde quieres guardar los emails
   - En la URL verás algo como: `.../list/AbCd12`
   - Copia el ID final (ejemplo: `AbCd12`)

3. **En el Theme Editor:**
   - **Email Service:** Selecciona "Klaviyo"
   - **Klaviyo API Key:** Pega tu API Key
   - **Klaviyo List ID:** Pega el List ID

---

##### 3️⃣ **Mailchimp** - ALTERNATIVA POPULAR

✅ **Ventajas:**
- Conocido y fácil de usar
- Plan gratuito hasta 500 contactos
- Integraciones múltiples

📍 **Cómo configurar:**

1. **Crear un formulario en Mailchimp:**
   - Ve a **Audience** → **Signup forms**
   - Click en **Embedded forms**
   - Copia el código HTML

2. **Obtener la Action URL:**
   Del código HTML, busca la línea que dice:
   ```html
   <form action="https://yourdomain.us1.list-manage.com/subscribe/post?u=123&id=456">
   ```
   Copia toda la URL del `action="..."`

3. **En el Theme Editor:**
   - **Email Service:** Selecciona "Mailchimp"
   - **Mailchimp Form Action URL:** Pega la URL

---

### 🔗 **Social Links**

| Opción | Descripción | Ejemplo |
|--------|-------------|---------|
| **Show Social Links** | Activa/desactiva los iconos | ☑️ Activado |
| **Instagram URL** | Link de Instagram | `https://instagram.com/thrive` |
| **TikTok URL** | Link de TikTok | `https://tiktok.com/@thrive` |
| **Twitter URL** | Link de Twitter/X | `https://twitter.com/thrive` |
| **Facebook URL** | Link de Facebook | `https://facebook.com/thrive` |

💡 **Tip:** Los iconos solo aparecen si pones la URL. Puedes usar solo los que quieras.

---

### 🔑 **Password Entry (Optional)**

Esta opción permite que ciertas personas (VIP, prensa, colaboradores) entren con contraseña mientras la tienda está bloqueada.

| Opción | Descripción |
|--------|-------------|
| **Show Password Entry** | Muestra/oculta el botón de contraseña |
| **Password Toggle Text** | Texto del botón toggle |
| **Password Placeholder** | Placeholder del input de contraseña |
| **Password Button Text** | Texto del botón de enviar |

💡 **Tip:** El botón aparece pequeño abajo de todo. Al hacer click, se despliega el formulario de contraseña.

---

## 🎨 Ejemplos de Configuración

### Ejemplo 1: Pre-lanzamiento Minimalista

```
Background Type: Image Only
Background Image: [Foto del producto/brand en blanco y negro]
Dark Overlay Opacity: 60%

Heading: "THRIVE"
Subheading: "Coming January 2025"
Text Color: #ffffff

Show Countdown: ✓
Launch Date: 2025-01-15T00:00:00

Show Email Form: ✓
Email Service: Shopify
Form Text: "Join the waitlist"
Button Color: #ffffff
Button Text Color: #000000

Show Social: ✓
Instagram URL: https://instagram.com/thrive
TikTok URL: https://tiktok.com/@thrive

Show Password Entry: ✗
```

**Resultado:** Página limpia, elegante, enfocada en recolectar emails.

---

### Ejemplo 2: Lanzamiento Épico con Video

```
Background Type: YouTube
YouTube Video ID: dQw4w9WgXcQ (reemplaza con tu video)
Dark Overlay Opacity: 50%
Video Poster: [Imagen de alta calidad del primer frame]

Heading: "THE FUTURE IS HERE"
Subheading: "Something extraordinary is dropping soon"
Text Color: #ffffff

Show Countdown: ✓
Launch Date: 2025-12-31T23:59:59
Days Label: "DÍAS"
Hours Label: "HRS"
Minutes Label: "MIN"
Seconds Label: "SEG"

Show Email Form: ✓
Email Service: Klaviyo
Klaviyo API Key: [tu API key]
Klaviyo List ID: [tu list ID]
Form Text: "Be the first to experience it"
Button Color: #3B2E10
Button Text Color: #ffffff

Show Social: ✓
Instagram, TikTok, Twitter: [todos tus links]

Show Password Entry: ✓
Password Toggle Text: "VIP Access"
```

**Resultado:** Experiencia inmersiva con video, countdown dramático, y acceso VIP.

---

### Ejemplo 3: Mantenimiento Rápido

```
Background Type: Image Only
Background Image: [Logo o imagen simple]
Dark Overlay Opacity: 70%

Heading: "We'll be right back"
Subheading: "We're making some improvements. Check back soon!"
Text Color: #ffffff

Show Countdown: ✗
Show Email Form: ✗
Show Social: ✓
Show Password Entry: ✓
```

**Resultado:** Página simple para mantenimiento con acceso para el equipo.

---

## 📊 Mejores Prácticas

### ✅ DO (Hacer)

1. **Usa video de alta calidad pero optimizado**
   - Máximo 20MB para videos subidos
   - Usa YouTube/Vimeo para videos largos o pesados
   - Siempre pon un Video Poster para mejor experiencia

2. **Configura el countdown con fecha real**
   - No uses fechas muy lejanas (genera desinterés)
   - 2-4 semanas es ideal para mantener expectativa

3. **Recolecta emails desde el día 1**
   - Es tu activo más valioso
   - Usa Klaviyo si planeas hacer email marketing

4. **Optimiza el overlay opacity**
   - 40-60% es ideal
   - Debe permitir ver el video pero leer el texto

5. **Mantén el mensaje simple y claro**
   - Heading corto y poderoso
   - Subheading que genere curiosidad

### ❌ DON'T (No hacer)

1. **No uses videos muy largos o pesados**
   - Hace que la página cargue lento
   - Usa loops cortos (10-30 segundos)

2. **No olvides poner fecha de lanzamiento**
   - Sin countdown, pierdes urgencia
   - Actualiza la fecha si se retrasa

3. **No ignores el mobile**
   - 60-70% del tráfico es mobile
   - Revisa siempre en celular

4. **No uses demasiados colores**
   - Mantén una paleta simple
   - Blanco sobre oscuro es más legible

5. **No dejes la password page activa más de lo necesario**
   - Desactívala en cuanto lances
   - Pierdes ventas cada día que esté activa

---

## 🎯 Casos de Uso Específicos

### 🚀 **Pre-lanzamiento de marca nueva**

**Objetivo:** Construir lista de emails y generar expectativa

**Configuración:**
- Video/Imagen impactante de la marca
- Countdown a fecha de lanzamiento
- Email form con Klaviyo
- Social media activo
- Password entry desactivado

**Duración:** 2-4 semanas antes del lanzamiento

---

### 🎁 **Lanzamiento de colección exclusiva**

**Objetivo:** Crear urgencia y exclusividad

**Configuración:**
- Video de la colección
- Countdown corto (3-7 días)
- Email form para early access
- Password entry para VIPs
- Social media con teaser

**Duración:** 1 semana

---

### 🛠️ **Mantenimiento temporal**

**Objetivo:** Informar sin perder clientes

**Configuración:**
- Imagen del logo/brand
- Sin countdown (o countdown a "volvemos")
- Sin email form (ya tienes clientes)
- Password entry para equipo
- Link a social media para updates

**Duración:** Horas a 1-2 días máximo

---

### 🎪 **Evento especial / Drop**

**Objetivo:** Generar hype máximo

**Configuración:**
- Video hype del producto/evento
- Countdown preciso al minuto
- Email form con beneficio ("early access")
- Social media muy activo
- Password opcional para prensa/influencers

**Duración:** 1-2 semanas

---

## 🔧 Solución de Problemas

### El video no se reproduce

**Posibles causas:**
- Video muy pesado (>20MB)
- Formato no soportado (usa .mp4)
- URL incorrecta en YouTube/Vimeo

**Solución:**
1. Verifica el formato del video
2. Comprime el video con [Handbrake](https://handbrake.fr/)
3. Usa YouTube/Vimeo para videos grandes
4. Verifica que el ID de YouTube/Vimeo sea correcto

---

### El countdown no funciona

**Posibles causas:**
- Formato de fecha incorrecto
- Fecha en el pasado
- JavaScript deshabilitado

**Solución:**
1. Verifica el formato: `YYYY-MM-DDTHH:MM:SS`
2. Asegúrate que la fecha sea futura
3. Prueba en navegador diferente
4. Verifica que "Show Countdown" esté activado

---

### Los emails no se guardan

**Shopify:**
- Verifica en **Customers** del admin
- Los emails aparecen como "Accepts Marketing: Yes"

**Klaviyo:**
- Verifica que el API Key sea correcto
- Verifica que el List ID sea correcto
- Revisa en Klaviyo si hay errores de API

**Mailchimp:**
- Verifica que la Action URL sea completa
- No modifiques la URL (debe tener `?u=` y `&id=`)

---

### La página se ve rara en mobile

**Solución:**
1. Reduce el tamaño del heading (se ajusta automático pero verifica)
2. Usa un Dark Overlay más opaco (60-70%)
3. Verifica que el video poster esté en vertical u horizontal según diseño
4. Revisa en **Mobile preview** del Theme Editor

---

## 📱 Cómo Desactivar la Password Page

Cuando estés listo para lanzar:

1. Ve a **Online Store** → **Preferences**
2. Desactiva ☐ **"Restrict access to visitors with the password"**
3. Click en **Save**

¡Y listo! Tu tienda estará pública.

💡 **Tip:** No borres la configuración de la password page. Puedes volver a activarla en el futuro para otro lanzamiento.

---

## 🎓 Tips de Marketing

### Antes del lanzamiento (1-2 semanas)

1. **Activa la password page**
2. **Configura el countdown**
3. **Comparte en redes sociales:**
   - "Something big is coming... 👀"
   - "Link in bio to join the waitlist"
4. **Corre ads a la password page** (Facebook/Instagram)
5. **Colabora con influencers** para compartir

### Durante el countdown (última semana)

1. **Envía recordatorios a la lista de emails**
2. **Actualiza redes sociales con sneak peeks**
3. **Crea urgencia:**
   - "Only 3 days left!"
   - "48 hours until launch"
4. **Prepara el inventario**

### Día del lanzamiento

1. **Desactiva la password page** a la hora exacta
2. **Envía email a la lista** anunciando el lanzamiento
3. **Post en redes sociales** con link directo
4. **Monitorea el sitio** para posibles errores
5. **Responde comentarios y preguntas** rápidamente

---

## 📊 Métricas a Seguir

### Antes del lanzamiento:

- **Emails recolectados** (meta: 100-1000+ según tu audiencia)
- **Tráfico a la password page** (Google Analytics)
- **Engagement en redes sociales** (shares, comments)
- **Tasa de conversión** (visitantes → emails)

### Día del lanzamiento:

- **Conversión de emails a ventas** (cuántos compraron)
- **Tráfico de diferentes fuentes** (email, social, ads)
- **Valor promedio de orden**
- **Productos más vendidos**

---

## ✅ Checklist Final

Antes de activar la password page, verifica:

- [ ] Video/imagen de fondo está configurado y se ve bien
- [ ] Dark overlay permite leer el texto
- [ ] Heading y subheading están bien escritos (sin typos)
- [ ] Countdown tiene la fecha correcta
- [ ] Email form está funcionando (haz una prueba)
- [ ] Los emails se están guardando correctamente
- [ ] Links de social media funcionan
- [ ] Se ve bien en mobile (revisa en tu celular)
- [ ] Password de Shopify está configurada
- [ ] Tienes plan de marketing para promocionar

---

## 🆘 Soporte

¿Necesitas ayuda?

1. **Revisa esta guía** primero
2. **Prueba en diferentes navegadores**
3. **Verifica la consola** del navegador (F12) para errores
4. **Contacta al equipo** si el problema persiste

---

**Última actualización:** Noviembre 2025
**Versión:** 1.0

---

## 🎉 ¡Listo!

Ya tienes todo lo que necesitas para crear una experiencia de pre-lanzamiento épica. Recuerda:

- 🎥 **Video de calidad** genera más engagement
- ⏰ **Countdown** crea urgencia
- 📧 **Emails** son tu activo más valioso
- 📱 **Mobile first** siempre

¡Mucha suerte con tu lanzamiento! 🚀
