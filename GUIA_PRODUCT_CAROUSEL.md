# 📦 Guía de Uso - Product Carousel

Esta guía te enseñará cómo usar correctamente la sección **Product Carousel** desde el editor de Shopify.

---

## 🎯 ¿Qué hace esta sección?

El Product Carousel muestra un carrusel de productos que puedes configurar de 4 formas diferentes:
1. **Single Collection** - Productos de una sola colección
2. **Multiple Collections** - Mezcla productos de varias colecciones (3 por colección)
3. **Product Tags** - Filtra productos por etiquetas
4. **Manual Selection** - Selecciona productos manualmente uno por uno

---

## 📋 Paso a Paso: Cómo Usarlo

### 1️⃣ Agregar la Sección

1. Ve a **Online Store > Themes > Customize**
2. Navega a la página donde quieres agregar el carrusel (Home, una página, etc.)
3. Click en **Add section**
4. Busca y selecciona **Product Carousel**

---

### 2️⃣ Configurar el Título

En el panel derecho verás:

**Carousel Title**: Escribe el título del carrusel
- Ejemplo: "Los más vendidos", "Nuevos productos", "Productos destacados"

**Rich Text**: (Opcional) Descripción debajo del título
- Ejemplo: "Descubre nuestros productos más populares"

---

### 3️⃣ Configurar "View All Link" (Opcional)

Si quieres mostrar un enlace "Ver todos":

1. **Show View All Link**: Activa el checkbox ☑️
2. **View All Text**: Escribe el texto (por defecto: "Ver todos")
3. **View All Link**: Agrega la URL
   - Para single collection: Usa este campo
   - Para multiple collections: Usa "View All Link (Multiple Collections)"

---

### 4️⃣ Seleccionar la Fuente de Productos ⚙️

Esta es la parte **MÁS IMPORTANTE**. Aquí seleccionas de dónde vienen los productos.

#### **Opción A: Single Collection** (Recomendada para empezar)

1. En **Product Source**, selecciona **"Single Collection"**
2. En **Collection**, click y selecciona UNA colección
   - Ejemplo: "Best Sellers", "New Arrivals", "Polos"
3. ✅ **Los productos aparecerán inmediatamente**

**Cuándo usar esto:**
- Cuando quieres mostrar productos de una sola categoría
- Es la opción más simple y confiable

---

#### **Opción B: Multiple Collections** (Para mezclar colecciones)

1. En **Product Source**, selecciona **"Multiple Collections"**
2. En **Collections**, click y selecciona VARIAS colecciones
   - Puedes seleccionar hasta 10 colecciones
3. El carrusel mostrará hasta **3 productos de cada colección**
4. ✅ **Los productos aparecerán mezclados**

**Ejemplo:**
Si seleccionas:
- "Polos" (mostrará 3 polos)
- "Hoodies" (mostrará 3 hoodies)
- "Longsleeves" (mostrará 3 longsleeves)

Total: 9 productos en el carrusel, mezclados

**Cuándo usar esto:**
- Cuando quieres mostrar variedad de categorías en un mismo carrusel
- Para mostrar "Lo mejor de cada categoría"

---

#### **Opción C: Product Tags** (Por etiquetas)

1. En **Product Source**, selecciona **"Product Tags"**
2. En **Product Tags**, escribe las etiquetas separadas por comas
   - Ejemplo: `best-seller, new, featured`
3. Los productos que tengan esas etiquetas se mostrarán

**Cuándo usar esto:**
- Cuando tus productos están etiquetados
- Para filtros específicos como "novedad", "oferta", etc.

---

#### **Opción D: Manual Selection** (Selección manual)

1. En **Product Source**, selecciona **"Manual Selection"**
2. En **Manual Product Selection**, click y selecciona productos uno por uno
3. Puedes seleccionar hasta 20 productos
4. Los productos aparecerán en el orden que los seleccionaste

**Cuándo usar esto:**
- Cuando quieres control total sobre qué productos mostrar
- Para promociones específicas
- Para curar una selección especial

---

### 5️⃣ Configurar Límite de Productos

**Maximum Products**: Usa el slider para seleccionar cuántos productos mostrar
- Mínimo: 4
- Máximo: 20
- Recomendado: 8-12

---

### 6️⃣ Configurar la Apariencia de las Tarjetas

Activa o desactiva elementos en las tarjetas de producto:

- ☑️ **Show Product Badges** - Mostrar badges (NEW, SALE, etc.)
- ☑️ **Show Product Rating** - Mostrar estrellas de rating
- ☑️ **Show Color Swatches** - Mostrar colores disponibles
- ☑️ **Show Size Selector** - Mostrar selector de tallas

**Recomendación:** Deja todos activados para una mejor experiencia

---

### 7️⃣ Guardar y Previsualizar

1. Click en **Save** (arriba a la derecha)
2. Previsualiza en diferentes dispositivos usando los iconos de arriba

---

## ⚠️ Solución de Problemas

### "No hay productos disponibles en este momento"

**Causas posibles:**

1. **No seleccionaste una colección/productos**
   - Solución: Verifica que hayas seleccionado una colección o productos

2. **La colección está vacía**
   - Solución: Agrega productos a la colección primero

3. **Todos los productos están "Out of stock"**
   - Solución: Asegúrate de tener productos con inventario disponible

4. **Product Source incorrecto**
   - Solución: Cambia a "Single Collection" para probar

---

### El carrusel se ve muy alto o con espacio vacío

**Causa:** No hay productos para mostrar

**Solución:**
1. Cambia **Product Source** a "Single Collection"
2. Selecciona una colección que tenga productos
3. Verifica que los productos tengan imágenes

---

### Los productos no se desplazan

**Causa:** Puede ser un problema de JavaScript o muy pocos productos

**Solución:**
1. Verifica que tengas al menos 5 productos
2. Actualiza la página (F5)
3. Verifica que **Show Navigation Arrows** esté activado

---

## 💡 Tips y Mejores Prácticas

### ✅ DO (Hacer)

1. **Usa "Single Collection" primero** - Es más fácil y confiable
2. **Asegúrate de tener al menos 6-8 productos** - Para que el carrusel funcione bien
3. **Usa imágenes de buena calidad** - Todas del mismo tamaño si es posible
4. **Activa los badges y swatches** - Mejora la experiencia del usuario
5. **Limita a 12 productos** - No sobrecargues el carrusel

### ❌ DON'T (No hacer)

1. **No mezcles demasiadas colecciones** - Máximo 4-5 colecciones
2. **No pongas más de 20 productos** - El carrusel se vuelve lento
3. **No uses colecciones vacías** - Siempre verifica que tengan productos
4. **No olvides el "View All Link"** - Ayuda a la navegación
5. **No uses etiquetas que no existen** - Verifica tus tags primero

---

## 📊 Ejemplos de Configuración

### Ejemplo 1: "Los más vendidos"

```
Carousel Title: Los más vendidos
Product Source: Single Collection
Collection: Best Sellers
Maximum Products: 12
Show Badges: ✓
Show Rating: ✓
Show Color Swatches: ✓
```

---

### Ejemplo 2: "Productos destacados de todas las categorías"

```
Carousel Title: Productos destacados
Product Source: Multiple Collections
Collections: Polos, Hoodies, Longsleeves
Maximum Products: 12
View All Link (Multiple Collections): /collections/all
```

---

### Ejemplo 3: "Novedades"

```
Carousel Title: Nuevos productos
Product Source: Product Tags
Product Tags: new, nuevo, novedad
Maximum Products: 8
```

---

### Ejemplo 4: "Selección especial Black Friday"

```
Carousel Title: Black Friday Deals
Product Source: Manual Selection
Products: (Seleccionar manualmente)
Maximum Products: 16
Show Badges: ✓ (para mostrar % de descuento)
```

---

## 🎨 Personalización Avanzada

Si quieres cambiar colores, fuentes, o el estilo del carrusel, necesitarás editar los archivos CSS del tema. Contacta a tu desarrollador para esto.

---

## ✅ Checklist Rápido

Antes de publicar, verifica:

- [ ] El título está bien escrito
- [ ] Seleccionaste la fuente de productos correcta
- [ ] Los productos se están mostrando correctamente
- [ ] Las imágenes se ven bien
- [ ] El "View All Link" funciona (si lo agregaste)
- [ ] Se ve bien en mobile y desktop
- [ ] Los badges y swatches funcionan
- [ ] Guardaste los cambios

---

## 🆘 ¿Necesitas Ayuda?

Si después de seguir esta guía todavía tienes problemas:

1. Verifica que tengas productos con inventario disponible
2. Prueba con "Single Collection" primero
3. Revisa que la colección seleccionada tenga productos
4. Contacta a tu desarrollador si el problema persiste

---

**Última actualización:** Noviembre 2025
**Versión:** 2.0
