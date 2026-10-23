---
name: envios-dosruedas-mdq
description: Sistema de diseño de alta velocidad para logística urbana, mensajería en moto y e-commerce en Mar del Plata.
colors:
  primary: "#0950f6"
  primary_dark: "#0950f6"
  accent: "#ffec01"
  accent_hover: "#fff240"
  accent_light: "#fffde6"
  surface: "#ffffff"
  surface_subtle: "#f0f5ff"
  surface_ice: "#e0ebff"
  text_primary: "#0950f6"
  text_on_primary: "#ffffff"
  text_on_accent: "#0950f6"
typography:
  display: "Anton, Impact, sans-serif"
  body: "Outfit, sans-serif"
  code: "Geist Mono, monospace"
---

# Design System: Envios DosRuedas (Mar del Plata)
**Project ID:** `envios-dosruedas-mdq`  
**Entorno Operativo:** Logística urbana de última milla, paquetería e-commerce, mensajería en moto y fulfillment en Mar del Plata.  
**Ubicación Base:** Friuli 1972, Mar del Plata, Buenos Aires, Argentina.  
**Archivos Fuente de Referencia:**  
1. `home_clean.html` (Home Principal y Radar Logístico)  
2. `contacto_clean.html` (Contacto Comercial y Canales de Atención Directa)  
3. `cotizar_clean.html` (Cotizador Interactivo con Mapa y Distancia Lineal)  
4. `deposito_fulfillment_clean.html` (Almacenamiento, Racks y Despacho)  
5. `empresas_cuenta_corriente_clean.html` (Servicios Corporativos B2B y Facturación Quincenal)  
6. `enviosflex_clean.html` (Mercado Envíos Flex "Llega Hoy" con Corte 15:00 hs)  
7. `envios_contrareembolso_clean.html` (Cobro en Destino, Rendición en 24 hs y Cero Comisión)  
8. `envios_express_clean.html` (Envíos de Urgencia en Franja de 3 hs)  
9. `envios_lowcost_clean.html` (Envíos Económicos en el Día hasta las 19:00 hs)  
10. `nuestras_redes_clean.html` (Comunidad, Flota y Canales Digitales)  
11. `preguntas_frecuentes_clean.html` (Centro de Ayuda, Tarifas y Preguntas Operativas)  
12. `servicios_clean.html` (Hub Integral de Servicios Logísticos)  
13. `sobre_nosotros_clean.html` (Trayectoria, Base Friuli y Flota Homogénea)  

---

## 1. Visual Theme & Atmosphere (Atmósfera Visual y Filosofía)

Envios DosRuedas encarna una estética **Brutalista Deportiva y Utilitaria Urbana**. Proyecta velocidad inmediata, rigor operativo y máxima confiabilidad en la logística de última milla en Mar del Plata.

El diseño se inspira directamente en la **señalética vial reflectiva**, la indumentaria de alta visibilidad para motociclistas urbanos y la precisión milimétrica de la telemetría satelital de ruteo. A diferencia de las interfaces corporativas genéricas basadas en grises o fondos oscuros pesados, la experiencia se construye sobre un contraste frontal y enérgico:
- **Azul Corporativo Ultramar (`#0950F6`)** como fondo de máxima autoridad y techo absoluto de oscuridad.
- **Amarillo Vial Reflectivo (`#FFEC01`)** como acento de alta visibilidad para llamados a la acción, alertas operativas y estados activos.
- **Blanco Señal Puro (`#FFFFFF`)** como lienzo luminoso, aportando claridad, limpieza y respiración a los bloques de contenido.

La sensación espacial es ágil, transparente y moderna. La profundidad y jerarquía no se construyen con sombras oscuras ni degradados artificiales, sino mediante **capas translúcidas tipo glassmorphism**, marcos perimetrales definidos y tarjetas ergonómicas con bordes generosamente redondeados que evocan la forma de los dispositivos móviles de los cadetes de reparto.

---

## 2. Color Palette & Roles (Paleta de Colores y Roles Semánticos)

El sistema cromático implementa estrictamente el **ADR 02 (Ley de Tres Colores de Marca)**: **el Azul `#0950F6` es el techo máximo de oscuridad de toda la aplicación**. Queda formalmente prohibido el uso de negros puros (`#000000`), grises neutros (`gray`, `slate`, `zinc`) o azules noche (`#041F5E`, `blue-900`, `blue-950`).

### 2.1. Base Primaria y Superficies
* **Azul Corporativo Ultramar (`#0950F6` / `brand-blue-500`):**  
  *Rol Funcional:* Identidad institucional principal y tope de oscuridad absoluta. Utilizado en hero sections, cabeceras, marquesinas de telemetría, banners de aviso y pie de página corporativo.
* **Blanco Señal Puro (`#FFFFFF`):**  
  *Rol Funcional:* Lienzo principal para secciones de lectura, tarjetas elevadas, cajas de formulario y tipografía de alto contraste sobre fondos azules.

### 2.2. Acentos y Alta Visibilidad (Máximo 15% del Área Visual)
* **Amarillo Vial Reflectivo (`#FFEC01` / `brand-yellow-500`):**  
  *Rol Funcional:* Botones de acción primaria (CTAs como "Cotizá tu envío" o "Escribinos por WhatsApp"), badges de estado, tags destacados con rotación (-rotate-1), estrellas de calificación 5.0 y pines de origen en mapas.
* **Amarillo Luminoso Hover (`#FFF240` / `brand-yellow-400`):**  
  *Rol Funcional:* Estado hover y foco reactivo para controles interactivos principales.
* **Amarillo Sutil Acaramelado (`#FFFDE6` / `brand-yellow-50`):**  
  *Rol Funcional:* Superficie tenue para pastillas informativas de Mercado Envíos Flex y alertas operativas destacadas.

### 2.3. Superficies Claras y Graduación Luminosa
* **Azul Glaciar Tenue (`#F0F5FF` / `#F3F7FF` / `brand-blue-50`):**  
  *Rol Funcional:* Fondo de inputs, selects, tarjetas secundarias y contenedores de métricas sobre fondo blanco.
* **Azul Hielo Claro (`#E0EBFF` / `#E8F0FE` / `brand-blue-100`):**  
  *Rol Funcional:* Bordes perimetrales sutiles y pastillas de metadatos operativos en tarjetas claras.

### 2.4. Construcción de Profundidad sin Azules Oscuros (Técnica de Capas Translúcidas)
Para jerarquizar elementos dentro de bloques con fondo azul (`#0950F6`), se utilizan capas translúcidas:
* **Módulos sobre Azul:** `bg-brand-blue-500` con `border border-white/10` o `border border-white/20`, o velos sutiles `bg-white/10` con `backdrop-blur-md`.
* **Divisores sobre Azul:** `border-white/10` y `border-white/15` para grillas y separadores.
* **Textos sobre Azul:** Blanco puro (`#FFFFFF`) para titulares y cifras clave; blanco atenuado al 80-85% (`text-white/80`) para párrafos descriptivos.
* **Textos sobre Blanco:** Azul corporativo (`#0950F6`) para títulos y etiquetas; azul con opacidad (`text-brand-blue/70` a `text-brand-blue/80`) para textos secundarios, preservando la identidad sin recurrir a grises neutros.

---

## 3. Typography Rules (Arquitectura Tipográfica)

El sistema tipográfico combina tres familias según su función semántica:

| Rol Semántico | Familia Tipográfica | Pesos Empleados | Transformación y Tracking | Aplicación en Interfaz |
| :--- | :--- | :--- | :--- | :--- |
| **Titulares Monumentales (Display)** | `Anton`, `Impact`, `sans-serif` | 400 (Heavy) | `uppercase`, `tracking-tight`, `leading-[0.92]` a `leading-none` | H1 principales, títulos de secciones H2/H3, cifras de métricas, tickers y texto de botones principales |
| **Cuerpo y Lectura (Interface)** | `Outfit`, `sans-serif` | 400, 500, 600, 700 | `normal`, `tracking-normal`, `leading-relaxed` | Párrafos narrativos, preguntas frecuentes, descripciones de servicio, campos de formulario y navegación |
| **Telemetría y Datos (Technical Mono)** | `Geist Mono`, `monospace` | 500, 600, 700 | `uppercase`, `tracking-wider`, `text-xs` o `text-[10px]` | Horarios de corte (15:00 hs, 13:00 hs), distancias en km, etiquetas técnicas, tarifas y remitos |
| **Iconografía Vectorial** | `Material Symbols Outlined` | 400 (`FILL 1` en acentos) | Inline alineado | Transporte, flechas reactivas, checks de verificación, teléfonos y pines |

---

## 4. Component Stylings (Estilo y Comportamiento de Componentes)

### 4.1. Botones de Acción (CTAs)
* **Botón Primario ("Cotizá tu envío" / "Solicitar servicio"):**
  - **Forma:** Píldora redondeada completa (`rounded-full`).
  - **Fondo:** Amarillo Vial (`#FFEC01`) con transición a Amarillo Luminoso (`#FFF240`) en hover.
  - **Tipografía:** Azul Corporativo (`#0950F6`), fuente `Anton`, mayúsculas sostenidas, `tracking-wider`.
  - **Icono Reactivo:** Flecha hacia la derecha (`arrow_forward`) con desplazamiento dinámico en hover (`group-hover:translate-x-1.5 transition-transform duration-200`).
* **Botón Secundario Transparente / Reversa:**
  - **Forma:** Píldora (`rounded-full`).
  - **Fondo:** Translúcido con borde perimetral blanco (`border-2 border-white`) sobre fondo azul, o borde azul (`border-2 border-brand-blue`) sobre fondo blanco.
  - **Hover:** Relleno Amarillo Vial (`#FFEC01`) con texto en Azul Corporativo.
* **Botón Flotante de WhatsApp:**
  - Acceso directo persistente en la esquina inferior con enlace directo hacia `https://wa.me/549223...` con mensaje predeterminado contextual.

### 4.2. Tarjetas y Contenedores (Phone-Like Cards)
* **Geometría Ergonómica:** Bordes generosamente redondeados (`rounded-2xl`, `rounded-3xl` o `rounded-[36px]`), emulando la ergonomía de terminales móviles y teléfonos de reparto.
* **Bordes Perimetrales de Alto Impacto:** Marcos nítidos de 4px (`border-4 border-white` sobre azul, o `border-4 border-brand-yellow` en tarjetas destacadas).
* **Sombra de Profundidad Azul:** Elevación mediante sombras azules profundas (`box-shadow: 0 30px 60px -12px rgba(0, 20, 100, 0.45)`), evitando sombras negras sucias.

### 4.3. Inputs y Formularios
* **Contenedor:** Bordes suaves (`rounded-xl` / `rounded-2xl`).
* **Fondo:** Blanco Puro o Azul Glaciar Tenue (`#F0F5FF`).
* **Borde:** 1px sutil en Azul Hielo (`#E0EBFF` o `rgba(9, 80, 246, 0.2)`).
* **Estado de Foco:** Anillo nítido en Azul Corporativo (`#0950F6`) con elevación de contraste.

### 4.4. Rótulos y Badges Inclinados (Tilted Badges)
* **Efecto Dinámico:** Rótulos en línea con leve inclinación angular (`-rotate-1` o `rotate-1`).
* **Fondo:** Amarillo Vial (`#FFEC01`) con tipografía `Anton` en Azul Corporativo, aportando tensión visual deportiva.

---

## 5. Layout Principles (Principios de Disposición y Espaciado)

* **Estructura Alternante:** Bloques de sección de Azul Eléctrico (`#0950F6`) que alternan dinámicamente con secciones de Blanco Puro (`#FFFFFF`), manteniendo el ritmo visual.
* **Ancho Máximo:** Contenedor central acotado a `1440px` (`max-w-7xl`) con márgenes laterales adaptables (`px-4 sm:px-6 lg:px-8`).
* **Grilla y Espaciado Base:** Retícula basada en múltiplos de 8px (micro-espaciado 8px/16px, separaciones de sección generosas de 64px a 96px).
* **Reflujo Móvil:** Adaptabilidad móvil estricta (pila vertical en pantallas menores a 768px, botones de toque ergonómicos de mínimo 44px de altura, sliders horizontales para tarjetas).

---

## 6. Design System Notes for Stitch Generation (Guía para Generación en Stitch)

Cuando uses Stitch para generar nuevas pantallas o componentes para Envios DosRuedas, utiliza las siguientes directivas textuales:

```markdown
**DESIGN SYSTEM (ENVIOS DOSRUEDAS MAR DEL PLATA - MANDATORY SPEC):**
- **Atmosphere:** High-speed urban motorcycle courier & e-commerce logistics in Mar del Plata. Confident, athletic-utilitarian, crisp, ultra-reliable. High-contrast Royal Blue (#0950f6) and Signal Yellow (#ffec01).
- **Color Tokens (Max Darkness Cap = #0950f6):**
  - Brand Royal Blue: #0950f6 (Hero backgrounds, heavy headers, dark card surfaces, footer)
  - Signal Yellow: #ffec01 (Primary CTAs, status badges, highlighted title tags, star ratings)
  - Signal Yellow Hover: #fff240
  - Pure Canvas White: #ffffff (Page background, light cards, high-contrast text on blue)
  - Subtle Blue Surface: #f0f5ff / #f3f7ff (Inputs, table stripes, metric cards)
  - Soft Ice Border: #e0ebff / #e8f0fe / rgba(9,80,246,0.15)
  - Translucent Layering on Blue: Use bg-brand-blue-500 with border-white/10 or border-white/20, or bg-white/5 to bg-white/10 with backdrop-blur-md.
  - STRICTLY BANNED COLORS: Zero blue-900, zero blue-950, zero brand-blue-900 (#041F5E), zero navy, zero pure black (#000000), zero neutral gray/slate classes (text-slate-*, text-gray-*). Subdued copy on light backgrounds must use text-brand-blue/70 or text-brand-blue/80.
- **Typography Rules:**
  - Display Titles: 'Anton', 'Impact', sans-serif (UPPERCASE, tracking-tight, leading-[0.92], impactful)
  - Interface & Body: 'Outfit', sans-serif (Clean geometric sans, regular/semibold/bold, leading-relaxed)
  - Data / Telemetry: 'Geist Mono', monospace (UPPERCASE, tracking-wider, text-xs, cutoffs, KM, prices)
  - Icons: Google Material Symbols Outlined
- **Component Geometry:**
  - Action Buttons: Pill-shaped (rounded-full). Primary buttons have #ffec01 background, #0950f6 Anton text, and an arrow icon that slides on hover.
  - Feature Cards: Phone-like heavily rounded corners (rounded-3xl or rounded-[36px]), 4px borders (border-4 border-white or border-brand-yellow), and deep blue shadows: box-shadow 0 30px 60px -12px rgba(0,20,100,0.45).
  - Tilted Tags: Inline title badges with slight rotation (-rotate-1 or rotate-1) on yellow backgrounds.
  - Form Fields: Rounded-xl, white or #f0f5ff background, subtle 1px blue border, focus ring in #0950f6.
  - Domain Modules: Interactive radio-cards for delivery slots (9-19 hs), picking rack visualizer for fulfillment, 3-step timeline for cash-on-delivery.
- **Layout & Structure:**
  - Alternating section blocks: Electric Blue sections alternating with crisp White sections.
  - Max width: max-w-7xl with px-4 lg:px-8.
  - Responsive: Single-column stack on mobile (<768px), horizontal touch sliders for cards.
- **Banned Patterns:** No generic purple/pink gradients, no Inter font, no emojis as icons, no Math.ceil for distance pricing, no Factura A references.
```

---

## 7. Anti-Patrones y Reglas de Exclusión Absoluta

* 🚫 **Prohibido el uso de `blue-900`, `blue-950`, `brand-blue-900` (`#041F5E`) o cualquier tono más oscuro que `#0950F6`:** Toda la profundidad y el anidamiento de tarjetas dentro de secciones azules se resuelve exclusivamente con velos translúcidos (`border-white/10`, `border-white/20`, `bg-white/10` y `backdrop-blur-md`). La introducción de azules noche rompe la vibrancia deportiva y viola el ADR 02.
* 🚫 **Prohibido el uso de Negro Puro (`#000000`) o Grises Neutros (`slate`, `gray`, `zinc`, `neutral`):** Todo contraste profundo y texto secundario se resuelve en la gama del Azul Corporativo (`#0950F6`), ya sea pleno o con opacidades (`text-brand-blue/80`).
* 🚫 **Prohibidos los degradados fluorescentes violáceos o cian ("AI Neon Gradients"):** La paleta se fundamenta en bloques de color planos, sólidos y de alto impacto vial (`#0950F6` y `#FFEC01`).
* 🚫 **Prohibido el uso de tipografías genéricas (`Inter`, `Roboto`, fuentes Serif clásicas):** Se respeta estrictamente la terna identitaria `Anton` + `Outfit` + `Geist Mono`.
* 🚫 **Prohibido el uso de emojis en lugar de iconos:** Se emplean exclusivamente glifos vectoriales de `Material Symbols Outlined`.
* 🚫 **Prohibidas las esquinas angulosas en tarjetas principales:** Todo contenedor central debe presentar radios de curvatura suaves (`rounded-2xl`, `rounded-3xl` o `rounded-[36px]`).
* 🚫 **Prohibido `Math.ceil` en distancias y tarifas (ADR 01):** La tarifa por kilómetro excedente (10 a 20 km) es estrictamente lineal (`distancia * precioPorKm`).
* 🚫 **Prohibida la promesa de Factura A:** La empresa emite comprobantes conforme a su encuadre fiscal estándar, sin emisión de Factura A.
* 🚫 **Prohibidas las promesas horarias antirreglamentarias:** Envíos Express siempre se ofrece en franjas de 3 hs solicitadas con 2 hs de anticipación (corte 15:00 hs); LowCost se entrega hasta las 19:00 hs (corte 13:00 hs). Nunca prometer "en 2 horas" o calificar a LowCost como servicio "agrupado".