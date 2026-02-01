# TechCiberSolutions - Sitio Web de Servicios Informáticos

## 📋 Objetivo del Proyecto

Este proyecto consiste en una página web estática profesional para una empresa de servicios informáticos. El sitio está diseñado para presentar los servicios de la empresa de manera clara y atractiva, facilitando la comunicación con clientes potenciales y proporcionando información relevante sobre los servicios ofrecidos.

## 📁 Estructura de Archivos

```
Proyecto_Informatico/
│
└── PROYECTO_INFORMATICO/
    ├── index.html          # Página principal con todas las secciones
    ├── styles.css          # Archivo de estilos CSS3
    ├── README.md           # Documentación del proyecto
    └── assets/
        ├── fondo de pantalla.jpg   # Fondo tipo wallpaper (HD)
        └── README.md               # Guía para fondos/recursos
```

### Descripción de Archivos

- **index.html**: Contiene toda la estructura HTML5 semántica del sitio web, incluyendo las secciones de navegación, inicio, servicios, sobre nosotros, contacto y footer.

- **styles.css**: Archivo CSS3 externo que contiene todos los estilos del sitio, incluyendo diseño responsive para diferentes dispositivos (desktop, tablet y móvil).

- **README.md**: Este archivo de documentación que explica el proyecto, su estructura y cómo modificarlo.

## 🏗️ Estructura del HTML

El archivo `index.html` está organizado en las siguientes secciones principales:

### 1. **Head (Cabecera)**
- Metadatos del documento (charset, viewport, description)
- Título de la página
- Enlace al archivo CSS externo

### 2. **Header (Navegación)**
- Barra de navegación fija en la parte superior
- Logo de la empresa
- Menú de navegación con enlaces a las secciones
- Menú hamburguesa para dispositivos móviles

### 3. **Sección Hero (Inicio)**
- Presentación principal tipo “landing” (hero)
- Título, subtítulo y botones (CTA)
- Accesos rápidos tipo “chips” (categorías)
- Panel lateral de contacto rápido

### 4. **Sección Servicios**
- Grid responsivo con 6 tarjetas de servicios:
  - Ciberseguridad
  - Análisis y Diseño de Software
  - Diseño de Redes de Computadoras
  - Diseño e Instalación de Cableado Estructurado
  - Diseño y Configuración de Redes WiFi
  - Asesorías Generales en Informática

### 5. **Sección Proyectos**
- Bloque informativo para planificación e implementación de proyectos

### 6. **Sección Cobertura**
- Bloque de cobertura/atención con panel lateral y mini “estadísticas”

### 7. **Sección Preguntas Frecuentes (FAQ)**
- Implementada con `details/summary` (HTML semántico)

### 8. **Sección Sobre Nosotros**
- Información sobre la empresa
- Valores y misión
- Características destacadas (años de experiencia, equipo certificado, etc.)

### 9. **Sección Contacto**
- Información de contacto (email, teléfono, dirección, horario)
- Formulario de contacto visual (sin funcionalidad backend)
- Campos: nombre, email, teléfono, servicio de interés, mensaje

### 10. **Footer (Pie de Página)**
- Información adicional de la empresa
- Enlaces rápidos
- Copyright

### 8. **Scripts JavaScript**
- Funcionalidad del menú hamburguesa móvil
- Smooth scroll para navegación suave
- Prevención de envío del formulario (solo visual)

## 🎨 Tecnologías Utilizadas

- **HTML5**: Estructura semántica del documento
- **CSS3**: Estilos modernos con:
  - Variables CSS (custom properties)
  - Flexbox y Grid Layout
  - Animaciones y transiciones
  - Media queries para responsive design
- **JavaScript Vanilla**: Funcionalidades interactivas básicas
- **Sin frameworks externos**: Código puro sin dependencias

## 🎯 Características del Diseño

### Diseño Responsive
El sitio está completamente optimizado para tres tipos de dispositivos:

1. **Desktop** (> 968px): Diseño completo con múltiples columnas
2. **Tablet** (768px - 968px): Adaptación de columnas y espaciado
3. **Móvil** (< 768px): Diseño de una columna con menú hamburguesa

### Paleta de Colores
- **Color primario**: Azul (#0066cc)
- **Color secundario**: Azul claro (#00a8ff)
- **Color de acento**: Cyan (#00d4ff)
- **Texto oscuro**: #1a1a1a
- **Texto claro**: #666666
- **Fondo claro**: #f8f9fa

### Tipografía
- Fuente principal: Segoe UI (sistema)
- Tamaños responsivos según dispositivo

## 🛠️ Instrucciones para Modificar o Ampliar el Sitio

### Modificar Contenido

1. **Cambiar el nombre de la empresa**:
   - Buscar "TechCiberSolutions" en `index.html` y reemplazar con el nombre deseado
   - Actualizar también en el logo y footer

2. **Modificar información de contacto**:
   - Editar la sección `contact-info` en `index.html`
   - Actualizar email, teléfono, dirección y horario

3. **Agregar o modificar servicios**:
   - Encontrar la sección `services-grid` en `index.html`
   - Copiar una tarjeta de servicio (`service-card`) y modificar el contenido
   - Ajustar el grid en CSS si es necesario

4. **Modificar colores**:
   - Editar las variables CSS en `:root` al inicio de `styles.css`
   - Cambiar los valores de `--primary-color`, `--secondary-color`, etc.

### Cambiar el fondo tipo “wallpaper”

1. Reemplaza el archivo:
   - `PROYECTO_INFORMATICO/assets/fondo de pantalla.jpg`
2. Si cambias el nombre, edita esta línea en `styles.css`:
   - `background-image: url("./assets/fondo de pantalla.jpg");`

### Agregar Nuevas Secciones

1. Crear una nueva sección en `index.html`:
```html
<section id="nueva-seccion" class="nueva-clase">
    <div class="container">
        <!-- Contenido aquí -->
    </div>
</section>
```

2. Agregar enlace en el menú de navegación:
```html
<li><a href="#nueva-seccion" class="nav-link">Nueva Sección</a></li>
```

3. Crear estilos en `styles.css` para la nueva sección

### Agregar Funcionalidad Backend al Formulario

Para conectar el formulario con un backend:

1. Modificar el atributo `action` del formulario:
```html
<form class="contact-form" action="tu-endpoint.php" method="POST">
```

2. Remover o modificar el script que previene el envío:
```javascript
// Eliminar o comentar esta línea:
e.preventDefault();
```

3. Agregar validación adicional si es necesario

### Optimizaciones Adicionales

- **Imágenes**: Agregar imágenes reales reemplazando los iconos emoji
- **SEO**: Mejorar meta tags, agregar Open Graph, schema.org
- **Accesibilidad**: Agregar atributos ARIA, mejorar contraste
- **Performance**: Minificar CSS y HTML, optimizar imágenes
- **Analytics**: Integrar Google Analytics u otra herramienta

## 📱 Compatibilidad

El sitio está diseñado para ser compatible con:
- Navegadores modernos (Chrome, Firefox, Safari, Edge)
- Dispositivos móviles (iOS y Android)
- Tablets
- Escritorio

## 🚀 Cómo Usar el Proyecto

1. Abrir `PROYECTO_INFORMATICO/index.html` en un navegador web moderno
2. No se requiere instalación de dependencias ni servidor
3. Para desarrollo, usar un servidor local (opcional):
   - Python: `python -m http.server 8000`
   - Node.js: `npx http-server`
   - VS Code: Extensión "Live Server"

## 📝 Notas Importantes

- El formulario de contacto es solo visual y no envía datos reales
- Los enlaces de navegación usan smooth scroll para mejor UX
- El menú hamburguesa solo aparece en dispositivos móviles
- Todos los textos están en español y son profesionales (no lorem ipsum)

## 🔄 Versión

- **Versión**: 1.0
- **Fecha**: 2024
- **Autor**: Proyecto desarrollado para empresa de servicios informáticos

---

**Nota**: Este proyecto está diseñado para trabajar dentro de Cursor y puede ser fácilmente modificado y ampliado según las necesidades específicas de la empresa.
