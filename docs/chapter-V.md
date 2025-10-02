# Capítulo V: Product Implementation, Validation & Deployment
## 5.1. Software Configuration Management.
A continuación se presenta la gestión centralizada y estructurada del repositorio como referencia fundamental para el desarrollo de EasyPark. Se describen las herramientas y metodologías que han permitido mantener coherencia, trazabilidad y calidad en todas las fases del ciclo de vida del software.

### 5.1.1. Software Development Environment Configuration.
Para construir EasyPark, se definió un entorno de desarrollo eficiente y colaborativo, alineado con las necesidades de una aplicación web de gestión de estacionamientos. Se emplearon las siguientes herramientas y plataformas:

- **WebStorm:** IDEs utilizados para desarrollo frontend.
- **Rider:** Para desarrollo backend, encargados de la lógica de negocio y servicios web.
- **Git:** Control de versiones local y coordinación de trabajo colaborativo.
- **GitHub:** Plataforma de gestión del repositorio central, issues, pull requests y documentación técnica.
- **Figma/Miro:** Diseño de interfaces, prototipos y colaboración UX/UI.

## Gestión del Proyecto

En EasyPark, la gestión del proyecto fue clave para coordinar actividades, tareas y equipos, asegurando el avance dentro de los plazos y objetivos definidos para transformar la gestión de estacionamientos en Lima.

**Modelo SaaS Web:**  
Se optó por una solución web en la nube, accesible vía navegador, que permite planificación, seguimiento y colaboración sin necesidad de instalaciones locales.
Durante el desarrollo, se utilizó una solución basada en la nube accesible vía navegador, permitiendo la planificación, seguimiento de tareas y colaboración, sin la necesidad de instalar la aplicaion en las computadoras de los usuarios.

## Gestión de Requisitos
El levantamiento y seguimiento de requisitos funcionales y no funcionales fue fundamental para garantizar que EasyPark respondiera a las necesidades de administradores y operadores de estacionamientos.

**Pivotal Tracker:**  
Gestión de historias de usuario, épicas, prioridades y seguimiento del flujo de trabajo ágil.
## Diseño UX/UI del Producto
EasyPark se diseñó con enfoque centrado en el usuario, garantizando una interfaz intuitiva y accesible desde todo tipo de dispositivos.
**Herramientas utilizadas:**
- **Figma:** Prototipos interactivos y diseño visual responsive.
- **Miro:** Mapas de empatía, user personas, customer journey maps y lluvias de ideas colaborativas.
- **Lucidchart:** Diagramas UML, arquitecturas y flujos operativos.
- **Overflow:** Visualización de flujos de usuario y recorridos críticos en la app.
## Desarrollo de Software
- **GitHub:** Repositorio central del código fuente y control de versiones de EasyPark.
- **Git:** Gestión de ramas, cambios y colaboración.
- **IDE (WebStorm/Rider):** Entornos de desarrollo adaptados a frontend y backend.
## Pruebas de Software
El objetivo de esta fase fue validar y verificar el correcto funcionamiento del sistema, asegurando confiabilidad en los procesos críticos de gestión de estacionamientos.

- **Lenguaje Gherkin:** Redacción de escenarios de usuario y automatización de pruebas basadas en comportamiento esperado.
- **Testing:** Cobertura de las funcionalidades clave como gestión de espacios, cobros, reportes y reservas.

## Documentación del Software
La documentación de EasyPark describe el funcionamiento del sistema tanto para usuarios finales como para el equipo técnico. Todo el material se integra en el repositorio y en la wiki de GitHub.

### 5.1.2. Source Code Management.
EasyPark implementa prácticas robustas para la gestión del código:

#### Plataforma de Control de Versiones

- **GitHub** es la plataforma centralizada para el control y seguimiento del código fuente. Se utiliza un único repositorio principal, con ramas y flujos dedicados para cada componente: backend, frontend y landing page.

#### Flujo de Trabajo Git (GitFlow)

Se adoptó **GitFlow** para mantener orden y facilitar la colaboración:

- **Ramas principales:**
  - `main`: Versión estable y lista para producción de EasyPark.
  - `develop`: Integración y pruebas previas a lanzamientos.
- **Ramas de apoyo:**
  - `feature`: Funcionalidades nuevas.
  - `release`: Preparación de nuevas versiones estables.
  - `hotfix`: Corrección de errores críticos en producción.

#### Versionado Semántico (Semantic Versioning)

EasyPark sigue el estándar **Semantic Versioning 2.0.0** (`X.Y.Z`):

- `X`: Cambios incompatibles.
- `Y`: Nuevas funcionalidades compatibles.
- `Z`: Parches y correcciones menores.

#### Commits Convencionales (Conventional Commits)

Para asegurar trazabilidad y claridad:

```
<type>[opcional scope]: <descripción>
[optional body]
[optional footer]
```

- `feat`: Nueva funcionalidad.
- `fix`: Corrección de errores.
- `docs`: Documentación.
- `refactor`, `perf`, `chore`, `build`.

Este enfoque facilita la automatización, el versionado y la revisión colaborativa.

### 5.1.3. Source Code Style Guide & Conventions.
En esta parte del proyecto, se centra en definir un conjunto uniforme de normas y convenciones de estilo y programación para el desarrollo de nuestra aplicación web EasyPark. Estas pautas son fundamentales para asegurar que el código sea consistente, claro y bien estructurado, lo que a su vez facilitará su mantenimiento y escalabilidad durante todo el ciclo de vida del proyecto.

EasyPark mantiene un conjunto uniforme de normas para HTML, CSS y JavaScript, asegurando consistencia y calidad:

#### HTML
- Uso de `<!DOCTYPE html>`, etiquetas en minúsculas, atributos entre comillas dobles.
- Comentarios claros y estructura semántica.
- Recursos enlazados correctamente.

#### CSS
- Nombres de clases/IDs en inglés y formato kebab-case.
- Uso correcto de llaves, punto y coma, y media queries para responsive design.

#### JavaScript
- `const` y `let` para variables, sin `var`.
- Funciones claras y con propósito único.
- Delegación de eventos y uso de listeners.

### 5.1.4. Software Deployment Configuration.

El despliegue de EasyPark cubre tres componentes: Landing Page, Backend y Frontend.

#### Landing Page

Se utiliza **GitHub Pages** para el despliegue, permitiendo acceso público sencillo y actualizaciones rápidas. El proceso incluye:

1. Selección de rama a desplegar desde Settings -> Pages en GitHub.
2. Espera de propagación y verificación del enlace de acceso.

#### Backend y Frontend

- Despliegue en servidores en la nube (Azure, AWS, Vercel, etc.) o contenedores Docker, según el entorno de producción requerido.
- Integración continua con GitHub Actions para automatizar pruebas y despliegues.
  
## 5.2. Landing Page, Services & Applications Implementation.
Esta sección detalla el proceso de desarrollo, pruebas, documentación y despliegue de la Landing Page, servicios web y aplicaciones frontend de EasyPark.

### 5.2.1. Sprint 1
Se documenta el trabajo colaborativo y las fases clave del Sprint 1, desde el sprint planning, desarrollo incremental y retrospectiva, alineados con los objetivos de digitalización y optimización de la gestión de estacionamientos.

#### 5.2.1.1. Sprint Planning 1.
Aquí se especifican los objetivos, historias de usuario priorizadas y entregables mínimos viables definidos para la primera iteración de EasyPark.

<table>
	<tbody>
		<tr>
			<td><strong>Sprint #</strong></td>
			<td>Sprint 1</td>
		</tr>
		<tr>
			<td colspan="2"><strong>Spring Planning Background</strong></td>
		</tr>
		<tr>
			<td><strong>Date</strong></td>
			<td>2025-09-3</td>
		</tr>
		<tr>
			<td><strong>Time</strong></td>
			<td>10:30 PM</td>
		</tr>
		<tr>
			<td><strong>Location</strong></td>
			<td>Remote mode through the GitHub platform</td>
		</tr>
		<tr>
			<td colspan="2"><strong>Prepared by</strong></td>
		</tr>
		<tr>
			<td><strong>Attendees (to planinning meeting)</strong></td>
			<td>All members of EasyPark</td>
		</tr>
		<tr>
			<td><strong>Sprint 0 Review Summary</strong></td>
			<td>Since this is our initial development sprint, a sprint summary has not yet been completed.</td>
		</tr>
		<tr>
			<td><strong>Sprint 0 Retrospective Summary</strong></td>
			<td>Since this is our initial development sprint, a sprint summary has not yet been completed.</td>
		</tr>
		<tr>
			<td colspan="2"><strong>Sprint Goal & User Stories</strong></td>
		</tr>
		<tr>
			<td><strong>Sprint 1 Goal</strong></td>
			<td>We are focused on building the EasyPark landing page, as we believe this is critical for the long-term sustainability of the product within the organization. We will confirm its success when we see a significant increase in user engagement.</td>
		</tr>
		<tr>
			<td><strong>Sprint 1 Velocity</strong></td>
			<td>10</td>
		</tr>
		<tr>
			<td><strong>Sum of Story points</strong></td>
			<td>18</td>
		</tr>
	</tbody>
</table>

#### 5.2.1.2. Aspect Leaders and Collaborators.
En esta sección se presenta la elaboración de el artefacto Leadership-andCollaboration Matrix (LACX), el cual se presenta al líder y los colaboradores de este Sprint 1.

| Team Member (Last Name, First Name) | GitHub Username | Landing page |
| ------------------------------------|-----------------|-------------------------------------------|
| Elescano Leon, Piero Hugo | PieroHugo | L |
| Espinoza Chavez, Moises Filemon |MoisesECh| C | 
| Florez Shimabukuro, Fátima Belén |PengwinKingdom| C |
| Nakasone Gomes, Marco Antonio  | marquinho04 | C | 
| Paredes Davila, Jose Adrian  | joseadro09 | C | 


#### 5.2.1.3. Sprint Backlog 1
El principal objetivo del primer sprint es desarrollar las funciones esenciales que permitan a los usuarios interesados en EasyPark informarse sobre su propósito, conocer sus características destacadas y entender las acciones que podrán realizar dentro de la aplicacion web.

<table>
  <tr>
    <td><strong>Sprint #</strong></td>
    <td colspan="7">Sprint 1</td>
  </tr>
  <tr>
    <td colspan="2"><strong>User Story</strong></td>
    <td colspan="6"><strong>Work-item / Task</strong></td>
  </tr>
  <tr>
    <td><strong>Id</strong></td>
    <td><strong>Title</strong></td>
    <td><strong>Id</strong></td>
    <td><strong>Title</strong></td>
    <td><strong>Description</strong></td>
    <td><strong>Estimation (Hours)</strong></td>
    <td><strong>Assigned To</strong></td>
    <td><strong>Status (To-do / In-Process / To-review / Done)</strong></td>
  </tr>

  <!-- EP05-US01 Información general EasyPark -->
  <tr>
    <td rowspan="2">EP05-US01</td>
    <td rowspan="2">Información general EasyPark</td>
    <td>T1</td>
    <td>Redactar descripción de EasyPark</td>
    <td>Redactar una descripción clara y concisa sobre EasyPark para la landing page.</td>
    <td>1</td>
    <td>Piero Elescano</td>
    <td>Done</td>
  </tr>
  <tr>
    <td>T2</td>
    <td>Agregar sección de información general</td>
    <td>Implementar la sección en el HTML y aplicar estilos.</td>
    <td>1</td>
    <td>Moises Espinoza</td>
    <td>Done</td>
  </tr>

  <!-- EP05-US02 Características destacadas -->
  <tr>
    <td rowspan="2">EP05-US02</td>
    <td rowspan="2">Características destacadas</td>
    <td>T3</td>
    <td>Listar beneficios y características</td>
    <td>Definir y listar los beneficios y características clave del sistema.</td>
    <td>0.5</td>
    <td>Fátima Florez</td>
    <td>Done</td>
  </tr>
  <tr>
    <td>T4</td>
    <td>Diseño sección de beneficios</td>
    <td>Agregar y estilizar la sección de características en la landing.</td>
    <td>1</td>
    <td>Moises Espinoza</td>
    <td>Done</td>
  </tr>

  <!-- EP05-US03 Planes y precios -->
  <tr>
    <td rowspan="2">EP05-US03</td>
    <td rowspan="2">Planes y precios</td>
    <td>T5</td>
    <td>Definir estructura de planes</td>
    <td>Redactar planes y precios ofrecidos por EasyPark.</td>
    <td>0.5</td>
    <td>Fátima Florez</td>
    <td>Done</td>
  </tr>
  <tr>
    <td>T6</td>
    <td>Implementar sección de planes y precios</td>
    <td>Maquetar e implementar la sección en la landing page.</td>
    <td>1</td>
    <td>Marco Nakasone</td>
    <td>Done</td>
  </tr>

  <!-- EP05-US04 Formulario de contacto -->
  <tr>
    <td rowspan="2">EP05-US04</td>
    <td rowspan="2">Formulario de contacto</td>
    <td>T7</td>
    <td>Diseñar formulario de contacto</td>
    <td>Diseñar y prototipar el formulario de contacto.</td>
    <td>0.5</td>
    <td>Fátima Florez</td>
    <td>Done</td>
  </tr>
  <tr>
    <td>T8</td>
    <td>Implementar funcionalidad del formulario</td>
    <td>Hacer funcional el formulario, validación y almacenamiento.</td>
    <td>1</td>
    <td>Piero Elescano</td>
    <td>Done</td>
  </tr>

  <!-- EP05-US05 Testimonios de clientes -->
  <tr>
    <td rowspan="2">EP05-US05</td>
    <td rowspan="2">Testimonios de clientes</td>
    <td>T9</td>
    <td>Recolectar testimonios/entrevistas</td>
    <td>Solicitar y redactar testimonios de clientes reales.</td>
    <td>0.5</td>
    <td>Jose Paredes</td>
    <td>Done</td>
  </tr>
  <tr>
    <td>T10</td>
    <td>Analizar las entrevistas</td>
    <td>Analisis de la informacion recolectada.</td>
    <td>1</td>
    <td>Moises Espinoza</td>
    <td>Done</td>
  </tr>

  <!-- EP05-US08 Enlaces a redes sociales -->
  <tr>
    <td>EP05-US08</td>
    <td>Enlaces a redes sociales</td>
    <td>T11</td>
    <td>Agregar enlaces a redes sociales</td>
    <td>Colocar íconos y enlaces a redes sociales oficiales en la landing.</td>
    <td>0.5</td>
    <td>Jose Paredes</td>
    <td>Done</td>
  </tr>

  <!-- EP05-US10 Accesibilidad y responsive -->
  <tr>
    <td rowspan="2">EP05-US10</td>
    <td rowspan="2">Accesibilidad y responsive</td>
    <td>T12</td>
    <td>Garantizar responsive design</td>
    <td>Aplicar media queries y pruebas en diferentes dispositivos.</td>
    <td>1</td>
    <td>Piero Elescano</td>
    <td>Done</td>
  </tr>
  <tr>
    <td>T13</td>
    <td>Test de accesibilidad</td>
    <td>Verificar el cumplimiento de estándares básicos de accesibilidad.</td>
    <td>1</td>
    <td>Fátima Florez</td>
    <td>Done</td>
  </tr>

  <!-- EP05-US19 Visualización de tarifas -->
  <tr>
    <td rowspan="2">EP05-US19</td>
    <td rowspan="2">Visualización de tarifas</td>
    <td>T14</td>
    <td>Redactar información de tarifas</td>
    <td>Redactar y actualizar la información sobre las tarifas del servicio EasyPark para la landing.</td>
    <td>0.5</td>
    <td>Marco Nakasone</td>
    <td>Done</td>
  </tr>
  <tr>
    <td>T15</td>
    <td>Agregar sección de tarifas en la landing</td>
    <td>Diseñar y maquetar la sección de tarifas, asegurando claridad y visibilidad.</td>
    <td>1</td>
    <td>Moises Espinoza</td>
    <td>Done</td>
  </tr>

  <!-- NUEVA SECCIÓN: EP05-US21 Recepción de notificaciones -->
  <tr>
    <td rowspan="2">EP05-US21</td>
    <td rowspan="2">Recepción de notificaciones</td>
    <td>T16</td>
    <td>Redactar beneficios de notificaciones</td>
    <td>Redactar una breve descripción sobre las ventajas de las notificaciones en EasyPark.</td>
    <td>0.5</td>
    <td>Fátima Florez</td>
    <td>Done</td>
  </tr>
  <tr>
    <td>T17</td>
    <td>Maquetar sección de notificaciones en la landing</td>
    <td>Diseñar y agregar la sección de notificaciones a la landing page.</td>
    <td>1</td>
    <td>Marco Nakasone</td>
    <td>Done</td>
  </tr>
</table>

#### 5.2.1.4. Development Evidence for Sprint Review
Para el Sprint 1, se presenta la evidencia de desarrollo de la landing page de EasyPark. Los commits registrados en el repositorio corresponden a la implementación de las secciones clave de la página. Esto se realizó siguiendo el diseño previo en Figma.

| Repository                        | Branch                  | Commit Message                                 | Commited on  |
|------------------------------------|-------------------------|------------------------------------------------|--------------|
| PieroHugo/Landing-Page             | main                    | initial commit                                 | 10/09/2025   |
| PieroHugo/Landing-Page             | develop                 | initial commit                                 | 10/09/2025   |
| PieroHugo/Landing-Page             | feature/structure-landing | feat: add landing page structure               | 11/09/2025   |
| PieroHugo/Landing-Page             | feature/structure-landing | feat: implement info section, styles           | 12/09/2025   |
| PieroHugo/Landing-Page             | feature/structure-landing | feat: add responsive and accessibility         | 13/09/2025   |
| PieroHugo/Landing-Page             | feature/structure-landing | fix: update content and images                 | 14/09/2025   |
| PieroHugo/Landing-Page             | feature/structure-landing | docs: add README with usage                    | 15/09/2025   |
| PieroHugo/Landing-Page             | feature/structure-landing | chore: minor refactor                          | 16/09/2025   |
| MoisesECh/Landing-Page             | feature/structure-landing | feat: benefits & features section              | 12/09/2025   |
| MoisesECh/Landing-Page             | feature/structure-landing | feat: add testimonials section                 | 13/09/2025   |
| MoisesECh/Landing-Page             | feature/structure-landing | fix: section layout and css improvements       | 14/09/2025   |
| MoisesECh/Landing-Page             | feature/structure-landing | feat: implement notification section           | 15/09/2025   |
| PengwinKingdom/Landing-Page        | feature/structure-landing | feat: add features list to landing             | 12/09/2025   |
| PengwinKingdom/Landing-Page        | feature/structure-landing | feat: add plans & pricing section              | 13/09/2025   |
| PengwinKingdom/Landing-Page        | feature/structure-landing | fix: improve form validation                   | 14/09/2025   |
| PengwinKingdom/Landing-Page        | feature/structure-landing | feat: add notification advantages section      | 15/09/2025   |
| marquinho04/Landing-Page           | feature/structure-landing | feat: add plans & pricing markup               | 13/09/2025   |
| marquinho04/Landing-Page           | feature/structure-landing | feat: FAQ & notification sections              | 14/09/2025   |
| marquinho04/Landing-Page           | feature/structure-landing | fix: responsive grid for landing               | 16/09/2025   |
| joseadro09/Landing-Page            | feature/structure-landing | feat: collect and add testimonials             | 13/09/2025   |
| joseadro09/Landing-Page            | feature/structure-landing | feat: add social media links section           | 14/09/2025   |
| joseadro09/Landing-Page            | feature/structure-landing | fix: improve testimonials style and markup     | 16/09/2025   |

#### 5.2.1.5. Execution Evidence for Sprint Review.

El equipo de desarrolladores logró concluir con el sprint 1, el cual involucra la implementación y despliegue de la landing page de EasyPark. A continuación se presentan las evidencias.
#### Landing page desplegada
![landing img](/assets/images/chapter-V/EasyPark-landing-deploy-1.png)

![landing img](/assets/images/chapter-V/EasyPark-landing-deploy-2.png)

![landing img](/assets/images/chapter-V/EasyPark-landing-deploy-3.png)

![landing img](/assets/images/chapter-V/EasyPark-landing-deploy-4.png)

![landing img](/assets/images/chapter-V/EasyPark-landing-deploy-5.png)

#### 5.2.1.6. Services Documentation Evidence for Sprint Review.

En este sprint no se cuenta la documentacion a razón que el primer sprint esta dirigido a la elaboración del landing page.

#### 5.2.1.7. Software Deployment Evidence for Sprint Review
En el desarrollo del Sprint 1 para EasyPark, se utilizó GitHub Pages para el despliegue de la página de aterrizaje. Esta herramienta se integró de manera fluida al flujo de trabajo, permitiendo el despliegue directo desde el repositorio. Además, se llevaron a cabo actividades específicas para preparar el entorno de despliegue.
#### Despliegue realizado en GitHub pages
![landing img](/assets/images/chapter-V/landing-page-deploy-evidence.jpg)

Enlace de la Landing Page: https://aplicaciones-open-source-grupo-3.github.io/Landing-Page/

![landing img](/assets/images/chapter-V/EasyPark-landing-deploy-1.png)

#### 5.2.1.8. Team Collaboration Insights during Sprint.
En esta seccion se evidencia el trabajo colaborativo del equipo de desarrollo de la primera parte del proyecto.

![landing img](/assets/images/chapter-I/Contributors.png)


### 5.2.2. Sprint 2
Se documenta el trabajo colaborativo y las fases clave del Sprint 2, desde el sprint planning, desarrollo incremental y retrospectiva. El Sprint 2 se enfoca en habilitar el pago end-to-end con pasarela sandbox, persistir transacciones y reflejarlas en un dashboard básico, alineado con la optimización de la gestión de estacionamientos.

#### 5.2.2.1. Sprint Planning 2.
Aquí se especifican los objetivos, historias de usuario priorizadas y entregables mínimos viables definidos para la segunda iteración de EasyPark.

<table>
	<tbody>
		<tr>
			<td><strong>Sprint #</strong></td>
			<td>Sprint 2</td>
		</tr>
		<tr>
			<td colspan="2"><strong>Spring Planning Background</strong></td>
		</tr>
		<tr>
			<td><strong>Date</strong></td>
			<td>2025-10-1</td>
		</tr>
		<tr>
			<td><strong>Time</strong></td>
			<td>10:30 AM</td>
		</tr>
		<tr>
			<td><strong>Location</strong></td>
			<td>Remote mode through the GitHub platform</td>
		</tr>
		<tr>
			<td colspan="2"><strong>Prepared by</strong></td>
		</tr>
		<tr>
			<td><strong>Attendees (to planinning meeting)</strong></td>
			<td>All members of EasyPark</td>
		</tr>
		<tr>
			<td><strong>Sprint 1 Review Summary</strong></td>
			<td>We delivered and deployed the first public version of the EasyPark landing page via GitHub Pages. It included top navigation, hero, benefits, pricing, testimonials, contact form with basic validation, social links, and responsive/accessibility adjustments. </td>
		</tr>
		<tr>
			<td><strong>Sprint 1 Retrospective Summary</strong></td>
			<td>We worked well by splitting tasks clearly and keeping daily async check-ins.</td>
		</tr>
		<tr>
			<td colspan="2"><strong>Sprint Goal & User Stories</strong></td>
		</tr>
		<tr>
			<td><strong>Spritn 2 Goal</strong></td>
			<td>Enable end-to-end parking ticket payments in the web app via a sandbox payment gateway. Success is achieved when users can pay the computed amount, receive a receipt ID, the space status updates to “Free,” and the transaction is persisted and visible in a simple admin dashboard.</td>
		</tr>
		<tr>
			<td><strong>Sprint 2 Velocity</strong></td>
			<td>10</td>
		</tr>
		<tr>
			<td><strong>Sum of Story points</strong></td>
			<td>26</td>
		</tr>
	</tbody>
</table>

#### 5.2.2.2. Aspect Leaders and Collaborators.
En esta sección se presenta la elaboración de el artefacto Leadership-andCollaboration Matrix (LACX), el cual se presenta al líder y los colaboradores de este Sprint 2.

| Team Member (Last Name, First Name) | GitHub Username | Landing page |
| ------------------------------------|-----------------|-------------------------------------------|
| Elescano Leon, Piero Hugo | PieroHugo | L |
| Espinoza Chavez, Moises Filemon |MoisesECh| C | 
| Florez Shimabukuro, Fátima Belén |PengwinKingdom| C |
| Nakasone Gomes, Marco Antonio  | marquinho04 | C | 
| Paredes Davila, Jose Adrian  | joseadro09 | C | 


#### 5.2.2.3. Sprint Backlog 2
<table> 
	<tr> 
		<td><strong>Sprint #</strong></td> 
		<td colspan="7">Sprint 2</td> 
	</tr> 
	<tr> 
		<td colspan="2"><strong>User Story</strong></td> 
		<td colspan="6"><strong>Work-item / Task</strong></td> 
	</tr> 
	<tr> 
		<td><strong>Id</strong></td> 
		<td><strong>Title</strong></td> 
		<td><strong>Id</strong></td> 
		<td><strong>Title</strong></td> 
		<td><strong>Description</strong></td> 
		<td><strong>Estimation (Hours)</strong></td> 
		<td><strong>Assigned To</strong></td> 
		<td><strong>Status (To-do / In-Process / To-review / Done)</strong></td> 
	</tr> 
	<tr> 
		<td rowspan="6">EP03-US20</td> 
		<td rowspan="6">Procesamiento de pagos frontend</td> 
		<td>T20-01</td> <td>UI de pago y cálculo de monto</td> 
		<td>Formulario con método sandbox, validaciones y cálculo de monto (tiempo × tarifa)</td> 
		<td>6</td> 
		<td>Piero Elescano</td> 
		<td>To-do</td> 
	</tr> 
	<tr> 
		<td>T20-02</td> 
		<td>Integración pasarela sandbox</td> 
		<td>Conectar SDK/REST de la pasarela y manejo de tokens</td> 
		<td>8</td> 
		<td>Moises Espinoza</td> 
		<td>To-do</td> 
	</tr> 
	<tr> 
		<td>T20-03</td> 
		<td>Flujos de éxito/fracaso</td> 
		<td>Mensajes de confirmación/error, reintento y estados de carga</td> 
		<td>4</td> 
		<td>Fátima Florez</td> 
		<td>To-do</td> 
	</tr> 
	<tr> 
		<td>T20-04</td> 
		<td>Persistir transacción y receiptId</td> 
		<td>Generar <code>receiptId</code> y guardar pago (monto, fecha, espacio, método, estado) en la BD</td> 
		<td>6</td> 
		<td>Marco Nakasone</td> 
		<td>To-do</td> 
	</tr> 
	<tr> 
		<td>T20-05</td> 
		<td>Actualizar estado del espacio</td> 
		<td>Marcar espacio como <strong>Libre</strong> post-pago y registrar en historial de ocupación</td> 
		<td>4</td> 
		<td>Jose Paredes</td> 
		<td>To-do</td> 
	</tr> 
	<tr> 
		<td>T20-06</td> 
		<td>Tests del flujo de pago</td> 
		<td>Pruebas unitarias/integración: éxito, tarjeta inválida, timeout, doble clic, etc</td> 
		<td>4</td> 
		<td>Moises Espinoza</td> 
		<td>To-do</td> 
	</tr> 
	<tr> 
		<td rowspan="4">EP01-US14</td> 
		<td rowspan="4">Visualización de dashboard</td> 
		<td>T14-01</td> 
		<td>Ruta protegida /admin</td> 
		<td>Configurar navegación protegida y layout del dashboard</td> 
		<td>3</td> 
		<td>Piero Elescano</td> 
		<td>To-do</td> 
	</tr> 
	<tr> 
		<td>T14-02</td> 
		<td>Tabla de transacciones</td> 
		<td>Listar fecha, monto, <code>receiptId</code>, espacio y estado; paginación básica</td> 
		<td>5</td> 
		<td>Marco Nakasone</td> 
		<td>To-do</td> 
	</tr> 
	<tr> 
		<td>T14-03</td> 
		<td>Endpoint listado pagos</td> 
		<td>Servicio/endpoint para obtener transacciones con filtros</td> 
		<td>4</td> 
		<td>Jose Paredes</td> 
		<td>To-do</td> 
	</tr> 
	<tr> 
		<td>T14-04</td> 
		<td>Estados vacío/error</td> 
		<td>Diseñar empty state y manejo de errores en la vista</td> 
		<td>4</td> 
		<td>Fátima Florez</td> 
		<td>To-do</td> 
	</tr> 
	<tr> 
		<td rowspan="2">EP03-US19</td> 
		<td rowspan="2">Visualización de tarifas</td> 
		<td>T19-01</td> 
		<td>Servicio de tarifas</td> 
		<td>Fuente de tarifas por horario/espacio; formateo para el frontend</td> 
		<td>3</td> 
		<td>Marco Nakasone</td> 
		<td>To-do</td> 
	</tr> 
	<tr> 
		<td>T19-02</td> 
		<td>Tarifa en UI de pago</td> 
		<td>Mostrar tarifa vigente y desglose antes de confirmar el pago</td> 
		<td>3</td> 
		<td>Piero Elescano</td> 
		<td>To-do</td> 
	</tr> 
	<tr> 
		<td rowspan="2">EP01-US15</td> 
		<td rowspan="2">Gestión visual de espacios</td> 
		<td>T15-01</td> <td>Endpoint cambiar estado</td> 
		<td>Exponer servicio para marcar espacio como Libre después del pago</td> 
		<td>3</td> 
		<td>Jose Paredes</td> 
		<td>To-do</td> 
	</tr> 
	<tr> 
		<td>T15-02</td> 
		<td>Refresco de ocupación</td> 
		<td>Actualizar la vista tras cambiar el estado</td> 
		<td>2</td> 
		<td>Piero Elescano</td> 
		<td>To-do</td> 
	</tr> 
	<tr> 
		<td rowspan="2">EP02-US12</td> 
		<td rowspan="2">Inicio de sesión</td> 
		<td>T12-01</td> 
		<td>Login básico y sesión</td> 
		<td>Formulario de login y manejo simple de sesión </td> 
		<td>4</td> 
		<td>Piero Elescano</td> 
		<td>To-do</td> 
	</tr> 
	<tr> 
		<td>T12-02</td> 
		<td>Guard para dashboard</td> 
		<td>Bloquear acceso a rutas privadas si no hay sesión válida</td> 
		<td>2</td> 
		<td>Fátima Florez</td> 
		<td>To-do</td> 
	</tr> 
	<tr> 
		<td rowspan="2">EP03-US31</td> 
		<td rowspan="2">Validación de integridad de datos</td> 
		<td>T31-01</td> 
		<td>Validar monto del pago</td> 
		<td>Recalcular en backend y comparar; evitar manipulación del importe</td> 
		<td>4</td> 
		<td>Marco Nakasone</td> 
		<td>To-do</td> 
	</tr> 
	<tr> 
		<td>T31-02</td> 
		<td>Idempotencia del cobro</td> 
		<td>Prevenir doble pago</td> 
		<td>4</td> 
		<td>Jose Paredes</td> 
		<td>To-do</td> 
	</tr> 
	<tr> 
		<td rowspan="2">EP02-US25</td> 
		<td rowspan="2">Cierre de sesión seguro</td> 
		<td>T25-01</td> 
		<td>Logout manual</td> 
		<td>Botón “Salir” y limpieza de sesión/token</td> 
		<td>2</td> 
		<td>Piero Elescano</td> 
		<td>To-do</td> 
	</tr> 
	<tr> 
		<td>T25-02</td> 
		<td>Auto-logout por inactividad</td> 
		<td>Expirar sesión automáticamente y redirigir a login</td> 
		<td>3</td> 
		<td>Jose Paredes</td>
		<td>To-do</td> 
	</tr> 
</table>


