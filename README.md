# 🌍 Sianna Travel - Sitio Web de Agencia de Viajes

Sitio web responsive para agencia de viajes con diseño moderno en tonos azules/turquesa, funcionalidad completa y chatbot integrado.

## 📋 Características

### ✨ Principales Funcionalidades

- **Diseño 100% Responsive**: Se adapta perfectamente a dispositivos móviles, tablets y desktop
- **Chatbot Inteligente**: Asistente virtual integrado que responde preguntas sobre tours, precios, destinos y más
- **Búsqueda de Tours**: Sistema de filtrado por región y mes
- **Catálogo de Viajes**: Tarjetas interactivas con tours destacados
- **Navegación Fluida**: Menú responsive con animaciones suaves
- **Promociones Destacadas**: Badges visuales para ofertas 2x1, descuentos y MSI

### 🎨 Diseño

- **Colores corporativos**: Azul Turquesa (#4DADC9, #5DADE2) como color principal
- **Azules profundos**: (#2C5F7C, #1E4D66) para contraste
- **Rojo de acento**: (#E74C3C) solo para detalles importantes y llamados a la acción
- **Efecto de mapa del mundo**: En el fondo del hero
- **Tipografía moderna y legible**
- **Iconos de Font Awesome**
- **Animaciones CSS suaves**
- **Efectos hover interactivos**
- **Secciones bien organizadas**

### 🤖 Chatbot Inteligente

El chatbot incluye respuestas automáticas para:
- Información sobre tours y destinos
- Consultas de precios y promociones
- Información sobre vuelos, hoteles y seguros
- Detalles de destinos específicos (Europa, Asia, Caribe, México)
- Información de contacto y sucursales
- Financiamiento y métodos de pago
- Mundo Joven Fest 2026

## 🚀 Instalación y Uso

### Requisitos Previos

- Navegador web moderno (Chrome, Firefox, Safari, Edge)
- Servidor web local (opcional) o abrir directamente el archivo HTML

### Opción 1: Abrir Directamente

1. Navega a la carpeta del proyecto
2. Doble clic en `index.html`
3. El sitio se abrirá en tu navegador predeterminado

### Opción 2: Servidor Local (Recomendado)

Con Python 3:
```bash
python -m http.server 8000
```

Con Node.js (http-server):
```bash
npx http-server
```

Con PHP:
```bash
php -S localhost:8000
```

Luego abre tu navegador en `http://localhost:8000`

### Opción 3: Visual Studio Code (Live Server)

1. Instala la extensión "Live Server"
2. Click derecho en `index.html`
3. Selecciona "Open with Live Server"

## 📁 Estructura del Proyecto

```
assana/
│
├── index.html          # Estructura HTML principal
├── styles.css          # Estilos CSS responsive
├── script.js           # JavaScript y lógica del chatbot
└── README.md           # Este archivo
```

## 🎯 Secciones del Sitio

### Header
- Barra superior con información de contacto
- Logo de Sianna Travel
- Menú de navegación responsive con iconos
- Toggle para dispositivos móviles

### Hero Section
- Banner promocional del Sianna Travel Fest 2026
- Información del evento (28 feb - 1 mar 2026, Centro Banamex)
- Badges de promociones (2x1, 50% desc, 24 MSI)
- Llamada a la acción "Regístrate Gratis"
- Eslogan "Descubre el mundo"
- Efecto de mapa del mundo en el fondo

### Búsqueda de Tours
- Tabs para diferentes servicios (Vuelos, Seguros, Tours, etc.)
- Formulario de búsqueda con filtros
- Selección de región y mes
- Botón de búsqueda

### Tours Destacados
- Grid de tarjetas de tours
- Imágenes de destinos
- Información de duración y descripción
- Precios desde
- Badges de ofertas especiales
- Botones de acción

### Servicios
- Grid de servicios principales
- Iconos representativos
- Descripciones breves
- Efectos hover

### Footer
- Información de la empresa
- Enlaces rápidos
- Información de contacto
- Redes sociales
- Copyright

### Chatbot
- Botón flotante para activar
- Ventana de chat minimizable
- Respuestas automáticas inteligentes
- Respuestas rápidas sugeridas
- Diseño moderno y funcional

## 💻 Funcionalidades JavaScript

### Menú Móvil
```javascript
// Toggle automático del menú en dispositivos móviles
// Cierre automático al hacer click fuera del menú
```

### Tabs de Búsqueda
```javascript
// Sistema de pestañas para diferentes tipos de búsqueda
// Vuelos, Seguros, Tours, Vuelo+Hotel, Hoteles
```

### Formulario de Búsqueda
```javascript
// Validación de formulario
// Prevención de envío sin datos requeridos
```

### Chatbot
```javascript
// Sistema de mensajes usuario/bot
// Generación automática de respuestas
// Detección de palabras clave
// Indicador de escritura
// Respuestas rápidas
```

### Animaciones
```javascript
// Scroll suave para enlaces ancla
// Animaciones on-scroll para tarjetas
// Efectos de entrada
```

### Easter Egg
```javascript
// Código Konami para descuento especial
// ↑ ↑ ↓ ↓ ← → ← → B A
```

## 🎨 Personalización

### Cambiar Colores

Edita las variables CSS en `styles.css`:

```css
:root {
    --primary-blue: #4DADC9;      /* Azul turquesa principal */
    --primary-turquoise: #5DADE2; /* Turquesa claro */
    --dark-blue: #2C5F7C;         /* Azul oscuro */
    --deep-blue: #1E4D66;         /* Azul profundo */
    --accent-red: #E74C3C;        /* Rojo de acento */
}
```

### Modificar Respuestas del Chatbot

Edita la función `generateBotResponse()` en `script.js`:

```javascript
function generateBotResponse(userMessage) {
    // Agrega nuevas condiciones y respuestas aquí
    if (message.includes('tu_palabra_clave')) {
        return 'Tu respuesta personalizada';
    }
}
```

### Agregar Nuevos Tours

Duplica y modifica el HTML en la sección `.tours-grid`:

```html
<div class="tour-card">
    <div class="tour-image">
        <img src="URL_IMAGEN" alt="Destino">
        <span class="tour-badge">Nuevo</span>
    </div>
    <div class="tour-info">
        <h3>Nombre del Tour</h3>
        <!-- Más contenido -->
    </div>
</div>
```

## 📱 Responsive Breakpoints

- **Desktop**: > 1024px (diseño completo)
- **Tablet**: 768px - 1024px (menú compacto)
- **Mobile**: < 768px (menú hamburguesa)
- **Small Mobile**: < 480px (optimización adicional)

## 🔧 Mejoras Futuras (Sugeridas)

- [ ] Integración con backend real
- [ ] Base de datos de tours
- [ ] Sistema de reservaciones
- [ ] Pasarela de pagos
- [ ] Panel de administración
- [ ] Galería de imágenes de destinos
- [ ] Sistema de reseñas y calificaciones
- [ ] Newsletter/suscripción
- [ ] Multi-idioma (i18n)
- [ ] Chatbot con IA real (OpenAI, DialogFlow)
- [ ] Búsqueda avanzada con filtros adicionales
- [ ] Comparador de paquetes
- [ ] Mapa interactivo de destinos

## 🛠️ Tecnologías Utilizadas

- **HTML5**: Estructura semántica
- **CSS3**: Estilos modernos, Flexbox, Grid, Animaciones
- **JavaScript ES6+**: Funcionalidad e interactividad
- **Font Awesome 6.4.0**: Iconos
- **Google Fonts**: Tipografías (Sistema)

## 🌐 Compatibilidad de Navegadores

- ✅ Chrome (90+)
- ✅ Firefox (88+)
- ✅ Safari (14+)
- ✅ Edge (90+)
- ✅ Opera (76+)

## 📞 Información de Contacto (Ejemplo)

- **Teléfono**: (55) 54 82 82 82
- **Email**: info@siannatravel.com
- **Website**: siannatravel.com
- **Evento**: Sianna Travel Fest 2026
  - Fechas: 28 de febrero - 1 de marzo 2026
  - Lugar: Centro Banamex

## 📄 Licencia

Este es un proyecto de demostración educativo. El diseño está inspirado en Mundo Joven para fines ilustrativos.

## 👨‍💻 Desarrollo

Desarrollado como ejemplo de sitio web responsive para agencia de viajes con las mejores prácticas de desarrollo web.

## 🎉 Características Especiales

### Chatbot Inteligente
El chatbot incluye más de 20 patrones de respuesta diferentes que cubren:
- Consultas generales
- Información de destinos
- Precios y promociones
- Métodos de pago
- Contacto y sucursales
- Eventos especiales

### Animaciones y Efectos
- Transiciones suaves en hover
- Animaciones de entrada para tarjetas
- Efectos de scroll
- Indicadores visuales
- Feedback inmediato al usuario

### Optimización
- CSS optimizado con variables
- JavaScript modular y comentado
- Imágenes optimizadas vía Unsplash
- Carga rápida de recursos
- Performance monitoring

## 📸 Capturas de Pantalla

El sitio incluye:
- Hero banner impactante con promociones
- Sistema de búsqueda intuitivo
- Galería de tours con imágenes atractivas
- Chatbot flotante siempre disponible
- Footer completo con información

## 🚢 Siguientes Pasos

Para poner este sitio en producción:

1. **Optimizar Imágenes**: Reemplaza los URLs de Unsplash con imágenes propias optimizadas
2. **Backend**: Implementa un servidor (Node.js, Python, PHP)
3. **Base de Datos**: MySQL, MongoDB o PostgreSQL para tours
4. **CDN**: Usa un CDN para recursos estáticos
5. **SEO**: Agrega meta tags, sitemap, robots.txt
6. **Analytics**: Integra Google Analytics o similar
7. **Formularios**: Conecta con servicio de email (SendGrid, etc.)
8. **Seguridad**: SSL, headers de seguridad, validación backend

## ⭐ Agradecimientos

- Diseño inspirado en Mundo Joven
- Iconos por Font Awesome
- Imágenes de ejemplo por Unsplash

---

**¡Disfruta explorando el mundo con Mundo Joven!** 🌍✈️🏖️
