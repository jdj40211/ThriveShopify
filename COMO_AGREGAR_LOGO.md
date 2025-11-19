# 🎨 Cómo Agregar el Logo de Thrive

Guía rápida para agregar el logo de Thrive a tu tienda.

---

## 📍 Método 1: Desde el Theme Editor (RECOMENDADO)

### Paso a Paso:

1. **Ve al Theme Editor**
   ```
   Shopify Admin
   → Online Store
   → Themes
   → Click "Customize"
   ```

2. **Selecciona el Header**
   ```
   En el panel izquierdo
   → Click en "Header" (arriba)
   → Se abrirá la configuración del header
   ```

3. **Sube el Logo**
   ```
   Busca la opción "Logo"
   → Click en "Select image"
   → Upload del archivo SVG del logo
   ```

4. **Ajusta el Tamaño** (Opcional)
   ```
   Busca "Logo Height"
   → Ajusta el slider (20-120px)
   → Recomendado: 40-50px
   ```

5. **Guarda**
   ```
   Click en "Save" (arriba a la derecha)
   ```

---

## 📍 Método 2: URL Directa del Logo Actual

Si ya tienes el logo subido en Shopify, usa esta URL:

```
https://cdn.shopify.com/s/files/1/0671/2285/6119/files/logoSinFondoThrive.svg?v=1763562361
```

### Cómo usar la URL:

1. **Descarga el logo** desde la URL de arriba
2. **Súbelo** desde el Theme Editor (Método 1)

O alternativamente:

1. **Ve a Settings → Files** en Shopify Admin
2. **Upload** el archivo SVG
3. **Copy** la URL generada
4. Úsala en el Theme Editor

---

## ⚙️ Configuraciones Recomendadas

### Logo Height (Altura del logo):

- **Mobile**: 32-40px (más pequeño para pantallas móviles)
- **Desktop**: 40-50px (tamaño estándar)
- **Large Desktop**: 50-60px (si quieres más impacto)

**Recomendación para Thrive**: `40px` ✅

---

## 🎨 Características del Logo Actual

El logo de Thrive (`logoSinFondoThrive.svg`) tiene estas características:

- ✅ **Formato**: SVG (vectorial, escalable sin perder calidad)
- ✅ **Fondo**: Transparente (sin fondo)
- ✅ **Color**: Negro (se invierte automáticamente en fondos oscuros)
- ✅ **Optimizado**: Para web

---

## 💡 Comportamiento Automático del Logo

El header tiene lógica inteligente que invierte el color del logo automáticamente:

### Cuando el logo es NEGRO:
- ✅ Fondo blanco → Logo negro (normal)
- ✅ Fondo transparente/oscuro → Logo blanco (invertido)

### Cuándo se invierte:
- En headers transparentes (Home, Producto)
- Antes de hacer scroll
- En fondos oscuros

### Cuándo NO se invierte:
- Después de hacer scroll (header blanco)
- En páginas con header sólido
- En fondos blancos

**Esto es automático**, no necesitas configurar nada. ✅

---

## 📱 Cómo Se Ve en Diferentes Pantallas

### Desktop (> 1024px):
```
Logo centrado en el header
Menú a la izquierda
Iconos (búsqueda, cuenta, carrito) a la derecha
```

### Mobile (< 1024px):
```
Menú hamburguesa | Logo | Iconos
```

---

## 🔧 Troubleshooting

### El logo no aparece:

1. **Verifica que el archivo se subió correctamente**
   - Ve a Settings → Files
   - Busca "logoSinFondoThrive.svg"
   - Debe estar ahí

2. **Limpia el caché del navegador**
   - Ctrl + Shift + R (Windows)
   - Cmd + Shift + R (Mac)

3. **Verifica en Theme Editor**
   - Debe verse el logo en la preview
   - Si no, vuelve a subirlo

### El logo se ve muy grande/pequeño:

**Solución:**
```
Theme Editor → Header → Logo Height
Ajusta el slider a 40px (recomendado)
```

### El logo se ve pixelado:

**Causa:** Subiste una imagen JPG/PNG de baja resolución

**Solución:**
- Usa el archivo SVG (vectorial, nunca pierde calidad)
- URL: https://cdn.shopify.com/s/files/1/0671/2285/6119/files/logoSinFondoThrive.svg?v=1763562361

### El logo no se invierte en fondos oscuros:

**Esto es normal si:**
- El header está configurado como "Solid" (sólido)
- Ya hiciste scroll (el header se vuelve blanco)

**Para verificar la inversión:**
- Ve a la Home (sin scroll)
- El logo debe verse blanco si el hero tiene fondo oscuro

---

## 📊 Especificaciones Técnicas

### Formato Actual:
```
Archivo: logoSinFondoThrive.svg
Formato: SVG (Scalable Vector Graphics)
Color: Negro #000000
Fondo: Transparente
Tamaño: Vectorial (escalable infinitamente)
```

### Ubicación en el Código:
```liquid
sections/header.liquid
Líneas 311-361 (Logo mobile y desktop)

Config desde Theme Editor:
- section.settings.logo (imagen)
- section.settings.logo_height (altura en px)
```

### Inversión Automática:
```liquid
:class="(forceSolid || isScrolled) ? 'invert-0' : 'invert-100'"

invert-0 = Logo normal (negro)
invert-100 = Logo invertido (blanco)
```

---

## ✅ Checklist Final

Después de agregar el logo, verifica:

- [ ] El logo aparece en el header (desktop y mobile)
- [ ] El tamaño es apropiado (40-50px recomendado)
- [ ] Se ve bien en fondo blanco (negro)
- [ ] Se invierte en fondos oscuros (blanco)
- [ ] No se pixela al hacer zoom
- [ ] Es clickeable y va a la Home
- [ ] Se ve bien después de hacer scroll

---

## 🎯 Resultado Final

Así debería verse tu header:

```
┌─────────────────────────────────────────────┐
│                                             │
│  SHOP  ▼    [LOGO THRIVE]    🔍 ♡ 👤 🛒   │
│                                             │
└─────────────────────────────────────────────┘
```

Desktop:
- Menú (izquierda)
- Logo (centro)
- Iconos (derecha)

Mobile:
- ☰ Logo | 🔍 👤 🛒

---

**¿Necesitas ayuda?**
Si tienes problemas, verifica que:
1. El archivo SVG esté subido en Settings → Files
2. Esté seleccionado en Theme Editor → Header → Logo
3. Logo Height esté entre 40-50px

🚀 ¡Listo! Tu logo está configurado.
