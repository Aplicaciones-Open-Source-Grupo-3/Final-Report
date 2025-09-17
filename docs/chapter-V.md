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
			<td colspan="2"><strong>Spring Planing Background</strong></td>
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
			<td><strong>Attends (to planinning meeting)</strong></td>
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
			<td><strong>Spritn 1 Goal</strong></td>
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
