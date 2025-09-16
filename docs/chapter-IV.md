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


#### Landing Page



##### Principios aplicados:






### 4.2.3. SEO Tags and Meta Tags

#### Landing Page



### 4.2.4. Searching Systems

#### **Landing Page**



#### **Web Application**

### 4.2.5. Navigation Systems

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



### 4.6.1. Software Architecture Context Diagram


### 4.6.2. Software Architecture Container Diagrams



### 4.6.3. Software Architecture Components Diagrams




## 4.7. Software Object-Oriented Design
En la sección de Software Object-Oriented Design se presentarán del diagrama de clases de la aplicaion.

### 4.7.1. Class Diagrams



## 4.8. Database Design
En la parte dedicada al Diseño de la Base de Datos, se mostrará un diagrama que ilustra cómo están organizadas las entidades y sus vínculos, facilitando un manejo eficiente de los datos tanto para almacenarlos como para consultarlos.

### 4.8.1. Database Diagram
Los diagramas de base de datos muestran la organización interna y las conexiones entre las entidades, facilitando la comprensión de cómo se guardan y vinculan los datos dentro del sistema de forma óptima.


