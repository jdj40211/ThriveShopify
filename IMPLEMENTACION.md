# Guía de Implementación - Thrive Custom Theme

Esta guía te ayudará a implementar todas las nuevas secciones y funcionalidades del tema Thrive.

## 📋 Tabla de Contenidos

1. [Metafields de Producto](#1-metafields-de-producto)
2. [Secciones Creadas](#2-secciones-creadas)
3. [Páginas de Políticas](#3-páginas-de-políticas)
4. [Cómo Agregar Contenido](#4-cómo-agregar-contenido)
5. [Checklist de Implementación](#5-checklist-de-implementación)

---

## 1. Metafields de Producto

Antes de usar las secciones, debes crear los siguientes metafields en el admin de Shopify:

### Ruta: `Settings > Custom Data > Products > Add definition`

| Nombre | Namespace y Key | Tipo | Descripción |
|--------|----------------|------|-------------|
| Tipo de Tela | `custom.fabric_type` | Single line text | Tipo de tela (ej: "Algodón Pima") |
| GSM | `custom.fabric_gsm` | Integer | GSM de la tela (ej: 180) |
| Tacto | `custom.fabric_feel` | Single line text | Tacto del producto (ej: "Suave y transpirable") |
| Tipo de Estampado | `custom.print_type` | Single line text | Tipo de estampado (ej: "DTG", "Serigrafía") |
| Referencia del Modelo | `custom.model_reference` | Single line text | Ej: "El modelo mide 1.80m y usa talla M" |
| Instrucciones de Cuidado | `custom.care_instructions` | Multi-line text | Instrucciones específicas de lavado |
| Guías Relacionadas | `custom.related_guides` | List of page references | Enlaces a guías relacionadas |

### Cómo Crear un Metafield:

1. Ve a **Settings > Custom Data > Products**
2. Click en **Add definition**
3. Llena los campos:
   - **Name**: Nombre visible (ej: "Tipo de Tela")
   - **Namespace and key**: usa el formato `custom.fabric_type`
   - **Type**: Selecciona el tipo según la tabla
4. Click en **Save**

---

## 2. Secciones Creadas

### 2.1 Detalles del Producto (`product-details`)

**Ubicación**: `sections/product-details.liquid`

Muestra información técnica del producto:
- Tipo de tela y GSM
- Tipo de estampado
- Instrucciones de cuidado
- Guía de tallas
- Enlaces a guías relacionadas

**Cómo agregar a un producto:**
1. Ve a **Online Store > Themes > Customize**
2. Selecciona un template de producto
3. Click en **Add section** > **Detalles del Producto**
4. Configura los textos y enlaces

**Datos necesarios:**
- Completa los metafields del producto (fabric_type, fabric_gsm, print_type, etc.)
- Crea páginas para guías de tallas y cuidado
- Asigna esas páginas en la configuración de la sección

---

### 2.2 Guía de Tallas (`size-guide`)

**Ubicación**: `sections/size-guide.liquid`

Guía de tallas interactiva con tabs por tipo de producto.

**Cómo implementar:**

1. Crea una página: **Online Store > Pages > Add page**
   - Título: "Guía de Tallas"
   - Template: `page.json` o cualquier template de página

2. En el Theme Editor:
   - Click en **Add section** > **Guía de Tallas**
   - Agrega bloques de **Tabla de Tallas** para cada tipo de producto

3. Configura cada tabla:
   - **Tipo de producto**: Polos, Hoodies, Longsleeves, etc.
   - **Columnas**: Activa las medidas que necesites (Pecho, Largo, Manga, etc.)
   - **Medidas**: Ingresa valores separados por comas
     - Ejemplo: Para talla M con Pecho y Largo activos: `96, 72`
   - **Imagen de medidas**: Sube una imagen mostrando cómo medir

4. Opcional: Sube una imagen de referencia mostrando cómo tomar medidas

**Ejemplo de Datos:**

Para Polos (Pecho y Largo activos):
- Talla S: `92, 70`
- Talla M: `96, 72`
- Talla L: `100, 74`

---

### 2.3 Instrucciones de Lavado (`care-instructions`)

**Ubicación**: `sections/care-instructions.liquid`

Sección con instrucciones de cuidado y lavado.

**Tipos de bloques disponibles:**

1. **Instrucción de Cuidado**: Item individual con icono
   - Iconos disponibles: Lavado, Blanqueador, Secado, Planchado, Limpieza en seco, etc.

2. **Cuidado por Material**: Tarjeta destacada para instrucciones específicas de un material

3. **Advertencia**: Alertas importantes (fondo rojo)

4. **Consejo**: Tips útiles (fondo verde)

**Cómo implementar:**

1. Crea una página: "Instrucciones de Lavado"
2. Agrega la sección **Instrucciones de Lavado**
3. Agrega bloques según necesites:
   - Instrucciones generales (ej: "Lavar a máquina con agua fría")
   - Advertencias (ej: "No usar blanqueador")
   - Consejos (ej: "Lava del revés para mantener colores vibrantes")
4. Opcional: Sube una imagen con la guía de símbolos de lavado

---

### 2.4 Embajadores / Comunidad (`ambassadors`)

**Ubicación**: `sections/ambassadors.liquid`

Muestra a las personas que usan Thrive (embajadores, comunidad).

**Cómo implementar:**

1. Crea una página o agrégala a tu homepage
2. Agrega la sección **Embajadores / Comunidad**
3. Para cada embajador, agrega un bloque **Embajador**:
   - **Foto**: Sube la foto desde tu Drive primero a Shopify Files
   - **Nombre**: Nombre del embajador
   - **Rol**: Ej: "Embajador Thrive", "Atleta"
   - **Frase**: Testimonial o frase acerca de Thrive
     - Ej: "Lo crearlas", "Lo mejorarlas con ChatGPT"
   - **Instagram URL**: Link a su Instagram
   - **Enlace a producto**: Link al producto que usa
   - **Overlay**: Activa si quieres mostrar texto al hacer hover

4. Configura el CTA al final para invitar a más personas a aplicar

**Frases sugeridas:**
- "Lo crearlas"
- "Lo mejorarlas con ChatGPT"
- "Calidad que se siente"
- "Diseño que inspira"

---

### 2.5 FAQ's del Producto (`product-faq`)

**Ubicación**: `sections/product-faq.liquid`

Sección de preguntas frecuentes con tabs por categoría.

**Cómo implementar:**

1. Decide si quieres categorías:
   - **Con categorías**: Tabs por tipo de producto (Polos, Hoodies, Longsleeves)
   - **Sin categorías**: Lista simple de preguntas

2. **Con categorías:**
   - Agrega bloques de **Categoría** (ej: Polos, Hoodies)
   - Agrega bloques de **Pregunta**
   - En cada pregunta, ingresa el ID de la categoría en el campo "ID de Categoría"
     - El ID se encuentra en el panel izquierdo del Theme Editor

3. **Sin categorías:**
   - Simplemente agrega bloques de **Pregunta**
   - Deja el campo "ID de Categoría" en blanco

**Preguntas sugeridas por producto:**

**Polos:**
- ¿Cómo es el calce de los polos?
- ¿Los polos encogen al lavar?
- ¿Qué tipo de tela usan?
- ¿Son resistentes al desteñido?

**Hoodies:**
- ¿Los hoodies tienen bolsillo canguro?
- ¿Vienen con capucha ajustable?
- ¿Cuál es el grosor de la tela?
- ¿Son buenos para clima frío?

**Longsleeves:**
- ¿Las mangas son largas?
- ¿El calce es ajustado o suelto?
- ¿Se pueden usar para hacer ejercicio?

---

### 2.6 Página de Políticas (`policy-page`)

**Ubicación**: `sections/policy-page.liquid`, `templates/page.policy.json`

Template para páginas de políticas con barra lateral de navegación.

**Cómo implementar:**

1. **Crea las páginas de políticas:**
   - Ve a **Online Store > Pages**
   - Crea 3 páginas:
     - "Política de Devoluciones"
     - "Política de Envíos"
     - "Política de Cambios"

2. **Asigna el template:**
   - Para cada página, en el panel derecho selecciona:
   - **Theme template**: `page.policy`

3. **Configura la sección:**
   - Ve al Theme Editor > selecciona una de las páginas de políticas
   - En la sección "Página de Políticas":
     - Agrega bloques **Enlace a Política** para cada página
     - Selecciona la página correspondiente en cada bloque
   - Configura la tarjeta de contacto (opcional)

4. **Escribe el contenido:**
   - Edita cada página y escribe el contenido de la política
   - Usa formato Markdown:
     - `## Título Grande`
     - `### Subtítulo`
     - `**Negrita**`
     - Listas con `-` o `1.`

---

## 3. Páginas de Políticas

### 3.1 Contenido Sugerido

#### Política de Devoluciones

```markdown
## Política de Devoluciones

Aceptamos devoluciones dentro de los 30 días posteriores a la recepción de tu pedido.

### Condiciones para Devoluciones

- El producto debe estar sin usar y con etiquetas
- Debe estar en su empaque original
- Debes proporcionar el comprobante de compra

### Cómo solicitar una devolución

1. Contáctanos a través de [email]
2. Proporciona tu número de orden
3. Indica el motivo de la devolución
4. Te enviaremos las instrucciones

### Reembolsos

Los reembolsos se procesarán dentro de 5-7 días hábiles después de recibir el producto.

### Excepciones

No aceptamos devoluciones de:
- Productos personalizados
- Productos en promoción final
```

#### Política de Envíos

```markdown
## Política de Envíos

### Tiempos de Entrega

- Envío nacional: 3-5 días hábiles
- Envío internacional: 7-15 días hábiles

### Costos de Envío

- Envío gratis en compras superiores a $X
- Costo estándar: $X

### Seguimiento

Recibirás un número de seguimiento una vez que tu pedido sea despachado.
```

#### Política de Cambios

```markdown
## Política de Cambios

Ofrecemos cambios por talla o producto diferente dentro de los 30 días.

### Proceso de Cambio

1. Contáctanos
2. Empaca el producto
3. Envíalo a nuestra dirección
4. Te enviaremos el nuevo producto

El cambio está sujeto a disponibilidad de inventario.
```

---

## 4. Cómo Agregar Contenido

### 4.1 Subir Fotos desde Drive

**No puedes subir directamente desde Drive a Shopify.** Debes:

1. Descarga las fotos de Drive a tu computadora
2. Ve a **Settings > Files** en Shopify
3. Click en **Upload files**
4. Sube las fotos
5. Usa esas fotos en las secciones del tema

**Organización recomendada:**

- Carpeta "Embajadores" para fotos de comunidad
- Carpeta "Productos" para fotos de producto
- Carpeta "Guias" para imágenes de guías (tallas, lavado)

### 4.2 Crear Páginas Nuevas

1. **Online Store > Pages > Add page**
2. Título: (nombre de la página)
3. Content: Escribe el contenido
4. Template: Selecciona el template apropiado
5. **Save**

### 4.3 Agregar Secciones a Templates

**Para productos:**
1. Theme Editor > Products > Default product
2. **Add section** > (elige la sección)
3. Arrastra la sección donde quieras que aparezca

**Para páginas:**
1. Theme Editor > Pages > (elige la página)
2. **Add section** > (elige la sección)

**Para homepage:**
1. Theme Editor > Home
2. **Add section** > (elige la sección)

---

## 5. Checklist de Implementación

### ✅ Configuración Inicial

- [ ] Crear todos los metafields de producto
- [ ] Subir fotos desde Drive a Shopify Files
- [ ] Crear páginas necesarias (Guía de Tallas, Instrucciones de Lavado, Políticas)

### ✅ Metafields de Productos

Para cada producto, completa:
- [ ] Tipo de Tela
- [ ] GSM
- [ ] Tacto
- [ ] Tipo de Estampado
- [ ] Referencia del Modelo
- [ ] Instrucciones de Cuidado específicas

### ✅ Página de Guía de Tallas

- [ ] Crear página "Guía de Tallas"
- [ ] Agregar sección Size Guide
- [ ] Crear tabla para Polos
- [ ] Crear tabla para Hoodies
- [ ] Crear tabla para Longsleeves
- [ ] Subir imágenes de cómo medir
- [ ] Agregar referencia del modelo

### ✅ Página de Instrucciones de Lavado

- [ ] Crear página "Instrucciones de Lavado"
- [ ] Agregar sección Care Instructions
- [ ] Agregar instrucciones generales
- [ ] Agregar instrucciones por material
- [ ] Agregar advertencias
- [ ] Agregar consejos
- [ ] Subir imagen de símbolos de lavado

### ✅ Sección de Embajadores

- [ ] Decidir dónde ubicarla (home o página dedicada)
- [ ] Agregar sección Ambassadors
- [ ] Agregar fotos y datos de embajadores
- [ ] Agregar frases acerca de Thrive
- [ ] Configurar enlaces a Instagram
- [ ] Configurar CTA para aplicar

### ✅ FAQ's por Producto

- [ ] Decidir estructura (con o sin categorías)
- [ ] Agregar sección Product FAQ
- [ ] Crear preguntas para Polos
- [ ] Crear preguntas para Hoodies
- [ ] Crear preguntas para Longsleeves
- [ ] Configurar CTA de contacto

### ✅ Páginas de Políticas

- [ ] Crear página "Política de Devoluciones"
- [ ] Crear página "Política de Envíos"
- [ ] Crear página "Política de Cambios"
- [ ] Asignar template `page.policy` a cada una
- [ ] Escribir contenido de cada política
- [ ] Configurar enlaces en la barra lateral
- [ ] Configurar tarjeta de contacto

### ✅ Sección en Productos

- [ ] Agregar "Detalles del Producto" al template de producto
- [ ] Configurar enlaces a guías (tallas, cuidado)
- [ ] Verificar que los metafields se muestren correctamente

### ✅ Enlaces y Navegación

- [ ] Agregar enlace a Guía de Tallas en el menú
- [ ] Agregar enlace a Políticas en el footer
- [ ] Agregar enlace a página de Embajadores (si aplica)
- [ ] Verificar que todos los enlaces funcionen

---

## 📝 Notas Finales

### Prioridad de Implementación

**Alta prioridad (hacerlo primero):**
1. Metafields de producto
2. Guía de Tallas
3. Detalles del Producto en templates
4. Políticas

**Media prioridad:**
5. Instrucciones de Lavado
6. FAQ's

**Baja prioridad (cuando tengas contenido):**
7. Embajadores / Comunidad

### Contenido que Necesitas Preparar

1. **Fotos:**
   - Fotos de embajadores/comunidad
   - Fotos de productos en uso
   - Imágenes de guía de medidas

2. **Textos:**
   - Frases de embajadores acerca de Thrive
   - Descripciones de productos
   - Contenido de políticas
   - Preguntas frecuentes

3. **Datos Técnicos:**
   - Medidas de cada talla (tabla completa)
   - Tipos de tela y GSM
   - Tipos de estampado
   - Instrucciones de lavado por tipo de producto

### Soporte

Si tienes problemas con la implementación:
1. Revisa que todos los metafields estén creados correctamente
2. Verifica que los nombres y keys sean exactos
3. Asegúrate de que las fotos estén subidas a Shopify Files
4. Revisa la consola del navegador para errores

---

## 🎉 ¡Todo Listo!

Ahora tienes todas las herramientas para completar el contenido de tu sitio Thrive. Ve paso a paso usando el checklist y pronto tendrás un sitio completo y profesional.
