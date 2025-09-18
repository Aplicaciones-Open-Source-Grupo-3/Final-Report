# Capítulo IV: Product Design
## 4.1. Style Guidelines
En esta sección, presentamos nuestra propuesta de diseño para el landing page y la aplicación web. 

### 4.1.1. General Style Guidelines
**Tono de Comunicación** <br>
EasyPark comunica eficiencia, modernidad y confianza. Su tono es profesional, directo y claro, pensado para administradores y operadores de estacionamientos que necesitan rapidez en la gestión. La experiencia busca transmitir seguridad y control, con un lenguaje sencillo y accesible.

**Tipografía:** <br>
- **Inter Bold** → Títulos y subtítulos (claridad y jerarquía).
- **Inter Medium** → Textos descriptivos y secundarios (legibilidad y neutralidad).

**Colores de la Marca:**<br>

- **Primarios:**
  
    - **Azul Casi Negro (#121A21):** fondo principal de la aplicación.
    - **Azul Profundo (#1A2633):** fondos de cuadros interactivos.
    - **Azul Brillante (#1273D4):** botones primarios y acciones principales.
    - **Blanco (#FFFFFF):** títulos, subtítulos y textos principales.

- **Secudarios:**

    - **Celeste Claro (#91ADC9):** textos secundarios.
    - **Azul Marino (#243647):** cuadros de texto.
    - **Azul Oscuro (#334D66):** bordes.
    - **Gris Claro (#E5E8EB):** líneas separadoras.
    - **Gris Medio (#757575):** descripciones, textos secundarios.
    - **Verde (#0AD95C):** estados disponibles, éxito.
    - **Naranja (#FA6138):** alertas y notificaciones.

**Paleta de Colores:**<br>

| Color           | Código Hex | Uso Principal                             |
| --------------- | ---------- | ----------------------------------------- |
| Blanco          | #FFFFFF    | Títulos, subtitulos, textos                       |
| Celeste Claro   | #91ADC9    | Textos secundarios           |
| Azul Marino     | #243647    | Cuadros de texto          |
| Gris Claro      | #E5E8EB    | Lineas separadoras              |
| Azul Oscuro     | #334D66    | Bordes                 |
| Azul Profundo   | #1A2633    | Fondos de cuadros interactivos            |
| Azul Casi Negro | #121A21    | Fondo de la aplicación                |
| Azul Brillante  | #1273D4    | Botones primarios, acciones principales   |
| Gris Medio      | #757575    | Textos secundarios, descripciones         |
| Verde           | #0AD95C    | Estados disponibles, éxito en operaciones |
| Naranja         | #FA6138    | Alertas y notificaciones                  |

**Spacing y Layout:**<br>
- **Espaciado amplio:** se prioriza la lectura y el orden visual.
- **Margen mínimo:** 16px en mobile, 24px en desktop.
- **Grid layout:** 12 columnas en desktop, 4–6 en mobile.
- **Botones:** rectangulares con esquinas levemente redondeadas (border-radius 8–12px), padding interno (12px 24px).
- **Consistencia:** todas las pantallas mantienen el mismo patrón de navegación lateral y secciones de contenido centralizadas.


### 4.1.2. Web Style Guidelines

Se utilizó el patrón de lectura Z para guiar la atención del usuario desde el logo y menú superior, hacia el mensaje principal y finalmente a la imagen del producto. Este recorrido visual permite una lectura fluida y rápida, ideal para captar el mensaje en pocos segundos.

**Responsive Design**
El diseño se adapta a desktop, tablet y mobile. Se mantiene un look & feel oscuro con acentos de color para guiar la atención.

**Componentes Implementados:**
- **Login/Register/Remember:** formularios simples con contraste claro.
- **Dashboard (Admin/Operator):** panel lateral con accesos rápidos + mapa central con estado en tiempo real.
- **Gestión de Plazas:** tabla + mapa visual con colores según disponibilidad.
- **Reportes y Analítica:** gráficas, métricas de ingresos, ocupación y actividad.
- **Pantalla de Operador:** flujos rápidos de entrada/salida y procesamiento de pagos.

**Interacciones:**
- **Hover sobre botones:** cambio de tonalidad (azul → celeste).
- **Indicadores dinámicos:** verde para disponible, rojo para ocupado, naranja para incidencia.
- **Animaciones ligeras:** transiciones suaves al cambiar de vistas.

## 4.2. Information Architecture
Orden lógico de las secciones

1. **Login/Register/Remember**
2. **Administrador**
   
   - Dashboard general (mapa + métricas).
   - Configuración de estacionamiento.
   - Gestión de plazas (mapa/tabla).
   - Tarifas y abonos.
   - Gestión de operadores.
   - Reportes y analítica.

3. **Operador**

    - Registro de entradas (ticket QR o impreso).
    - Procesar salidas (cobro + liberación de plaza).
    - Control en tiempo real.
    - Reporte de incidencias.
    - Reservas y clientes abonados.

### 4.2.1. Organization Systems

- **Jerárquico:** primero la visión general (ocupación), luego la gestión detallada (plazas, tarifas, usuarios).
- **Secuencial:** flujo de entrada → pago → salida.
- **Por audiencia:**
  
  - Administradores → configuración, métricas, control total.
  - Operadores → flujos rápidos de entradas/salidas y resolución de incidencias.

### 4.2.2. Labeling Systems

Un sistema de etiquetado claro y consistente es esencial para facilitar la navegación y comprensión del producto, tanto en la landing page como en la aplicación web.

#### Landing Page
- **Menú Principal:** Inicio, Características, Precios, Contacto, Ingresar.
- **Secciones:** Títulos y subtítulos descriptivos como “¿Cómo funciona?”, “Planes y Precios”, “Contáctanos”.
- **Botones:** Etiquetas directas y orientadas a la acción, por ejemplo “Comenzar”, “Solicitar Demo”, “Ver planes”.
- **Mensajes y alertas:** Textos breves y claros, como “Enviado con éxito” o “Error de autenticación”.

#### Aplicación Web
- **Menú Lateral:** Dashboard, Plazas, Tarifas, Operadores, Reportes, Configuración, Salir.
- **Acciones rápidas:** “Agregar”, “Editar”, “Eliminar”, “Ver Detalles”, “Descargar Reporte”.
- **Indicadores:** Etiquetas de estado como “Disponible”, “Ocupado”, “Incidencia”, “Abonado”.
- **Formularios:** Campos con etiquetas como “Nombre”, “Correo”, “Contraseña”, “Placa del vehículo”, “Tarifa”.

**Principios aplicados:**
- Claridad y brevedad en los nombres.
- Consistencia en el uso de términos a lo largo de todo el sistema.
- Utilización de iconografía complementaria en menús y botones para mejorar el reconocimiento rápido.

### 4.2.3. SEO Tags and Meta Tags

La optimización SEO es clave para mejorar la visibilidad del producto en motores de búsqueda y asegurar el alcance a usuarios potenciales.

#### Landing Page

**Meta Tags:**
- `<title>EasyPark - Gestión eficiente de estacionamientos</title>`
- `<meta name="description" content="EasyPark es una plataforma avanzada para la administración y operación de estacionamientos, optimizando la gestión y el control en tiempo real." />`
- `<meta name="keywords" content="estacionamiento, gestión, administración, parking, reservas, operadores, control, analítica, automatización" />`
- `<meta name="viewport" content="width=device-width, initial-scale=1.0" />`
- `<meta property="og:title" content="EasyPark - Gestión eficiente de estacionamientos" />`
- `<meta property="og:description" content="Optimiza y digitaliza la administración de tu estacionamiento con EasyPark." />`
- `<meta property="og:image" content="URL_de_imagen_destacada" />`
- `<meta property="og:type" content="website" />`

**Otras recomendaciones:**
- Uso de etiquetas `alt` descriptivas en todas las imágenes.
- URLs legibles y amigables (ejemplo: `/precios`, `/caracteristicas`).
- Estructuración semántica del HTML con encabezados jerárquicos (`<h1>`, `<h2>`, etc.).


### 4.2.4. Searching Systems

La búsqueda eficiente es indispensable para que los usuarios encuentren información relevante de manera rápida.

#### Landing Page
- No se requiere un sistema de búsqueda avanzado, ya que la información es estática y accesible mediante el menú principal y los enlaces de las secciones.

#### Aplicación Web
- **Barra de búsqueda global:** Presente en el dashboard para encontrar rápidamente plazas, usuarios, o reportes.
- **Filtros y búsqueda contextual:** Dentro de módulos específicos (gestión de plazas, reportes, operadores), permitiendo filtrar por nombre, estado, fecha, etc.
- **Sugerencias automáticas:** Autocompletado de campos en formularios (por ejemplo, búsqueda de placas de vehículos o nombres de clientes).

**Principios aplicados:**
- Resultados relevantes y ordenados por prioridad.
- Tiempos de respuesta rápidos.
- Diseño accesible y visible en todas las pantallas principales.


### 4.2.5. Navigation Systems

Un sistema de navegación intuitivo y consistente es esencial para una experiencia de usuario óptima.

#### Landing Page
- **Menú superior fijo:** Acceso rápido a las secciones principales.
- **Botones de acción:** “Comenzar”, “Solicitar Demo”, siempre visibles en la cabecera y secciones clave.
- **Desplazamiento anclado (“scroll to”):** Los enlaces del menú desplazan suavemente a la sección correspondiente.
- **Footer:** Enlaces adicionales a redes sociales, términos y condiciones, políticas de privacidad, contacto.

#### Aplicación Web
- **Menú lateral:** Navegación principal para acceder a Dashboard, Plazas, Tarifas, Operadores, Reportes y Configuración. Permanece visible en todo momento.
- **Breadcrumbs:** Indican la ubicación actual dentro de módulos complejos.
- **Navegación contextual:** Botones de “volver” o “ir a inicio” en sub-módulos y formularios.
- **Accesos rápidos:** Íconos y atajos para tareas recurrentes.
- **Indicadores de estado:** Se resaltan las secciones activas y las notificaciones importantes.

**Principios aplicados:**
- Consistencia visual y funcional en todos los entornos.
- Acceso directo a funciones críticas en uno o dos clics.
- Adaptabilidad para todo tipo de dispositivos (diseño responsive).

## 4.3. Landing Page UI Design
En esta sección se presenta el diseño de la Landing Page de EasyPark, enfocado en captar la atención de los usuarios objetivo desde el primer contacto. El diseño busca comunicar claramente el valor del producto, generar confianza e incentivar la acción mediante una interfaz moderna, intuitiva y alineada a los principios de usabilidad.

### 4.3.1. Landing Page Wireframe
Para la elaboración de los wireframes de la landing page, hemos utilizado la herramienta de Figma para el proceso de diseño.

**Main section**: Es la sección principal de la landing page.

![main img](/assets/images/chapter-IV/LandingPage-wireframe-Main.png)

**About section**: Es la seccion donde se presenta el producto

![about img](/assets/images/chapter-IV/LandingPage-wireframe-About.png)

**How it works section**: Es la seccion donde se presentan las caracteristicas del producto

![about img](/assets/images/chapter-IV/LandingPage-wireframe-Howitworks.png)

**Pricing section**: Es la seccion donde se muestra los planes de suscripcion a los usuarios

![about img](/assets/images/chapter-IV/LandingPage-wireframe-Pricing.png)

**Contact section**: Es la seccion donde es usuario puede contactarse con el equipo

![about img](/assets/images/chapter-IV/LandingPage-wireframe-Contact.png)

### 4.3.2. Landing Page Mock-up
Para la elaboración de los mock-ups de la landing page, hemos utilizado la herramienta de Figma para el proceso de diseño.

**Main section**: Es la sección principal de la landing page.

![main img](/assets/images/chapter-IV/LandingPage-mockup-Main.png)

**About section**: Es la seccion donde se presenta el producto

![about img](/assets/images/chapter-IV/LandingPage-mockup-About.png)

**How it works section**: Es la seccion donde se presentan las caracteristicas del producto

![about img](/assets/images/chapter-IV/LandingPage-mockup-Howitworks.png)

**Pricing section**: Es la seccion donde se muestra los planes de suscripcion a los usuarios

![about img](/assets/images/chapter-IV/LandingPage-mockup-Pricing.png)

**Contact section**: Es la seccion donde es usuario puede contactarse con el equipo

![about img](/assets/images/chapter-IV/LandingPage-mockup-Contact.png)

## 4.4. Web Applications UX/UI Design
En esta sección se incluyen secciones internas en el cual se presentará y explicará la propuesta visual y de interacción para las aplicaciones que conforman la interacción del usuario con los productos digitales.

### 4.4.1. Web Applications Wireframes
![wireframes_web](/assets/images/chapter-IV/wireframes_web.png)

### 4.4.2. Web Applications Wireflow Diagrams

### 4.4.3. Web Applications Mock-ups

![mockups_web](/assets/images/chapter-IV/mockups_web.png)

### 4.4.4. Web Applications User Flow Diagrams

![user_flow_diagram](/assets/images/chapter-IV/user_flow_diagram.png)

## 4.5. Web Applications Prototyping

![user_flow_diagram](/assets/images/chapter-IV/user_flow_diagram.png)

## 4.6. Domain-Driven Software Architecture

El modelo C4 permite visualizar un sistema de software en distintos niveles de detalle, desde lo más general hasta lo más específico. Para EasyPark, se construyeron tres vistas: Contexto, Contenedores y Componentes, que facilitan entender cómo interactúan los usuarios con la plataforma, cómo está organizada su arquitectura interna y cómo se distribuyen las responsabilidades dentro del backend.

### 4.6.1. Software Architecture Context Diagram
En este diagrama muestra a EasyPark como un sistema en su ecosistema. Representa a los usuarios principales (administrador y operador) y a los sistemas externos (pasarelas de pago, notificaciones, mapas, etc.) con los que la plataforma se integra. Su objetivo es dar una visión clara de quién usa EasyPark y qué servicios externos lo rodean.
![c4](/assets/images/chapter-IV/structurizr-Context.png)

### 4.6.2. Software Architecture Container Diagrams
En este diagrama se abren los detalles de EasyPark y se representan sus contenedores principales: la WebApp, el Backend API, los servicios de dominio (espacios, reservas, pagos, reportes, incidencias, usuarios), la base de datos, el cache Redis y el worker de notificaciones. Este diagrama permite entender cómo se organizan las piezas internas del sistema y cómo se comunican entre sí y con los servicios externos.
![c4](/assets/images/chapter-IV/structurizr-Container.png)

### 4.6.3. Software Architecture Components Diagrams
En este diagrama se descompone el contenedor Backend API en sus componentes internos (controladores de autenticación, espacios, reservas, pagos, reportes, incidencias, validaciones y adaptadores de integración). El objetivo de este nivel es mostrar la distribución de responsabilidades dentro del backend, destacando qué hace cada componente y cómo se relaciona con los servicios de dominio, la base de datos y los sistemas externos.
![c4](/assets/images/chapter-IV/structurizr-Component.png)


## 4.7. Software Object-Oriented Design
En la sección de Software Object-Oriented Design se presentarán del diagrama de clases de la aplicacion.

### 4.7.1. Class Diagrams

![diagram](/assets/images/chapter-IV/class-diagram.png)


## 4.8. Database Design
En la parte dedicada al Diseño de la Base de Datos, se mostrará un diagrama que ilustra cómo están organizadas las entidades y sus vínculos, facilitando un manejo eficiente de los datos tanto para almacenarlos como para consultarlos.

### 4.8.1. Database Diagram
Los diagramas de base de datos muestran la organización interna y las conexiones entre las entidades, facilitando la comprensión de cómo se guardan y vinculan los datos dentro del sistema de forma óptima.

![diagram](/assets/images/chapter-IV/data-base-diagram.png)
