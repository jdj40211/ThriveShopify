# 🎠 Guía de Uso - Content Carousel

Guía rápida para configurar el Content Carousel con todas sus opciones.

---

## 📋 Configuración Básica

### 1. Agregar la Sección

1. Ve a **Theme Editor**
2. Click en **Add section**
3. Selecciona **Content Carousel**

---

## ⚙️ Opciones de Configuración

### **Título y Enlaces**

- **Carousel Title**: Título del carrusel
- **Show View All Link**: Activa para mostrar "Ver todos"
- **View All Text**: Texto del enlace (por defecto: "Ver todos")
- **View All Link**: URL del enlace

---

### **Navegación**

#### **Show Navigation Arrows** ☑️
- **Activado (por defecto)**: Muestra las flechas ← →
- **Desactivado**: Oculta las flechas, solo navegación táctil/arrastre

**Cuándo desactivar:**
- Si usas autoplay (el carrusel se mueve solo)
- Para una experiencia más minimalista
- En mobile donde el swipe es más natural

---

### **Carousel Settings**

#### **Items per view (desktop)**
- **Rango**: 1 a 6 items
- **Por defecto**: 5
- Cuántos elementos se ven al mismo tiempo en pantallas grandes

#### **Gap between items**
- **Rango**: 0 a 40px
- **Por defecto**: 8px (reducido para mejor apariencia)
- Espacio entre las tarjetas del carrusel

**Recomendaciones:**
- **0-8px**: Carrusel compacto y moderno ✅
- **12-16px**: Espaciado medio
- **20-40px**: Carrusel espaciado

---

### **📐 Card Size** (NUEVO)

Controla el tamaño y proporción de las tarjetas individuales.

#### **Card Aspect Ratio**
Selecciona la proporción de aspecto de las imágenes:

- **Square (1:1)**: Formato cuadrado, ideal para logos o íconos
- **Portrait (2:3)**: Formato vertical (por defecto), perfecto para fotos de productos o personas
- **Landscape (4:3)**: Formato horizontal clásico, bueno para paisajes
- **Wide (16:9)**: Formato panorámico, ideal para banners o escenas amplias

**Recomendaciones por tipo de contenido:**
- **Fotos de personas/productos**: Portrait (2:3) ✅
- **Logos/iconos**: Square (1:1)
- **Paisajes/escenas**: Landscape (4:3) o Wide (16:9)
- **Banners promocionales**: Wide (16:9)

#### **Card Max Width**
- **Rango**: 200px a 500px
- **Por defecto**: 280px
- Controla el ancho máximo de cada tarjeta

**Recomendaciones:**
- **200-240px**: Tarjetas pequeñas, muestra más items
- **260-300px**: Tamaño estándar (óptimo) ✅
- **320-400px**: Tarjetas grandes, más impacto visual
- **400-500px**: Tarjetas muy grandes, menos items visibles

💡 **Tip:** Si usas `Card Max Width` grande, reduce `Items per view` para que no se vea apretado.

---

### **🔄 Autoplay / Infinite Scroll**

#### **Enable Autoplay** ☑️
Activa el desplazamiento automático e infinito del carrusel.

**Cuando está activado:**
- ✅ El carrusel se mueve automáticamente
- ✅ Loop infinito (vuelve al inicio cuando llega al final)
- ✅ Se pausa cuando pasas el mouse encima
- ✅ Continúa cuando quitas el mouse

**Cuando está desactivado:**
- El carrusel es manual (solo flechas y arrastre)
- No hay loop infinito

---

#### **Autoplay Delay**
- **Rango**: 1000ms a 10000ms (1 a 10 segundos)
- **Por defecto**: 3000ms (3 segundos)
- Tiempo que espera antes de pasar al siguiente slide

**Recomendaciones:**
- **1000-2000ms**: Muy rápido (para contenido simple)
- **3000-4000ms**: Velocidad ideal ✅
- **5000-10000ms**: Lento (para leer mucho texto)

---

#### **Transition Speed**
- **Rango**: 200ms a 2000ms
- **Por defecto**: 600ms
- Velocidad de la animación al cambiar de slide

**Recomendaciones:**
- **200-400ms**: Transición rápida
- **500-700ms**: Velocidad ideal ✅
- **800-2000ms**: Transición lenta y suave

---

## 🎨 Ejemplos de Configuración

### Ejemplo 1: Carrusel Estático (Manual)

```
Carousel Title: Content Carousel
Show Navigation Arrows: ✓ Activado
Items per view: 5
Gap between items: 8px
Card Aspect Ratio: Portrait (2:3)
Card Max Width: 280px
Enable Autoplay: ✗ Desactivado
```

**Resultado:** Carrusel que solo se mueve con flechas o arrastre

---

### Ejemplo 2: Carrusel Infinito Lento (Ideal para mostrar testimonios)

```
Carousel Title: Lo que dicen de nosotros
Show Navigation Arrows: ✗ Desactivado
Items per view: 3
Gap between items: 12px
Card Aspect Ratio: Portrait (2:3)
Card Max Width: 320px
Enable Autoplay: ✓ Activado
Autoplay Delay: 5000ms (5 segundos)
Transition Speed: 800ms
```

**Resultado:** Carrusel que se mueve lento, da tiempo para leer

---

### Ejemplo 3: Carrusel Rápido Dinámico (Ideal para productos/fotos)

```
Carousel Title: Nuestros Productos
Show Navigation Arrows: ✓ Activado
Items per view: 4
Gap between items: 8px
Enable Autoplay: ✓ Activado
Autoplay Delay: 2500ms (2.5 segundos)
Transition Speed: 400ms
```

**Resultado:** Carrusel dinámico con transiciones rápidas, pero con flechas para control manual

---

### Ejemplo 4: Carrusel Compacto Sin Espacio

```
Carousel Title: Galería
Show Navigation Arrows: ✗ Desactivado
Items per view: 5
Gap between items: 0px
Enable Autoplay: ✓ Activado
Autoplay Delay: 3000ms
Transition Speed: 600ms
```

**Resultado:** Carrusel sin espacios entre items, totalmente automático

---

### Ejemplo 5: Galería de Logos (Square Format)

```
Carousel Title: Nuestras Marcas
Show Navigation Arrows: ✓ Activado
Items per view: 6
Gap between items: 16px
Card Aspect Ratio: Square (1:1)
Card Max Width: 200px
Enable Autoplay: ✗ Desactivado
```

**Resultado:** Grid de logos cuadrados, compacto y limpio

---

### Ejemplo 6: Banners Promocionales (Wide Format)

```
Carousel Title: Ofertas Especiales
Show Navigation Arrows: ✗ Desactivado
Items per view: 2
Gap between items: 8px
Card Aspect Ratio: Wide (16:9)
Card Max Width: 500px
Enable Autoplay: ✓ Activado
Autoplay Delay: 4000ms
Transition Speed: 500ms
```

**Resultado:** Banners panorámicos grandes con autoplay suave

---

## 💡 Tips y Mejores Prácticas

### ✅ DO (Hacer)

1. **Reduce el gap entre items a 0-8px** para un look más moderno
2. **Usa autoplay para contenido visual** (fotos, productos)
3. **Desactiva las flechas si usas autoplay** (menos distracción)
4. **Pausa automática funciona bien** - El mouse encima pausa el carrusel
5. **Ajusta el delay según el contenido**:
   - Contenido simple/visual: 2-3 segundos
   - Contenido con texto: 5-6 segundos
6. **Elige el aspect ratio correcto**:
   - Fotos de personas: Portrait (2:3)
   - Logos: Square (1:1)
   - Banners: Wide (16:9)
7. **Ajusta Card Max Width según Items per view**:
   - 6+ items: 200-240px
   - 4-5 items: 260-300px
   - 2-3 items: 320-400px

### ❌ DON'T (No hacer)

1. **No uses autoplay muy rápido (< 2 segundos)** - Marea al usuario
2. **No combines flechas grandes con autoplay** - Demasiadas opciones
3. **No pongas gap muy grande con autoplay** - Se ve entrecortado
4. **No uses transición muy lenta (> 1 segundo)** - Parece lento
5. **No actives autoplay si hay mucho texto** - No da tiempo de leer

---

## 🎯 Casos de Uso Recomendados

### **Galería de Fotos**
```
Gap: 0px
Autoplay: ✓ Activado
Delay: 3000ms
Speed: 600ms
Arrows: ✗ Desactivado
```

### **Testimonios / Reseñas**
```
Gap: 16px
Autoplay: ✓ Activado
Delay: 6000ms
Speed: 800ms
Arrows: ✓ Activado
```

### **Categorías de Producto**
```
Gap: 8px
Autoplay: ✗ Desactivado
Arrows: ✓ Activado
Items per view: 4-5
```

### **Lookbook / Inspiración**
```
Gap: 4px
Autoplay: ✓ Activado
Delay: 4000ms
Speed: 500ms
Arrows: ✗ Desactivado
```

---

## 🔧 Personalización Avanzada

### Comportamiento del Autoplay

El autoplay tiene estas características incorporadas:
- ✅ **Pausa al hacer hover** - Se detiene cuando pasas el mouse
- ✅ **Continúa al quitar el mouse** - Sigue cuando lo quitas
- ✅ **Loop infinito** - Vuelve al inicio cuando termina
- ✅ **No se desactiva al interactuar** - Sigue después de usar flechas

---

## 📊 Espaciado Recomendado por Dispositivo

El carrusel ajusta automáticamente el espaciado en diferentes pantallas:

**Mobile (< 768px):**
- Muestra 2 items
- Usa el gap configurado

**Tablet (768px - 1024px):**
- Muestra 3 items
- Usa el gap configurado

**Desktop (> 1024px):**
- Muestra el número configurado en "Items per view"
- Usa el gap configurado

---

## ✅ Checklist de Configuración

Antes de publicar, verifica:

- [ ] El título está correcto
- [ ] Agregaste las tarjetas de contenido (bloques)
- [ ] El espaciado (gap) se ve bien
- [ ] Si usas autoplay, el delay es apropiado para el contenido
- [ ] La velocidad de transición es suave
- [ ] Las flechas están activadas/desactivadas según necesites
- [ ] Se ve bien en mobile, tablet y desktop
- [ ] El carrusel no se ve muy rápido ni muy lento
- [ ] Guardaste los cambios

---

## 🆘 Solución de Problemas

### El carrusel no se mueve automáticamente

**Causa:** Autoplay no está activado

**Solución:**
1. Activa **Enable Autoplay** ☑️
2. Guarda y recarga la página

---

### El carrusel se mueve muy rápido

**Solución:**
- Aumenta el **Autoplay Delay** (ej: de 3000 a 5000ms)
- Aumenta el **Transition Speed** (ej: de 400 a 800ms)

---

### Las flechas no aparecen

**Causa:** Están desactivadas o solo hay 1 tarjeta

**Solución:**
1. Verifica que **Show Navigation Arrows** esté activado ☑️
2. Asegúrate de tener al menos 2 tarjetas

---

### Hay mucho espacio entre las tarjetas

**Solución:**
- Reduce el **Gap between items** a 0-8px

---

### El carrusel no se pausa al pasar el mouse

**Causa:** Esto es el comportamiento esperado cuando autoplay está activado

**Nota:** El carrusel SÍ se pausa automáticamente al hacer hover, esto está incorporado en el código

---

**Última actualización:** Noviembre 2025
**Versión:** 2.0
