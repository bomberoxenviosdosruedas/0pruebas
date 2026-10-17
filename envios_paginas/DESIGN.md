# Sistema de Diseño: Envíos DosRuedas (Mar del Plata)
**Identificador del Proyecto:** `envios-dosruedas-mdq`  
**Referencia Técnica:** [home_clean.html](file:///C:/Users/prest/proyectos/0pruebas/envios_paginas/home_clean.html) · [servicios_clean.html](file:///C:/Users/prest/proyectos/0pruebas/envios_paginas/servicios_clean.html) · [enviosflex_clean.html](file:///C:/Users/prest/proyectos/0pruebas/envios_paginas/enviosflex_clean.html) · [envios_lowcost_clean.html](file:///C:/Users/prest/proyectos/0pruebas/envios_paginas/envios_lowcost_clean.html) · [envios_express_clean.html](file:///C:/Users/prest/proyectos/0pruebas/envios_paginas/envios_express_clean.html) · [deposito_fulfillment_clean.html](file:///C:/Users/prest/proyectos/0pruebas/envios_paginas/deposito_fulfillment_clean.html) · [cotizar_clean.html](file:///C:/Users/prest/proyectos/0pruebas/envios_paginas/cotizar_clean.html) · [contacto_clean.html](file:///C:/Users/prest/proyectos/0pruebas/envios_paginas/contacto_clean.html) · [sobre_nosotros_clean.html](file:///C:/Users/prest/proyectos/0pruebas/envios_paginas/sobre_nosotros_clean.html) · [preguntas_frecuentes_clean.html](file:///C:/Users/prest/proyectos/0pruebas/envios_paginas/preguntas_frecuentes_clean.html) · [nuestras_redes_clean.html](file:///C:/Users/prest/proyectos/0pruebas/envios_paginas/nuestras_redes_clean.html) · [SECCIONES.md](file:///C:/Users/prest/proyectos/0pruebas/envios_paginas/SECCIONES.md)  
**Entorno Operativo:** Logística e-commerce urbana, mensajería en moto, envíos en el día y cadetería inteligente en Mar del Plata.

---

## 1. Atmósfera Visual y Filosofía de Diseño
La interfaz proyecta la energía vibrante, ágil y de alta confiabilidad de un servicio logístico de última milla propio en las calles de Mar del Plata. Es una estética **Brutalista Deportiva / Urban Utilitarian**, donde la velocidad y la puntualidad se comunican mediante:
- **Contraste de Alto Impacto:** Diálogo constante entre un Azul Eléctrico Ultramar y un Amarillo Fluorescente de Alta Visibilidad, evocando chalecos reflectivos, asfalto y dinamismo en ruta.
- **Tipografía Monumental Condensada:** Títulos en caja alta que transmiten solidez física y compromiso innegociable, combinados con micro-copys en tipografía monoespaciada que recuerdan remitos y telemetría de ruteo.
- **Geometría Híbrida Orgánica:** Botones en píldora suavemente redondeados contrastados con tarjetas modulares tipo visor digital (*app cards*) con radios amplios de hasta 36px y micro-rotaciones lúdicas de 1° a 2° que rompen la rigidez del lienzo tradicional.
- **Micro-movimiento y Telemetría:** Marquesinas continuas (*tickers*), radares con pulsos interactivos y tarjetas elevadas mediante sombras profundas tintadas al azul.

---

## 2. Paleta de Colores Calibrada (Tokens Semánticos)

Todos los colores están calibrados para mantener coherencia estricta sin fluctuación térmica:

### 2.1. Colores Primarios y de Fondo
* **Azul Eléctrico Ultramar (`#0950f6` / `brand.blue`):**  
  *Rol Funcional:* Color de identidad central de la marca. Fondo de secciones troncales (Hero, Catálogo, Footer), texto principal sobre superficies blancas y bordes interactivos destacados.
* **Azul Noche Profundo (`#063dc2` / `brand.blue-dark`):**  
  *Rol Funcional:* Superficie de contraste en subcontenedores oscuros, fondos de tarjetas dentro de secciones azules, estados hover de elementos primarios y fondo del drawer móvil.
* **Blanco Señal Puro (`#ffffff`):**  
  *Rol Funcional:* Fondo de lienzo limpio para secciones de servicios y testimonios, relleno de tarjetas elevadas y texto de alto contraste sobre fondos oscuros.

### 2.2. Acentos y Alta Visibilidad
* **Amarillo Tránsito / Racing Yellow (`#ffec01` / `brand.yellow`):**  
  *Rol Funcional:* Acento primario de máxima jerarquía. Botones de acción clave (*Call to Action* "Cotizá tu envío"), badges de flota propia, rotulaciones inclinadas en titulares, estrellas de calificación y acentos de radar.
* **Amarillo Luminoso Hover (`#fff240` / `brand.yellow-hover`):**  
  *Rol Funcional:* Estado activo e interacción hover sobre botones y enlaces de acento amarillo.
* **Crema Sutil Acaramelado (`#fffde6` / `brand.yellow-light`):**  
  *Rol Funcional:* Fondo sutil para tarjetas destacadas (como MercadoLibre Flex) y cápsulas de estado secundario.

### 2.3. Tonos de Apoyo y Superficies Tenues
* **Azul Glaciar Tenue (`#f3f7ff` / `brand.blue-subtle`):**  
  *Rol Funcional:* Relleno de campos de formulario (inputs), cápsulas de métricas técnicas internas y fondos de tarjetas de baja jerarquía.
* **Azul Hielo Claro (`#e8f0fe` / `brand.blue-light`):**  
  *Rol Funcional:* Bordes sutiles de tarjetas sobre fondo blanco y badges informativos de paquetería estándar.

### 2.4. Transparencias y Vidrio Arquitectónico (Glassmorphism)
* **Borde Sutil Translúcido (`rgba(255, 255, 255, 0.15)`):** Líneas divisoras y marcos de 1px sobre superficies azules.
* **Velo Glassmorphic (`rgba(9, 80, 246, 0.95)` con `backdrop-blur-md`):** Barra de navegación fija y paneles flotantes.
* **Tinte Divisor Claro (`rgba(9, 80, 246, 0.10)`):** Bordes separadores sobre fondo blanco puro.

---

## 3. Arquitectura Tipográfica

El sistema utiliza tres familias complementarias que diferencian jerarquía narrativa, lectura funcional y telemetría de datos:

| Rol | Familia | Pesos Utilizados | Transformación / Tracking | Aplicación |
| :--- | :--- | :--- | :--- | :--- |
| **Display / Titulares** | `Anton`, `Impact`, `sans-serif` | 400 (Heavy) | `uppercase`, `tracking-tight`, `leading-[0.92]` a `leading-none` | H1, H2, H3, llamadas de atención, marcas y CTAs principales |
| **Interfaz / Lectura** | `Outfit`, `sans-serif` | 400 (Regular), 500 (Medium), 600 (Semibold), 700 (Bold) | `normal`, `tracking-normal`, `leading-relaxed` | Párrafos descriptivos, etiquetas de formulario, navegación, testimonios |
| **Telemetría / Datos** | `Geist Mono`, `monospace` | 500, 600, 700 | `uppercase`, `tracking-wider`, `text-[10px]` a `text-xs` | Horarios de corte, insignias operativas, tramos en KM, coordenadas, metadatos |
| **Iconografía** | `Material Symbols Outlined` | 400, con `FILL 1` para estrellas | Inline simétrico alineado verticalmente | Indicadores de servicio, flechas, teléfonos, pines de radar |

---

## 4. Estilo y Comportamiento de Componentes

### 4.1. Botones de Acción (CTAs)
* **Primario ("Cotizá tu envío"):** Forma de píldora completa (`rounded-full`), relleno en Amarillo Tránsito (`#ffec01`), texto en Azul Eléctrico (`#0950f6`), tipografía `Anton` en mayúsculas, tamaño mediano/grande (`px-8 py-3.5`), flecha hacia la derecha con desplazamiento reactivo al hover (`group-hover:translate-x-1 transition-transform`).
* **Secundario ("Ver servicios"):** Forma de píldora (`rounded-full`), contorno fino o texto blanco con hover hacia el Amarillo Tránsito, acompañado de flecha direccional.
* **Acciones en Tarjetas:** Botón ancho completo (`w-full`), altura compacta (`py-2.5` a `py-3`), fuente display o semibold, con icono `arrow_forward` al extremo derecho.

### 4.2. Tarjetas y Fichas de Producto / Servicio
* **Forma y Bordes:** Esquinas generosamente redondeadas (`rounded-3xl` de 24px hasta `rounded-[36px]` de 36px) que simulan la estética física de terminales móviles y teléfonos de reparto.
* **Borde Físico Distintivo:** Marco sólido de 4px (`border-4`) en blanco o amarillo que recorta la tarjeta con nitidez sobre fondos saturados.
* **Elevación e Iluminación (`card-phone-shadow`):**  
  `box-shadow: 0 30px 60px -12px rgba(0, 20, 100, 0.45), 0 0 0 1px rgba(255, 255, 255, 0.15);`  
  Una sombra profunda tintada al azul que otorga peso y presencia tridimensional flotante.
* **Métrica en 3 Columnas:** Grilla interna compacta (`grid-cols-3`) con celdas redondeadas (`rounded-2xl`) en fondo suave para destacar: `TRAMO`, `VENTANA`, `PESO` o `CORTE`, `ENTREGA`, `TARIFA`.

### 4.3. Insignias e Indicadores de Estado (Badges)
* **Insignia Operativa Clásica:** Píldora (`rounded-full`) en `font-mono text-xs font-bold uppercase` con icono de rayo (`⚡`), punto de radar activo o check.
* **Rótulos de Título Inclinados:** Caja contenedora en Amarillo Tránsito con leve rotación negativa (`-rotate-1`) colocada directamente sobre palabras clave del encabezado ("ÚLTIMA MILLA", "VENDEN Y ENVÍAN").

### 4.4. Formularios y Captura de Leads
* **Inputs y Selects:** Esquinas suavizadas (`rounded-xl`), fondo blanco o azul tenue (`#f3f7ff`), borde fino de 1px (`border-brand-blue/20`), iconos identificadores en el flanco izquierdo (persona, tienda, paquete), foco limpio en azul corporativo sin halos exagerados.
* **Etiquetas:** Situadas arriba del campo, en `font-mono text-xs font-bold uppercase tracking-wider`.

### 4.5. Marquesinas y Tickers de Diferenciales
* **Estructura:** Doble marquesina continua infinita (`animate-marquee` y `animate-marquee-reverse`) con pausa accesible en `hover` o vía botón conmutable.
* **Separadores Tipográficos:** Rombo sólido (`◆`) o estrella de cuatro puntas (`✦`) en Amarillo Tránsito entre lemas.

---

## 5. Principios de Maquetación y Grilla

1. **Ritmo Vertical por Bloques de Alto Contraste:**  
   Alternancia estratégica de bloques:  
   `Azul Eléctrico (#0950f6)` → `Blanco Puro (#ffffff)` → `Azul Eléctrico (#0950f6)` → `Blanco Puro (#ffffff)`.  
   Esta alternancia mantiene la vigilia visual y evita la fatiga de lectura.
2. **Contenedor Maestro:**  
   Ancho máximo estándar de `max-w-7xl` (1280px) con relleno horizontal responsivo `px-4 lg:px-8`. Los formularios de cotización se concentran en `max-w-6xl` para enfocar la conversión.
3. **Composición Asimétrica del Hero:**  
   Columna izquierda (7 columnas en desktop) reservada a la narrativa monumental y botones de acción; columna derecha (5 columnas) dedicada a la interfaz de telemetría y mapa isométrico con radar activo.
4. **Bento Grid para Soluciones Empresariales:**  
   Distribución asimétrica 7:5 combinando un módulo amplio de Cuenta Corriente con dos tarjetas apiladas de alta jerarquía (Flex y Corporativo).
5. **Comportamiento Móvil (< 768px):**  
   - Todas las grillas colapsan estrictamente a 1 columna.  
   - Los carruseles permiten deslizamiento horizontal nativo táctil (`overflow-x-auto` con `scroll-smooth`).  
   - La cabecera despliega un menú lateral *Drawer* accesible (`#mobile-drawer`) con cierre por botón o backdrop.

---

## 6. Bloque de Instrucciones de Diseño para Generación en Stitch (Requerido)

> Copiar este bloque completo en la sección de diseño de cualquier prompt de Stitch o en `.stitch/next-prompt.md`:

```markdown
**DESIGN SYSTEM (REQUIRED - ENVIOS DOSRUEDAS MAR DEL PLATA):**
- **Atmosphere:** Urban high-speed logistics and e-commerce delivery interface. Confident, brutalist-athletic, utilitarian, clean, ultra-reliable. Strong contrast between Royal Blue and Racing Yellow.
- **Color Palette:**
  - Primary Brand Blue: #0950f6 (Hero backgrounds, primary headers, high-contrast borders)
  - Deep Navy Blue: #063dc2 (Hover states, deep card surfaces, mobile drawer)
  - Crisp Canvas White: #ffffff (Page surfaces, light section backgrounds, elevated card containers)
  - Signal Racing Yellow: #ffec01 (Primary CTAs, active status badges, highlight tags, stars)
  - Subtle Blue Tint: #f3f7ff (Form fields, metric boxes, subtle card backgrounds)
  - Soft Ice Blue: #e8f0fe (Card borders, secondary badges)
- **Typography:**
  - Display & Big Titles: 'Anton', 'Impact', sans-serif (UPPERCASE, tracking-tight, leading-[0.92], bold impact)
  - Body & User Interface: 'Outfit', sans-serif (Clean geometric sans, leading-relaxed, weights 400/600/700)
  - Technical / Telemetry / Labels: 'Geist Mono', monospace (UPPERCASE, tracking-wider, text-xs, cut-off hours, KM, stats)
  - Icons: Google Material Symbols Outlined
- **Component Geometry & Radii:**
  - Buttons & Badges: Pill-shaped (rounded-full). Primary buttons have #ffec01 background with #0950f6 Anton text and an arrow icon.
  - Feature Cards: Phone-like heavily rounded corners (rounded-3xl or rounded-[36px]), 4px borders (border-4 border-white or border-brand-yellow), and deep blue shadows: box-shadow 0 30px 60px -12px rgba(0,20,100,0.45).
  - Tilted Tags: Inline title badges with slight rotation (-rotate-1 or rotate-1) on yellow backgrounds.
  - Form Inputs: Rounded-xl, background #ffffff or #f3f7ff, 1px subtle blue border, icons inside left.
- **Layout Architecture:**
  - Alternating full-width section blocks: High-contrast Electric Blue sections alternating with pure White sections.
  - Containment: Centered max-w-7xl with px-4 lg:px-8.
  - Responsive: Single column stack on mobile (<768px), horizontal smooth carousels with visible pagination dots.
- **Banned AI Patterns:** No generic purple/neon gradients, no generic Inter font, no centered bland hero layouts, no emojis, no fake round stats.
```

---

## 7. Anti-Patrones y Reglas de Exclusión (Lo que NUNCA debe hacerse)

* ❌ **Prohibido el uso de la tipografía `Inter` o fuentes Serif genéricas:** Solo está permitido el trío `Anton` + `Outfit` + `Geist Mono`.
* ❌ **Prohibidos los degradados fluorescentes violáceos o cian ("AI Neon Gradients"):** La paleta se basa en colores planos y contundentes (`#0950f6` y `#ffec01`).
* ❌ **Prohibido el uso de Negro Puro (`#000000`):** Toda la oscuridad y contraste profundo se resuelve mediante Azul Noche (`#063dc2`) o Azul Eléctrico (`#0950f6`).
* ❌ **Prohibidos los emojis como iconos:** Emplear exclusivamente glifos vectoriales de `Material Symbols Outlined`.
* ❌ **Prohibidas las tarjetas con esquinas angulosas o genéricas:** Todo contenedor principal debe respetar los radios suaves (`rounded-2xl`, `rounded-3xl` o `rounded-[36px]`).
* ❌ **Prohibida la invención de estadísticas vacías:** Nunca colocar métricas inventadas tipo "99.9% Uptime" o "5000+ horas"; utilizar datos y garantías reales del servicio local (Base Friuli 1972, corte 15:00 hs, franjas de 3 hs, flota propia).
