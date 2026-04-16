# Mi Jornada en el Ecosistema Linux - Landing Page

Una landing page limpia, responsive y minimalista que documenta mi experiencia de aprendizaje a través de 8 distribuciones Linux diferentes. El proyecto utiliza un diseño simple con fondo claro, cuadros blancos y texto negro para máxima legibilidad.

**Autor:** Winni  
**Proyecto:** SENATI  
**Año:** 2026

---

##  Descripción General

Esta landing page es un portafolio interactivo que presenta 8 distribuciones Linux organizadas por categorías:

- **Estabilidad y Fundamentos:** Debian, Ubuntu
- **Auditoría y Hacking Ético:** Kali Linux, Parrot OS  
- **Vanguardia y Control:** Fedora, Manjaro
- **Rendimiento y Gaming:** Zorin OS, Nobara

Cada distro incluye descripción, logo, e imagen de la interfaz de escritorio. La página también contiene un video educativo de YouTube y un formulario de contacto.

---

##  Características Principales

✅ **Diseño Minimalista** - Fondo claro, cuadros blancos, letras negras (simple y limpio)  
✅ **Responsivo** - Se adapta perfectamente a cualquier pantalla (móvil, tablet, escritorio)  
✅ **Navegación Flotante** - Barra de navegación fija encima con enlaces suave a cada sección  
✅ **Animaciones Suaves** - Tarjetas con efecto de elevación y Intersection Observer  
✅ **Video Responsivo** - YouTube embed con proporción 16:9 automática  
✅ **Formulario Interactivo** - Campos blancos con feedback visual en focus  
✅ **Bien Documentado** - 3 archivos TXT explican cada CSS en detalle  
✅ **Logos Visibles** - Perfectamente visibles sobre fondo claro  

---

##  Estructura del Proyecto

```
Landing Page/
|
+-- index.html                    # Estructura HTML (todas las secciones)
+-- estilos.css                   # Estilos globales (colores, tipografía, layout)
+-- estilos-navbar.css            # Barra de navegación flotante
+-- estilo-form.css               # Formulario de contacto
+-- app.js                         # Animaciones (Intersection Observer)
|
+-- imagenes/                     # Carpeta de imágenes
│   ├── debian.jpg
│   ├── ubuntu.jpeg
│   ├── kali.jpg
│   ├── Parrot.webp
│   ├── fedora.webp
│   ├── manjaro.png
│   ├── zorin.png
│   └── nobara.png
│

```

---

## Requisitos

- Navegador web moderno (Chrome, Firefox, Safari, Edge)
- Conexión a internet (para Google Fonts y YouTube)
- No requiere backend ni herramientas especiales

---

## Instalación y Uso

### Opción 1: Clonar desde Git

```bash
# Clonar el repositorio
git clone https://github.com/Pineda-25/landing-page-distros.git

# Navegar a la carpeta
cd "Landing Page"

# Abrir en navegador (elegir uno según tu S.O.)

# Linux/Mac:
open index.html

# Windows (PowerShell):
Start-Process index.html

# O simplemente arrastra index.html al navegador
```

### Opción 2: Uso Directo

1. Descarga todos los archivos
2. Asegúrate que la carpeta `imagenes/` esté en el mismo nivel que `index.html`
3. Abre `index.html` en tu navegador
4. ¡Listo! La página cargará automáticamente

---

## Stack Tecnológico

### Frontend

| Tecnología | Propósito | Versión |
|------------|-----------|---------|
| HTML5 | Estructura semántica | - |
| CSS3 | Estilos y animaciones | - |
| JavaScript (Vanilla) | Animaciones en scroll | ES6 |
| Google Fonts | Tipografía | Poppins, Inter |

### APIs Externas

- **YouTube Embed API** - Video educativo 16:9
- **Simple Icons** - Logos de distros Linux

---

## Estructura de Secciones

### 1. **Navbar (Barra de Navegación)**
```
Position: Fixed (encima de todo)
Contenido: 7 enlaces a secciones (Inicio, Estabilidad, Seguridad, etc.)
```

### 2. **#inicio (Introducción)**
```
Contenido: Título grande + párrafo centrado
Propósito: Presentar el concepto de la jornada Linux
```

### 3. **#estables (Estabilidad y Fundamentos)**
```
Contenido: 2 tarjetas (Debian, Ubuntu)
```

### 4. **#seguridad (Auditoría y Hacking Ético)**
```
Contenido: 2 tarjetas (Kali, Parrot)
Enfoque: Herramientas de seguridad
Colores: Kali (azul), Parrot (cian)
```

### 5. **#vanguardia (Vanguardia y Control)**
```
Contenido: 2 tarjetas (Fedora, Manjaro)
Enfoque: Software actualizado y control
Colores: Fedora (azul claro), Manjaro (verde)
```

### 6. **#rendimiento (Rendimiento y Gaming)**
```
Contenido: 2 tarjetas (Zorin, Nobara)
Enfoque: Rendimiento y creadores
Colores: Zorin (cian), Nobara (azul claro)
```

### 7. **#multimedia (Video)**
```
Contenido: Video YouTube + descripción
Proporción: 16:9 automática
ID Video: P003kpGUl9k
```

### 8. **#contacto (Formulario)**
```
Contenido: 3 inputs (Nombre, Email, Comentario) + Botón enviar
Diseño: Centrado max-width 480px
Estilo: Blanco puro con bordes grises sutiles
```

### 9. **footer (Pie de Página)**
```
Contenido: Crédito y proyecto
Estilo: Texto negro sin líneas divisorias
```

---

## Paleta de Colores

| Color | Hex | Uso |
|-------|-----|-----|
| **Fondo Principal** | `#f5f5f5` | Fondo de toda la página |
| **Blanco Puro** | `#ffffff` | Tarjetas, formulario, navbar |
| **Negro Puro** | `#000000` | Títulos, texto principal, botones |
| **Gris Claro** | `#f5f5f5` | Inputs del formulario |
| **Gris Medio** | `#cccccc` | Bordes sutiles |
| **Gris Oscuro** | `#333333` | Botones en hover |
| **Blanco Transparente** | `rgba(255, 255, 255, 0.95)` | Navbar con semi-transparencia |
| **Negro Transparente** | `rgba(0, 0, 0, 0.1)` | Fondos en hover de botones |

Diseño simple: solo blanco, negro y grises para máxima claridad.

---

## Cómo Se Hizo

### Proceso de Desarrollo

1. **Concepto y Planificación**
   - Identificar 8 distros significativas en mi aprendizaje
   - Organizar por categorías educativas
   - Diseñar estructura de secciones

2. **Maquetado HTML**
   - Estructura semántica con `<section>` para cada categoría
   - `<article>` para cada tarjeta de distro
   - Formulario con `<form>` y `<input>` apropiados
   - Embed de YouTube con `<iframe>`

3. **Diseño CSS**
   - Reset de estilos con `* { margin: 0; padding: 0; }`
   - Sistema de colores minimalista (blanco, negro, grises)
   - Layout con Flexbox (sin CSS Grid para simplicidad)
   - Transiciones suaves (0.2s - 0.3s)
   - Sin animaciones complejas ni decoraciones
   - Media queries para responsividad
   - Bordes: sutiles o sin bordes para diseño limpio

4. **Animaciones JavaScript**
   - Intersection Observer API para detectar cuando elementos entran al viewport
   - Animación de entrada suave: fade-in y translateY
   - Transiciones simples sin efectos complejos
   - Solo 25 líneas de código (muy minimalista)

5. **Optimizaciones**
   - Responsividad móvil-first
   - Imágenes optimizadas (.jpg, .png, .webp)
   - Google Fonts para tipografía
   - Simple Icons para logos
   - Barra navbar flotante con `position: fixed` y `z-index: 1000`

6. **Iteraciones y Simplificación**
   - Versión inicial: Fondo azul oscuro, colores cian/azul, bordes coloridos
   - Versión actual: Fondo claro, blanco/negro/gris, sin decoraciones
   - Resultado: Más legible, más profesional, más fácil de mantener

---

## Animaciones

### Tarjetas de Distros
```css
Estado Normal:
  - scale: 1
  - translateY: 0
  - opacity: 1

Hover:
  - Elevan 5px (translateY: -5px)
  - Fondo permanece blanco
  - Imagen dentro amplía 2% (scale: 1.02)
  - Transición: 0.3s ease

En Scroll (Intersection):
  - Entran desde abajo con fade
  - Transición suave sin efectos complejos
```

### Botones
```css
Navbar:
  - Normal: texto negro
  - Hover: fondo gris suave + scale(1.08)
  - Transición: 0.3s ease

Formulario:
  - Normal: fondo negro
  - Hover: gris oscuro + scale(1.03)
  - Transición: 0.2s ease

Inputs:
  - Normal: fondo gris claro
  - Focus: borde negro, fondo blanco
```

### Video
```css
Normal: 100% ancho con aspect-ratio 16/9
Hover: amplía 2% (scale: 1.02)
```

---



### v1.0 - Lanzamiento Inicial
-  Diseño con glassmorphism
- Animaciones complejas con múltiples delays
-  Sistema de colores gradiente
-  8 distros Linux categorizado

---

## Técnicas HTML/CSS/JS Utilizadas

### HTML5
- `<section>` para agrupación semántica
- `<article>` para tarjetas independientes
- `<nav>` con `<ul>` y `<li>` para navegación
- `<form>` con inputs semánticamente correctos
- `<iframe>` para embed de YouTube
- Atributos `data-*` no usados (vanilla JS simple)

### CSS3
- **Flexbox:** Alineamiento y distribución de elementos
- **Aspect-ratio:** Video responsivo sin JS
- **Transitions:** Animaciones suaves
- **Transform:** Escala y traslación sin afectar layout
- **Box-shadow:** Sombras sutiles
- **Filter:** Drop-shadow en logos
- **Pseudo-elementos:** `::after` para líneas decorativas
- **Pseudo-clases:** `:hover`, `:focus`

### JavaScript (25 líneas)
- **Intersection Observer API:** Detecta cuando elementos entran al viewport
- **arrow functions:** `(() => {})` para callbacks
- **Modern ES6:** let, const, template literals no usados aquí

---

## Métricas del Proyecto

| Métrica | Valor |
|---------|-------|
| Tamaño total | 2.0 MB |
| Archivos HTML | 1 |
| Archivos CSS | 3 |
| Archivos JS | 1 (25 líneas) |
| Imágenes | 8 |
| Documentación TXT | 3 (45 KB) |
| Distros Linux | 8 |
| Secciones | 9 |
| Colores únicos | 18+ |

---

## Notas Importantes

1. **Conexión a Internet:** Requiere para Google Fonts y YouTube
2. **Imágenes:** La carpeta `imagenes/` debe estar en el mismo directorio
3. **Compatibilidad:** Funciona en todos los navegadores modernos
4. **Formulario:** Actualmente no envía datos (requiere backend)
5. **SEO:** Usa etiquetas semánticas correctas pero sin `<meta description>`

---

## Contacto

**Autor:** Winni  
**Proyecto:** Jornada en el Ecosistema Linux - SENATI  
**Año:** 2026

Para sugerencias o preguntas sobre el proyecto, usar el formulario en la página.

---

## Licencia

Este proyecto es de propósito educativo. Libre para usar, modificar y distribuir.

---

## Checklist de Uso

- Descargar/Clonar repositorio
- Verificar que exista carpeta `imagenes/`
- Abrir `index.html` en navegador
- Probar navegación (scroll y botones navbar)
- Verificar animaciones de tarjetas
- Llenar formulario y probar interacción
- Reproducir video de YouTube
- Probar en diferentes tamaños de pantalla
- Leer documentación TXT si deseas aprender CSS

---

Disfruta explorando el mundo de Linux con esta landing page minimalista y limpia.

