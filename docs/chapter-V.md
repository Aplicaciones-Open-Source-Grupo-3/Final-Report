# Capítulo V: Product Implementation, Validation & Deployment
## 5.1. Software Configuration Management.
Seguidamente, se mostrará un repositorio centralizado y estructurado que funcionará como referencia para un desarrollo enfocado y coherente de nuestra solución. Además se incluyen otras secciones para Source Code Management, Development Environment Configuration y Deployment Configuration.

### 5.1.1. Software Development Environment Configuration.
En esta sección, se detalla la configuración del entorno de desarrollo utilizado para construir la aplicación EasyPark. Se describen las herramientas y plataformas que facilitaron la planificación del proyecto, el diseño centrado en el usuario, el desarrollo frontend y backend, las pruebas automatizadas y la documentación técnica. Estas soluciones permitieron una colaboración efectiva entre los miembros del equipo, asegurando un desarrollo ágil, organizado y alineado con los objetivos del sistema.
## Gestión del Proyecto
La gestión del proyecto es clave para coordinar actividades, tareas y equipos, asegurando que el proyecto Vehix avance dentro de los tiempos y objetivos planteados.

**Modelo SaaS Web:** 

Durante el desarrollo, se utilizó una solución basada en la nube accesible vía navegador, permitiendo la planificación, seguimiento de tareas y colaboración, sin la necesidad de instalar la aplicaion en las computadoras de los usuarios.
## Gestión de Requisitos
Esta disciplina asegura que el sistema cumpla con las necesidades de los usuarios y partes interesadas, mediante el levantamiento y seguimiento de requisitos funcionales y no funcionales.

**Pivotal Tracker:**  

Utilizada para gestionar historias de usuario, agruparlas en épicas y asignarles prioridades. Proporciona visibilidad en tiempo real del progreso del equipo y permite ajustes dinámicos en el flujo de trabajo.
## Diseño UX/UI del Producto
El diseño centrado en el usuario fue esencial para Vehix. Nuestro objetivo fue crear una interfaz intuitiva, accesible desde web y dispositivos móviles.
**Herramientas utilizadas:**
- **Uxpressia:**  
  Nos permitió desarrollar mapas de empatía, perfiles de usuario (User Personas) y Customer Journey Maps.
- **MIRO:**  
  Facilitó sesiones colaborativas para ideación, mapas mentales y estructuración del diseño de experiencia.
- **Figma:**  
  Herramienta central para la creación de prototipos interactivos y diseño visual responsive.
- **Lucidchart:**  
  Usada para la elaboración de diagramas UML, mapas mentales y arquitecturas del sistema.
- **Overflow:**  
  Utilizada para diseñar flujos de usuario (User Flows) y visualizar recorridos dentro de la aplicación.
## Desarrollo de Software
- **GitHub:**  
  Repositorio central de código fuente y seguimiento del control de versiones del proyecto Vehix.
- **Git:**  
  Herramienta instalada localmente que nos permitió gestionar cambios, crear ramas y coordinar el trabajo colaborativo.
- **WebStorm:**  
  IDE utilizado principalmente para desarrollo en frontend con HTML, CSS, JavaScript y Vue.js.
- **Rider:**  
  IDE empleado para el backend con C# y ASP.NET, donde se implementó el servicio web que alimenta a la aplicación Vehix.
## Pruebas de Software
El objetivo de esta fase fue validar y verificar el correcto funcionamiento del sistema.

**Lenguaje Gherkin:**  

Utilizamos este lenguaje específico de dominio (DSL) para redactar historias de usuario en formato estructurado, permitiendo automatizar pruebas basadas en escenarios.
Esto facilitó una verificación sistemática del comportamiento esperado de la aplicación.
## Documentación del Software

Incluye todo el material que describe el funcionamiento del sistema y cómo utilizarlo. La documentación fue elaborada tanto para usuarios finales como para el equipo técnico, y se integró como parte del repositorio del proyecto.

### 5.1.2. Source Code Management.
En esta sección se describe cómo se gestionaron las modificaciones al código del sistema Vehix, así como las convenciones empleadas para los commits y las versiones liberadas a lo largo del ciclo de desarrollo.

### Plataforma de Control de Versiones

Para el control y seguimiento del código fuente, se utilizó **GitHub** como plataforma centralizada. Allí se crearon distintos repositorios independientes para las principales partes del sistema: landing page, backend (servicio web), frontend y documentación técnica. El control de versiones se realizó de forma distribuida mediante **Git**, instalado localmente por cada integrante del equipo.

### Flujo de Trabajo Git (GitFlow)

Se adoptó el modelo de ramificación **GitFlow**, debido a su capacidad para mantener el código organizado y facilitar el trabajo colaborativo. Esta metodología define dos tipos de ramas:

#### Ramas Principales

- `main`: Contiene la versión estable y lista para producción del sistema Vehix. Todo código integrado aquí representa una nueva entrega oficial del producto.
- `develop`: Es la rama donde se integran funcionalidades completadas y testeadas. Sirve como entorno previo a producción para preparar nuevos lanzamientos.

#### Ramas de Apoyo

- `feature`: Se crean desde `develop` para el desarrollo de nuevas funcionalidades específicas. Una vez finalizadas, se integran nuevamente en `develop`.
- `release`: Generadas desde `develop` para preparar una nueva versión estable. Incluyen ajustes menores, corrección de bugs y preparación para despliegue.
- `hotfix`: Se crean directamente desde `main` cuando se requiere resolver errores críticos en producción. Una vez resueltos, se integran tanto en `main` como en `develop`.

### Versionado Semántico (Semantic Versioning)

El proyecto implementa el estándar **Semantic Versioning 2.0.0**, permitiendo una numeración clara y predecible de versiones mediante el esquema `X.Y.Z`, donde:

- `Z` (Patch): Se incrementa por correcciones menores sin afectar compatibilidad.
- `Y` (Minor): Se incrementa cuando se agregan nuevas funcionalidades compatibles.
- `X` (Major): Se incrementa cuando se introducen cambios que rompen compatibilidad con versiones anteriores.

**Ejemplos de nombres de ramas release:**
- `release-1.0.5`
- `release-2.1.4`
- `release-2.2.1`

### Commits Convencionales (Conventional Commits)

Para mantener un historial claro y significativo de los cambios, se empleó el estándar **Conventional Commits**, con la siguiente estructura:

``` <type>[opcional scope]: <descripción> ```

```[optional body]```

```[optional footer]```

#### Tipos de Commit (`type`):

- `feat`: Nueva funcionalidad.
- `fix`: Corrección de errores.
- `docs`: Cambios en la documentación.
- `refactor`: Reestructuración sin alterar comportamiento.
- `perf`: Mejoras de rendimiento.
- `chore`: Tareas menores sin impacto funcional.
- `build`: Cambios relacionados a dependencias o configuración.

#### Otros Campos:

- **scope** *(opcional)*: Indica qué módulo o componente fue modificado.
- **description** *(obligatorio)*: Breve explicación del cambio, en minúsculas y forma imperativa.
- **body** *(opcional)*: Detalles adicionales del cambio.
- **footer** *(opcional)*: Información extra sobre _breaking changes_ u otros avisos.

Este enfoque facilita la trazabilidad, automatización del versionado y claridad en las revisiones por parte del equipo de desarrollo de *Vehix*.
### Commits Convencionales (Conventional Commits)

### 5.1.3. Source Code Style Guide & Conventions.
En esta parte del proyecto, nos centraremos en definir un conjunto uniforme de normas y convenciones de estilo y programación para el desarrollo de nuestra aplicación web Vehix. Estas pautas son fundamentales para asegurar que el código sea consistente, claro y bien estructurado, lo que a su vez facilitará su mantenimiento y escalabilidad durante todo el ciclo de vida del proyecto.

Para asegurar la consistencia y calidad en el desarrollo de nuestra Landing Page implementaremos una serie de convenciones específicas para los distintos lenguajes y tecnologías que utilizamos:

#### HTML

-  Siempre iniciar los documentos HTML con `<!DOCTYPE html>` y configurar `<meta charset="UTF-8">`.

-  Nombres de etiquetas y atributos siempre en minúsculas (`<div>`, `<section>`, `<button>`, etc.).

-  Siempre se deben usar **comillas dobles**  `(")` para los valores de los atributos.
Ejemplo: `<input type="text" name="email" />`

``` 
input type="text" name="email" />
```

-  Se incluirán los atributos `alt`, `width` y `height` en las imágenes para mejorar la accesibilidad y el diseño responsivo.

-  Utilizar comentarios `<!-- -->` para marcar secciones importantes del código.

-  Definir la codificación de caracteres como UTF-8 para soportar la mayoría de los caracteres de   todos los idiomas, `<meta charset="UTF-8">`

-  Inclusión de la hoja de estilos CSS, la hoja de estilo principal debe ser enlazada dentro de la sección `<head>`. Usando siempre la etiqueta `<link>` de la siguiente manera:

``` 
<link rel="stylesheet" href="styles.css">                                 
``` 
   
-  Inclusión de archivos JavaScript, los archivos JavaScript deben incluirse **antes del cierre de la etiqueta `</body>`** para mejorar el tiempo de carga de la página.

``` 
<script src="script.js"></script>
</body>
</html>
``` 


#### CSS

- Todos los nombres de clases e IDs deben estar en inglés y escritos usando el formato **kebab-case**, es decir, en minúsculas y separando palabras con guiones (`-`), por ejemplo: `.hero-text`, `.plan-card-pro`, `.faq-title`.

-  cada declaración debe terminar con un punto y coma `;`.
    Ejemplo correcto:
    
 ```
.title-who {
  font-size: 34px;
  font-weight: bold;
  padding: 2%;
}	
```

-  Las llaves `{}` deben colocarse en la misma línea que el selector.

```
.benefit-card {
  background: black;
  color: white;
}
```

- Implementar **media queries** (`@media`) para adaptar el diseño a diferentes dispositivos.

```
@media (max-width: 768px) {
  .hero-text {
    text-align: center;
  }
}
```


#### JavaScript

-  Usar `const` para valores que no cambian y `let` para los que sí.

```
const wrapper = document.getElementById("main-wrapper");
let currentSlide = 0;
```

- Evitar el uso de `var` por completo (obsoleto).

- Las llaves `{}` deben abrirse en la misma línea que la declaración.

```
function toggleMenu() {
  // lógica aquí
}
```

- Punto y coma obligatorio al final de cada instrucción.

```
document.addEventListener("DOMContentLoaded", updateSlider);
```

- cada función debe hacer una sola cosa.

```
document.addEventListener("DOMContentLoaded", updateSlider);
```

- Usar **event delegation y listeners** con funciones nombradas cuando sea posible.

```
document.querySelectorAll('.faq-question').forEach(button => {
  button.addEventListener('click', () => {
    // ...
  });
});
```

### 5.1.4. Software Deployment Configuration.

En esta sección, se tratará de explicar el procedimiento de despliegue de nuestros proyectos como LandingPage, Backend y FrontEnd.

##### LandingPage

Para el despliegue de nuestra landing page se escogio Git Page siendo una alternativa facil de usar y de configurar.

 - **Paso 1:** Para desplegar el LandingPage hay que dirigirse al repositorio del landingPage y luego entrar a la opción de settings.



 - **Paso 2**: Ahora entraremos a la opción de Pages donde seleccionaremos la rama del proyecto que queremos desplegar



- **Paso 3:** Es asi como debe quedarla selección de la rama 



- **Paso 4:** Luego de esperar unos minutos la pagina del LandingPage se desplegara y aparecerá la opción de acceder a esta misma



## 5.2. Landing Page, Services & Applications Implementation.
En esta sección se detalla y demuestra el proceso llevado a cabo para la implementación, pruebas, documentación y despliegue de la Landing Page, los Servicios Web y las Aplicaciones Web Frontend.

### 5.2.1. Sprint 1
En esta sección, documentaremos y explicaremos el desarrollo del Sprint 1 en términos de desarrollo del producto y el trabajo colaborativo del equipo. Se abordará varias secciones, incluyendo el Sprint Backlog, Development Evidence for Sprint Review, Sprint Planning.

#### 5.2.1.1. Sprint Planning 1.
En esta sección, especificáremos los principales aspectos del Sprint Planning Meeting 1.


