<div align="center">
  

![UPC_logo_transparente](/assets/images/chapter-I/upc_logo.png)

# UNIVERSIDAD PERUANA DE CIENCIAS APLICADAS
# Facultad: Ingeniería
# Carrera: Ingeniería de Software
# Periodo 2520
# Código del curso: 1ASI0729 
# Nombre del curso: Desarrollo de Aplicaciones Open Source
# NRC: 7351
# Nombre del profesor: Rafael Oswaldo Castro Veramendi

# Informe de Trabajo Final
### Nombre del startup: QuickPark
### Nombre del producto: EasyPark
### Relación de integrantes:


|       Apellidos y Nombres        |     Código      |
|----------------------------------|-----------------|
| Elescano Leon, Piero Hugo        |   u202313354    |
| Florez Shimabukuro, Fátima Belén |   u202320610    |
| Espinoza Chávez, Moisés Filemón  |   u202221383    |
| Paredes Davila, Jose Adrian      |   u202216163    |
| Nakasone Gomes, Marco Antonio    |   u202210790    |

### **Diciembre, 2025**
</div>

# **Registro de Versiones Del Informe**

| Versión | Fecha       | Autor                                | Descripción de Modificación                                           |
|---------|-------------|--------------------------------------|------------------------------------------------------------------------|
| 0.0     | 02/09/2025  | Elescano Leon, Piero Hugo            | Se crea la estructura inicial del documento de EasyPark.               |
| 1.0     | 03/09/2025  | Elescano Leon, Piero Hugo            | Se crean las ramas principales y se organiza el repositorio.           |
| 1.1     | 04/09/2025  | Florez Shimabukuro, Fátima Belén     | Avances en Capítulo I: Introducción y perfiles de integrantes.         |
| 1.2     | 05/09/2025  | Florez Shimabukuro, Fátima Belén; Nakasone Gomes, Marco Antonio | Desarrollo de la sección Lean UX Process y primeros wireframes.        |
| 1.3     | 06/09/2025  | Espinoza Chávez, Moisés Filemón      | Se agregan user personas y matriz de tareas de usuario.                |
| 1.4     | 08/09/2025  | Elescano Leon, Piero Hugo; Nakasone Gomes, Marco Antonio | Actualización de User Stories y Product Backlog.                       |
| 1.5     | 09/09/2025  | Florez Shimabukuro, Fátima Belén     | Desarrollo de la arquitectura de información y guidelines de estilo.   |
| 1.6     | 11/09/2025  | Paredes Davila, Jose Adrian          | Revisión y ajustes menores en entrevistas y event storming.            |
| 1.7     | 12/09/2025  | Nakasone Gomes, Marco Antonio        | Revisión general y aportes en documentación de anexos.                 |
| 1.8     | 14/09/2025  | Elescano Leon, Piero Hugo            | Integración y revisión de la landing page (estructura y secciones).    |
| 1.9     | 15/09/2025  | Florez Shimabukuro, Fátima Belén; Nakasone Gomes, Marco Antonio | Mejoras visuales y de accesibilidad en la landing page.                |
| 2.0     | 16/09/2025  | Elescano Leon, Piero Hugo            | Revisión y actualización final del Capítulo IV: Product Design.        |
| 2.1     | 16/09/2025  | Espinoza Chávez, Moisés Filemón      | Corrección en los impact mapping y user journey.                       |
| 2.2     | 17/09/2025  | Florez Shimabukuro, Fátima Belén     | Documentación de evidencias de desarrollo de la landing page.          |
| 2.3     | 18/09/2025  | Elescano Leon, Piero Hugo            | Ajustes finales en conclusiones y organización de entregables.         |
| 2.4     | 20/09/2025  | Elescano Leon, Piero Hugo; Florez Shimabukuro, Fátima Belén | Inicio de Sprint 2: Configuración y primeros avances para el despliegue del frontend en Netlify. |
| 2.5     | 23/09/2025  | Elescano Leon, Piero Hugo                                   | Implementación de la estructura principal del frontend, integración con DB JSON en Kobey.        |
| 2.6     | 26/09/2025  | Florez Shimabukuro, Fátima Belén                            | Desarrollo de vistas principales y revisión de estilos visuales para la web app.                 |
| 2.7     | 29/09/2025  | Elescano Leon, Piero Hugo; Espinoza Chávez, Moisés Filemón  | Ajustes en la integración del frontend con la base de datos y solución de bugs iniciales.        |
| 2.8     | 02/10/2025  | Espinoza Chávez, Moisés Filemón                             | Validación de funcionalidades y revisión colaborativa de la experiencia de usuario.              |
| 2.9     | 05/10/2025  | Florez Shimabukuro, Fátima Belén                            | Documentación de evidencias del despliegue en Netlify y mejoras en la interacción.               |
| 3.0     | 08/10/2025  | Elescano Leon, Piero Hugo            | Cierre de Sprint 2: Despliegue exitoso de la primera versión de la aplicación web frontend.      |
| 3.1     | 05/11/2025  | Elescano Leon, Piero Hugo; Nakasone Gomes, Marco Antonio   | Actualización del frontend: refactor de componentes, mejoras de accesibilidad y rendimiento. Migración desde una fake API a una API REST; adaptación de llamadas y documentación técnica. |
| 3.2     | 14/11/2025  | Elescano Leon, Piero Hugo; Espinoza Chávez, Moisés Filemón; Florez Shimabukuro, Fátima Belén; Nakasone Gomes, Marco Antonio | Despliegue del frontend en Render, ajustes de configuración para producción, actualización de la documentación del despliegue y correcciones menores. Se actualiza la lista de integrantes en el README. |
| 3.3     | 27/11/2025  | Elescano Leon, Piero Hugo; Florez Shimabukuro, Fátima Belén; Espinoza Chávez, Moisés Filemón; Nakasone Gomes, Marco Antonio | Cierre del Sprint 4: finalización de tareas planificadas, revisión de objetivos, resolución de incidencias, pruebas finales y retrospectiva. |
| 3.4     | 28/11/2025  | Elescano Leon, Piero Hugo; Florez Shimabukuro, Fátima Belén; Espinoza Chávez, Moisés Filemón; Nakasone Gomes, Marco Antonio | Despliegue final - Frontend: despliegue a producción con configuración de hosting, CI/CD, certificados HTTPS, gestión de variables de entorno y verificación de rutas, assets y rendimiento. |
| 3.5     | 29/11/2025  | Elescano Leon, Piero Hugo; Florez Shimabukuro, Fátima Belén; Espinoza Chávez, Moisés Filemón; Nakasone Gomes, Marco Antonio | Despliegue final - Backend: despliegue a producción, migraciones y verificación de base de datos, configuración de entornos y secretos, monitoreo inicial, y pruebas de integración end-to-end. |

# Project Report Collaboration Insights 
Se presenta el reporte de colaboracion por miembro del equipo

![UPC](/assets/images/chapter-I/report-commits.png)


  - **Link del repositorio:** https://github.com/Aplicaciones-Open-Source-Grupo-3/Final-Report.git
  
  - **Link de Landing Page:** https://aplicaciones-open-source-grupo-3.github.io/Landing-Page/

  - **Link de la aplicacion web:** https://easypark24.netlify.app/

  - **Link del backend:** https://easypark-platform.onrender.com/swagger-ui/index.html
    
# Student Outcome

Criterio: Capacidad de comunicarse efectivamente con un rango de audiencias. 

En el siguiente cuadro se detallan las acciones realizadas y las conclusiones alcanzadas por el equipo de trabajo, las cuales evidencian el cumplimiento del logro correspondiente al ABET – EAC - Student Outcome 3.


<table>
  <tr>
    <th>Criterio Específico</th>
    <th>Acciones Realizadas</th>
    <th>Conclusiones</th>
  </tr>
  <tr>
    <td rowspan="4">Comunica oralmente con efectividad a diferentes rangos de audiencia</td>
    <td>Elescano Leon, Piero Hugo:<br>TB1: Expuso con claridad las ideas y avances sobre la estructuración y diseño de la landing page durante las reuniones de equipo, asegurando la comprensión de todos y promoviendo la toma de decisiones conjunta.<br><br>TP1: Presentó ante el equipo la nueva versión del Landing Page, explicando con claridad los cambios aplicados respecto al Sprint anterior, la mejora en la estructura de componentes y la organización del código según los principios de diseño y buenas prácticas. Además, explicó la integración del backend simulado con JSON Server.<br><br>TB2: Expuso el refactor del frontend, demostró la integración con la API REST y realizó la presentación del sitio desplegado en Render, respondiendo preguntas técnicas del equipo y coordinando pruebas en entorno de producción.</td> 
    <td rowspan="4">TB1: La comunicación oral efectiva dentro del equipo facilitó la comprensión de ideas, permitió la resolución rápida de dudas y contribuyó a una mejor coordinación en el desarrollo de la landing page, adaptándose al nivel de conocimiento de cada miembro.<br><br>TP1: El equipo demostró una comunicación oral clara y efectiva al exponer los avances del Sprint 2, explicar decisiones técnicas y presentar el Landing Page y la Web App. Cada integrante mostró dominio del contenido y capacidad para adaptar su discurso según la audiencia, evidenciando trabajo colaborativo y seguridad en sus presentaciones.<br><br>TB2: Las presentaciones y demos orales sobre la migración a API REST y el despliegue en Render facilitaron la comprensión técnica del proceso, permitieron una coordinación efectiva para la puesta en producción y agilizaron la resolución de incidencias durante y después del despliegue.</td>
  </tr> 
  <tr>
    <td><br>Florez Shimabukuro, Fátima Belén:<br>TB1: Participó activamente en las presentaciones internas, explicando el enfoque visual y la experiencia de usuario de la landing page de manera accesible para todos los integrantes y ajustando su mensaje según la audiencia.<br><br>TP1: Expuso las funcionalidades principales de la primera versión del Frontend Web Application, explicando el flujo de navegación, el uso de componentes reutilizables y la interacción del JSON Server. Durante la revisión del sprint, comunicó el enfoque del diseño y la aplicación de los principios de Single Page Application (SPA).<br><br>TB2: Realizó el walkthrough de los cambios de interfaz, explicó las mejoras de accesibilidad implementadas y justificó decisiones de diseño ante el equipo y stakeholders durante la demo del sitio en Render.</td>
  </tr>
  <tr>
    <td><br>Espinoza Chávez, Moisés Filemón:<br>TB1: Lideró sesiones de retroalimentación presentando los avances en la integración de contenidos y funcionalidades, utilizando un lenguaje claro y estructurado para asegurar el entendimiento de todo el equipo.<br><br>TP1: Comunicó los resultados del proceso de validación interna del Frontend y del Landing Page. Explicó los hallazgos encontrados al probar las interfaces y justificó las correcciones aplicadas en base a observaciones del Sprint anterior. Evidenció comprensión del flujo funcional del sistema y la importancia de la mejora continua en el desarrollo web.<br><br>TB2: Explicó el contrato de la nueva API REST, mostró ejemplos de llamadas y evidencias de pruebas funcionales durante la sesión de revisión, aclarando el impacto de los cambios en las integraciones del frontend.</td>
  </tr>
  <tr>
    <td><br>Nakasone Gomes, Marco Antonio:<br>TB1: Moderó discusiones del grupo sobre el diseño y la estructura, comunicando de manera efectiva las conclusiones y próximos pasos, manteniendo un ambiente participativo y claro.<br><br>TP1: Explicó la planificación del sprint, los objetivos del incremento y la distribución de roles en el equipo, mostrando seguridad y claridad. También presentó los principales avances del proyecto en el Stage Review, utilizando un lenguaje adecuado.<br><br>TB2: Coordinó y explicó el proceso de despliegue en Render, la configuración de entorno, estrategias de rollback y monitoreo, y lideró la comunicación técnica con el equipo durante la puesta en producción.</td>
  </tr>
  <tr>
    <td rowspan="4">Comunica por escrito con efectividad a diferentes rangos de audiencia</td>
    <td><br> Elescano Leon, Piero Hugo:<br>TB1: Redactó reportes de avance sobre el desarrollo de la landing page, utilizando un lenguaje técnico adecuado para el público objetivo, lo cual facilitó el seguimiento del progreso del equipo.<br><br>TP1: Documentó en el informe final las modificaciones aplicadas al Landing Page, indicando versión, fecha, responsables y justificación de cada cambio en el Registro de Versiones. Detalló las mejoras implementadas, con capturas de pantalla y fragmentos de código, y actualizó la sección de Servicios y Despliegue, mostrando la URL del sitio publicado.<br><br>TB2: Documentó las modificaciones del frontend, actualizó la guía de consumo de la API REST (endpoints, ejemplos y notas de integración) y registró los pasos de despliegue y configuración para Render en el repositorio.</td>
    <td rowspan="4">TB1: La comunicación escrita efectiva permitió documentar adecuadamente el desarrollo de la landing page, compartir información relevante con precisión y mantener informados a todos los interesados, adaptando el contenido y el nivel de detalle según la audiencia.<br><br>TP1: Se evidenció una comunicación escrita técnica y coherente en la documentación. Los integrantes redactaron informes, registros y evidencias con claridad, aplicando buenas prácticas, gramática adecuada y lenguaje profesional. La actualización de artefactos y reportes reflejó mejora continua y compromiso con la calidad del proyecto.<br><br>TB2: La documentación escrita (guías de migración, especificaciones de API y procedimientos de despliegue) permitió transferir conocimiento al equipo, reducir errores en la integración y facilitar la reproducibilidad y mantenimiento del entorno de producción.</td>
  </tr>
  <tr>
    <td><br> Florez Shimabukuro, Fátima Belén:<br>TB1: Elaboró documentos que describían las decisiones de diseño visual y experiencia de usuario, asegurándose de que fueran comprensibles tanto para el equipo como para los asesores externos.<br><br>TP1: Describió la arquitectura del Frontend, detallando la estructura de carpetas, la conexión con el servidor simulado y el uso de Angular. Mantuvo el control de versiones con GitFlow, registrando commits descriptivos y actualizando el Sprint Backlog con evidencia de tareas completadas. Redactó con claridad técnica y siguiendo las convenciones del proyecto.<br><br>TB2: Redactó las decisiones de diseño y los cambios en accesibilidad tras la migración, incluyendo ejemplos visuales y comparativos frente a la versión anterior para facilitar la comprensión y revisión.</td>
  </tr>
  <tr>
    <td><br> Espinoza Chávez, Moisés Filemón:<br>TB1: Participó en la redacción de la documentación del proyecto, estructurando los contenidos de manera lógica y clara para facilitar su entendimiento por distintas audiencias.<br><br>TP1: Actualizó las versiones corregidas de artefactos previos reflejando los cambios aplicados en el Sprint 2. Además, documentó en el Project Collaboration Insights cómo las actividades del equipo fueron implementadas. La redacción mostró orden y precisión.<br><br>TB2: Elaboró la especificación de la API REST (endpoints, parámetros, ejemplos de request/response) y preparó el registro de la migración desde la fake API, incluyendo pruebas y logs relevantes.</td>
  </tr>
  <tr>
    <td><br> Nakasone Gomes, Marco Antonio:<br>TB1: Coordinó la recopilación de reportes escritos y la organización de los entregables finales, asegurando la coherencia y claridad en los documentos generados por el equipo.<br><br>TP1: Elaboró y redactó las secciones de Sprint Planning 2, Aspect Leaders and Collaborators y Sprint Backlog 2 en el informe final. La escritura fue organizada, aplicando correctamente la estructura del documento académico y cuidando la gramática. Además, integró la conclusión general del TP1, resumiendo el progreso del proyecto y las perspectivas para el siguiente sprint.<br><br>TB2: Preparó la guía técnica de despliegue en Render, detallando variables de entorno, comandos de build, pasos para restaurar versiones anteriores y recomendaciones de monitoreo post-despliegue.</td>
  </tr>
</table>

# Contenido

## [Capítulo I: Introducción](/docs/chapter-I.md)
### [1.1. Startup Profile](/docs/chapter-I.md/#11-startup-profile)
  #### [1.1.1. Descripción de la Startup](/docs/chapter-I.md/#111-descripción-de-la-startup)
  #### [1.1.2. Perfiles de integrantes del equipo](/docs/chapter-I.md/#112-perfiles-de-integrantes-del-equipo)
### [1.2. Solution Profile](/docs/chapter-I.md/#12-solution-profile)
  #### [1.2.1. Antecedentes y problemática](/docs/chapter-I.md/#121-antecedentes-y-problemática)
  #### [1.2.2. Lean UX Process](/docs/chapter-I.md/#122-lean-ux-process)
  ##### [1.2.2.1. Lean UX Problem Statements](/docs/chapter-I.md/#1221-lean-ux-problem-statements)
  ##### [1.2.2.2. Lean UX Assumptions](/docs/chapter-I.md/#1222-lean-ux-assumptions)
  ##### [1.2.2.3. Lean UX Hypothesis Statements](/docs/chapter-I.md/#1223-lean-ux-hypothesis-statements)
  ##### [1.2.2.4. Lean UX Canvas](/docs/chapter-I.md/#1224-lean-ux-canvas)
### [1.3. Segmentos objetivos](/docs/chapter-I.md/#13-segmentos-objetivos)

## [Capítulo II: Requirements Elicitation & Analysis](/docs/chapter-II.md)
### [2.1. Competidores](/docs/chapter-II.md/#21-competidores)
  #### [2.1.1. Análisis competitivo](/docs/chapter-II.md/#211-análisis-competitivo)
  #### [2.1.2. Estrategias y tácticas frente a competidores](/docs/chapter-II.md/#212-estrategias-y-tácticas-frente-a-competidores)
### [2.2. Entrevistas](/docs/chapter-II.md/#22-entrevistas)
  #### [2.2.1. Diseño de entrevistas](/docs/chapter-II.md/#221-diseño-de-entrevistas)
  #### [2.2.2. Registro de entrevistas](/docs/chapter-II.md/#222-registro-de-entrevistas)
  #### [2.2.3. Análisis de entrevistas](/docs/chapter-II.md/#223-análisis-de-entrevistas)
### [2.3. Needfinding](/docs/chapter-II.md/#23-need-finding)
  #### [2.3.1. User Personas](/docs/chapter-II.md/#231-user-personas)
  #### [2.3.2. User Task Matrix](/docs/chapter-II.md/#232-user-task-matrix)
  #### [2.3.3. User Journey Mapping](/docs/chapter-II.md/#233-user-journey-mapping)
  #### [2.3.4. Empathy Mapping](/docs/chapter-II.md/#234-empathy-mapping)
### [2.4. Big Picture Event Storming](/docs/chapter-II.md/#24-big-picture-event-storming)
### [2.5. Ubiquitous Language](/docs/chapter-II.md/#25-ubiquitous-language)

## [Capítulo III: Requirements Specification](/docs/chapter-III.md)
### [3.1. User Stories](/docs/chapter-III.md/#31-user-stories)
### [3.2. Impact Mapping](/docs/chapter-III.md/#32-impact-mapping)
### [3.3. Product Backlog](/docs/chapter-III.md/#33-product-backlog)
  
## [Capítulo IV: Product Design](/docs/chapter-IV.md)
### [4.1. Style Guidelines](/docs/chapter-IV.md/#41-style-guidelines)
  #### [4.1.1. General Style Guidelines](/docs/chapter-IV.md/#411-general-style-guidelines)
  #### [4.1.2. Web Style Guidelines](/docs/chapter-IV.md/#412-web-style-guidelines)
### [4.2. Information Architecture](/docs/chapter-IV.md/#42-information-architecture)
  #### [4.2.1. Organization Systems](/docs/chapter-IV.md/#421-organization-systems)
  #### [4.2.2. Labeling Systems](/docs/chapter-IV.md/#422-labeling-systems)
  #### [4.2.3. SEO Tags and Meta Tags](/docs/chapter-IV.md/#423-seo-tags-and-meta-tags)
  #### [4.2.4. Searching Systems](/docs/chapter-IV.md/#424-searching-systems)
  #### [4.2.5. Navigation Systems](/docs/chapter-IV.md/#425-navigation-systems)
### [4.3. Landing Page UI Design](/docs/chapter-IV.md/#43-landing-page-ui-design)
  #### [4.3.1. Landing Page Wireframe](/docs/chapter-IV.md/#431-landing-page-wireframe)
  #### [4.3.2. Landing Page Mock-up](/docs/chapter-IV.md/#432-landing-page-mock-up)
### [4.4. Web Applications UX/UI Design](/docs/chapter-IV.md/#44-web-applications-uxui-design)
  #### [4.4.1. Web Applications Wireframes](/docs/chapter-IV.md/#441-web-applications-wireframes)
  #### [4.4.2. Web Applications Wireflow Diagrams](/docs/chapter-IV.md/#442-web-applications-wireflow-diagrams)
  #### [4.4.3. Web Applications Mock-ups](/docs/chapter-IV.md/#443-web-applications-mock-ups)
  #### [4.4.4. Web Applications User Flow Diagrams](/docs/chapter-IV.md/#444-web-applications-user-flow-diagrams)
### [4.5. Web Applications Prototyping](/docs/chapter-IV.md/#45-web-applications-prototyping)
### [4.6. Domain-Driven Software Architecture](/docs/chapter-IV.md/#46-domain-driven-software-architecture)
  #### [4.6.1. Software Architecture Context Diagram](/docs/chapter-IV.md/#461-software-architecture-context-diagram)
  #### [4.6.2. Software Architecture Container Diagrams](/docs/chapter-IV.md/#462-software-architecture-container-diagrams)
  #### [4.6.3. Software Architecture Components Diagrams](/docs/chapter-IV.md/#463-software-architecture-components-diagrams)
### [4.7. Software Object-Oriented Design](/docs/chapter-IV.md/#47-software-object-oriented-design)
  #### [4.7.1. Class Diagrams](/docs/chapter-IV.md/#471-class-diagrams)
### [4.8. Database Design](/docs/chapter-IV.md/#48-database-design)
  #### [4.8.1. Database Diagram](/docs/chapter-IV.md/#481-database-diagram)
  
## [Capítulo V: Product Implementation, Validation & Deployment](/docs/chapter-V.md)
### [5.1. Software Configuration Management](/docs/chapter-V.md/#51-software-configuration-management)
#### [5.1.1. Software Development Environment Configuration](/docs/chapter-V.md/#511-software-development-environment)
#### [5.1.2. Source Code Management](/docs/chapter-V.md/#512-source-code-management)
#### [5.1.3. Source Code Style Guide & Conventions](/docs/chapter-V.md/#513-source-code-style-guide-&-conventions)
#### [5.1.4. Software Deployment Configuration](/docs/chapter-V.md/#514-software-deployment-configuration)

### [5.2. Landing Page, Services & Applications Implementation](/docs/chapter-V.md/#52-landing-page-services-&-applications-implementation)
#### [5.2.1. Sprint 1](/docs/chapter-V.md/#521-sprint-1)
##### [5.2.1.1. Sprint Planning 1](/docs/chapter-V.md/#5211-sprint-planning-1)
##### [5.2.1.2. Aspect Leaders and Collaborators](/docs/chapter-V.md/#5212-aspect-leaders-and-collaborators)
##### [5.2.1.3. Sprint Backlog 1](/docs/chapter-V.md/#5213-sprint-backlog-1)
##### [5.2.1.4. Development Evidence for Sprint Review](/docs/chapter-V.md/#5214-development-evidence-for-sprint-review)
##### [5.2.1.5. Execution Evidence for Sprint Review](/docs/chapter-V.md/#5215-execution-evidence-for-sprint-review)
##### [5.2.1.6. Services Documentation Evidence for Sprint Review](/docs/chapter-V.md/#5216-services-documentation-evidence-for-sprint-review)
##### [5.2.1.7. Software Deployment Evidence for Sprint Review](/docs/chapter-V.md/#[5217-software-deployment-evidence-for-sprint-review)
##### [5.2.1.8. Team Collaboration Insights during Sprint](/docs/chapter-V.md/#5218-team-collaboration-insights-during-sprint)

#### [5.2.2. Sprint 2](/docs/chapter-V.md/#522-sprint-2)
##### [5.2.2.1. Sprint Planning 2](/docs/chapter-V.md/#5221-sprint-planning-2)
##### [5.2.2.2. Aspect Leaders and Collaborators](/docs/chapter-V.md/#5222-aspect-leaders-and-collaborators)
##### [5.2.2.3. Sprint Backlog 2](/docs/chapter-V.md/#5223-sprint-backlog-2)
##### [5.2.2.4. Development Evidence for Sprint Review](/docs/chapter-V.md/#5224-development-evidence-for-sprint-review)
##### [5.2.2.5. Execution Evidence for Sprint Review](/docs/chapter-V.md/#5225-execution-evidence-for-sprint-review)
##### [5.2.2.6. Services Documentation Evidence for Sprint Review](/docs/chapter-V.md/#5226-services-documentation-evidence-for-sprint-review)
##### [5.2.2.7. Software Deployment Evidence for Sprint Review](/docs/chapter-V.md/#[5227-software-deployment-evidence-for-sprint-review)
##### [5.2.2.8. Team Collaboration Insights during Sprint](/docs/chapter-V.md/#5228-team-collaboration-insights-during-sprint)

#### [5.2.3. Sprint 3](/docs/chapter-V.md/#523-sprint-3)
##### [5.2.3.1. Sprint Planning 3](/docs/chapter-V.md/#5231-sprint-planning-3)
##### [5.2.3.2. Aspect Leaders and Collaborators](/docs/chapter-V.md/#5232-aspect-leaders-and-collaborators)
##### [5.2.3.3. Sprint Backlog 3](/docs/chapter-V.md/#5233-sprint-backlog-3)
##### [5.2.3.4. Development Evidence for Sprint Review](/docs/chapter-V.md/#5234-development-evidence-for-sprint-review)
##### [5.2.3.5. Execution Evidence for Sprint Review](/docs/chapter-V.md/#5235-execution-evidence-for-sprint-review)
##### [5.2.3.6. Services Documentation Evidence for Sprint Review](/docs/chapter-V.md/#5236-services-documentation-evidence-for-sprint-review)
##### [5.2.3.7. Software Deployment Evidence for Sprint Review](/docs/chapter-V.md/#5237-software-deployment-evidence-for-sprint-review)
##### [5.2.3.8. Team Collaboration Insights during Sprint](/docs/chapter-V.md/#5238-team-collaboration-insights-during-sprint)

#### [5.2.4. Sprint 4](/docs/chapter-V.md/#524-sprint-4)
##### [5.2.4.1. Sprint Planning 4](/docs/chapter-V.md/#5241-sprint-planning-4)
##### [5.2.4.2. Aspect Leaders and Collaborators](/docs/chapter-V.md/#5242-aspect-leaders-and-collaborators)
##### [5.2.4.3. Sprint Backlog 4](/docs/chapter-V.md/#5243-sprint-backlog-4)
##### [5.2.4.4. Development Evidence for Sprint Review](/docs/chapter-V.md/#5244-development-evidence-for-sprint-review)
##### [5.2.4.5. Execution Evidence for Sprint Review](/docs/chapter-V.md/#5245-execution-evidence-for-sprint-review)
##### [5.2.4.6. Services Documentation Evidence for Sprint Review](/docs/chapter-V.md/#5246-services-documentation-evidence-for-sprint-review)
##### [5.2.4.7. Software Deployment Evidence for Sprint Review](/docs/chapter-V.md/#5247-software-deployment-evidence-for-sprint-review)
##### [5.2.4.8. Team Collaboration Insights during Sprint](/docs/chapter-V.md/#5248-team-collaboration-insights-during-sprint)

### [5.3. Validation Interviews](/docs/chapter-V.md/#53-validation-interviews)
#### [5.3.1. Design Interviews](/docs/chapter-V.md/#531-design-interviews)
#### [5.3.2. Interview Record](/docs/chapter-V.md/#532-interview-record)
#### [5.3.3. Evaluation based on heuristics](/docs/chapter-V.md/#533-evaluation-based-on-heuristics)

### [5.4. Video About the Product](/docs/chapter-V.md/#54-video-about-the-product)

## [Conclusiones](/docs/conclusions.md)

## [Bibliografía](/docs/bibliography.md)

## [Anexos](/docs/annexes.md)
