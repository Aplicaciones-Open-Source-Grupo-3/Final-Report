# Capítulo III: Requirements Specification

## 3.1. User Stories
En esta sección el equipo redacta la definición y la elaboración de los User Stories (Como, Quiero y Para). Las historias de usuario son un recurso clave para construir software y diseñar proyectos con enfoque en las necesidades y experiencias de las personas. De manera que se a usado la sintaxis Gherkin para los tests de aceptación.

| Epic /Story ID | Título | Descripción | Criterios de aceptación | Relacionado con (Epic ID) |
| :---- | :---- | ----- | ----- | ----- |
| EP01 | Gestión de Estacionamientos | **Como** administrador de estacionamientos **quiero** gestionar los espacios y ocupación en tiempo real **para** optimizar los ingresos y reducir la informalidad. | - | - |
| EP02 | Gestión de Usuarios y Roles | **Como** administrador u operador **quiero** gestionar usuarios y asignar roles **para** controlar accesos y mantener la seguridad. | - | - |
| EP03 | Gestión de Pagos y Reservas | **Como** usuario o administrador **quiero** procesar pagos, emitir comprobantes y gestionar reservas **para** facilitar y transparentar las transacciones. | - | - |
| EP04 | Reportes y Analíticas | **Como** administrador **quiero** acceder a reportes y analíticas en tiempo real **para** tomar mejores decisiones sobre tarifas, promociones y eficiencia. | - | - |
| EP05 | Landing Page & Información Corporativa | **Como** visitante **quiero** acceder a información clara sobre EasyPark, sus beneficios y contacto **para** considerar el uso del sistema. | - | - |
| US01 | Información general EasyPark | **Como** visitante **quiero** ver una descripción clara de EasyPark en la landing page **para** entender de qué trata la solución. | Escenario 1: Visualización exitosa Dado que el visitante accede a la landing page, Cuando busca información general sobre EasyPark, Entonces la descripción detallada se muestra correctamente y es comprensible. <br>---<br> Escenario 2: Falta de contenido Dado que el visitante accede a la landing page, Cuando la sección de información general no está disponible o contiene errores, Entonces el sistema muestra un mensaje indicando que la información no está disponible. | EP05 |
| US02 | Características destacadas | **Como** potencial cliente **quiero** ver una lista de beneficios y características clave en la landing **para** decidir si EasyPark es adecuado para mi negocio. | Escenario 1: Visualización exitosa Dado que el visitante accede a la landing page, Cuando selecciona la sección de beneficios, Entonces se despliega una lista actualizada de características. <br>---<br> Escenario 2: Error de carga Dado que el visitante accede a la sección de beneficios, Cuando la información no se puede cargar, Entonces el sistema informa el error y sugiere intentar más tarde. | EP05 |
| US03 | Planes y precios | **Como** interesado **quiero** consultar los planes y precios desde la landing **para** evaluar la oferta y tomar decisiones. | Escenario 1: Visualización correcta Dado que el usuario accede a la sección de precios, Cuando selecciona un plan, Entonces visualiza detalles claros y completos de cada plan. <br>---<br> Escenario 2: Información incompleta Dado que el usuario consulta los planes, Cuando los datos están incompletos o desactualizados, Entonces el sistema muestra un aviso de que la información se actualizará pronto. | EP05 |
| US04 | Formulario de contacto | **Como** visitante **quiero** enviar una consulta o solicitar información a través de un formulario en la landing **para** recibir atención personalizada. | Escenario 1: Envío exitoso Dado que el usuario completa el formulario correctamente, Cuando envía la consulta, Entonces el sistema confirma la recepción y almacena la solicitud. <br>---<br> Escenario 2: Error en el formulario Dado que el usuario omite campos obligatorios o ingresa datos incorrectos, Cuando intenta enviar el formulario, Entonces el sistema indica los errores y solicita corrección. | EP05 |
| US05 | Testimonios de clientes | **Como** visitante **quiero** conocer opiniones de otros usuarios **para** confiar en la solución EasyPark. | Escenario 1: Visualización exitosa Dado que el visitante accede a testimonios, Cuando existen testimonios disponibles, Entonces se muestran correctamente en la landing page. <br>---<br> Escenario 2: Sin testimonios Dado que el visitante accede a la sección de testimonios, Cuando no existen testimonios publicados, Entonces el sistema informa que aún no hay opiniones disponibles. | EP05 |
| US06 | Preguntas frecuentes (FAQs) | **Como** visitante **quiero** consultar un listado de preguntas frecuentes **para** resolver dudas rápidamente. | Escenario 1: Acceso exitoso Dado que el usuario accede a la sección de FAQs, Cuando selecciona una pregunta, Entonces se muestra la respuesta correspondiente. <br>---<br> Escenario 2: Error de carga Dado que el usuario accede a FAQs, Cuando la información no está disponible, Entonces el sistema muestra mensaje de error y sugiere contactar soporte. | EP05 |
| US07 | Acceso a demo o tour virtual | **Como** potencial usuario **quiero** acceder a una demo interactiva o tour virtual **para** conocer cómo funciona EasyPark. | Escenario 1: Acceso exitoso Dado que el usuario selecciona la demo, Cuando inicia el tour, Entonces puede navegar entre las funciones sin errores. <br>---<br> Escenario 2: Demo no disponible Dado que el usuario intenta acceder a la demo, Cuando la funcionalidad está deshabilitada, Entonces el sistema indica que la demo se encuentra temporalmente fuera de servicio. | EP05 |
| US08 | Enlaces a redes sociales | **Como** visitante **quiero** encontrar enlaces a redes sociales oficiales **para** seguir novedades y contacto alternativo. | Escenario 1: Visualización exitosa Dado que el visitante accede a la landing, Cuando busca los enlaces, Entonces se muestran correctamente y redirigen a las redes oficiales. <br>---<br> Escenario 2: Enlaces rotos Dado que el visitante selecciona un enlace, Cuando el enlace está roto o desactualizado, Entonces el sistema muestra un aviso de error y contacta al administrador. | EP05 |
| US09 | Registro de interés (newsletter) | **Como** usuario interesado **quiero** dejar mi correo para recibir novedades y promociones **para** mantenerme informado. | Escenario 1: Registro exitoso Dado que el usuario ingresa un correo válido, Cuando confirma el registro, Entonces recibe un mensaje de confirmación. <br>---<br> Escenario 2: Error en suscripción Dado que el usuario ingresa un correo inválido o repetido, Cuando intenta suscribirse, Entonces el sistema informa el error y solicita corrección. | EP05 |
| US10 | Accesibilidad y responsive | **Como** visitante **quiero** que la landing page funcione correctamente en cualquier dispositivo y sea accesible **para** tener una buena experiencia. | Escenario 1: Visualización en múltiples dispositivos Dado que el visitante accede desde distintos dispositivos, Cuando navega la landing, Entonces el contenido se adapta correctamente y es accesible. <br>---<br> Escenario 2: Problemas de visualización Dado que el visitante accede desde un dispositivo poco común, Cuando la página no se adapta, Entonces el sistema muestra un aviso de incompatibilidad y recomienda navegadores compatibles. | EP05 |
| US11 | Registro de usuario | **Como** operador o administrador **quiero** crear una cuenta en EasyPark **para** acceder a las funcionalidades del sistema. | Escenario 1: Registro exitoso Dado que el usuario ingresa información válida, Cuando solicita el registro, Entonces su cuenta se crea correctamente. <br>---<br> Escenario 2: Error en el registro Dado que el usuario ingresa información incompleta o inválida, Cuando intenta registrarse, Entonces el sistema notifica el error y solicita corrección. | EP02 |
| US12 | Inicio de sesión | **Como** usuario registrado **quiero** iniciar sesión de forma segura **para** acceder al panel de gestión. | Escenario 1: Inicio exitoso Dado que el usuario ingresa credenciales válidas, Cuando solicita acceso, Entonces accede al panel correctamente. <br>---<br> Escenario 2: Error de autenticación Dado que el usuario ingresa credenciales incorrectas, Cuando intenta acceder, Entonces el sistema muestra un mensaje de error y permite reintentar. | EP02 |
| US13 | Recuperación de contraseña | **Como** usuario **quiero** recuperar mi contraseña olvidada **para** restablecer acceso a mi cuenta. | Escenario 1: Recuperación exitosa Dado que el usuario solicita recuperar su contraseña con un correo válido, Cuando sigue el enlace enviado, Entonces puede restablecer su contraseña. <br>---<br> Escenario 2: Error en recuperación Dado que el usuario ingresa un correo no registrado, Cuando solicita la recuperación, Entonces el sistema muestra un aviso de error. | EP02 |
| US14 | Visualización de dashboard | **Como** administrador **quiero** acceder a un dashboard central **para** ver el estado general de los estacionamientos. | Escenario 1: Acceso exitoso Dado que el usuario inicia sesión, Cuando accede al dashboard, Entonces visualiza los datos actualizados. <br>---<br> Escenario 2: Error de carga Dado que el usuario accede al dashboard, Cuando los datos no se pueden cargar, Entonces el sistema muestra un mensaje de error temporal. | EP01 |
| US15 | Gestión visual de espacios | **Como** operador **quiero** ver y actualizar el estado de los espacios (libre/ocupado/reservado) **para** mantener la información al día. | Escenario 1: Actualización exitosa Dado que el operador selecciona un espacio, Cuando cambia su estado, Entonces la actualización se refleja en tiempo real. <br>---<br> Escenario 2: Error de actualización Dado que el operador intenta modificar un espacio, Cuando ocurre un error de sistema, Entonces el estado no cambia y se informa el problema. | EP01 |
| US16 | Consulta de historial de ocupación | **Como** administrador **quiero** ver el historial de ocupación de los espacios **para** analizar tendencias. | Escenario 1: Consulta exitosa Dado que el usuario selecciona un rango de fechas, Cuando solicita el historial, Entonces se muestran los datos correspondientes. <br>---<br> Escenario 2: Sin datos Dado que el usuario selecciona un periodo sin registros, Cuando solicita el historial, Entonces el sistema informa que no hay datos disponibles. | EP04 |
| US17 | Gestión de reservas desde frontend | **Como** usuario **quiero** reservar un espacio de estacionamiento desde la aplicación **para** asegurar disponibilidad. | Escenario 1: Reserva exitosa Dado que el usuario selecciona un espacio disponible, Cuando confirma la reserva, Entonces el sistema la registra correctamente. <br>---<br> Escenario 2: Reserva fallida Dado que el usuario selecciona un espacio, Cuando ya está ocupado, Entonces el sistema notifica que debe elegir otro espacio. | EP03 |
| US18 | Cancelación de reservas | **Como** usuario **quiero** cancelar una reserva activa **para** liberar el espacio sin penalización (cuando aplica). | Escenario 1: Cancelación exitosa Dado que el usuario tiene una reserva activa, Cuando solicita la cancelación, Entonces el sistema libera el espacio y notifica al usuario. <br>---<br> Escenario 2: Cancelación fallida Dado que el usuario intenta cancelar una reserva ya vencida o no existente, Cuando realiza la acción, Entonces el sistema informa que no es posible cancelar. | EP03 |
| US19 | Visualización de tarifas | **Como** conductor **quiero** consultar las tarifas vigentes según horario y espacio **para** planificar mi pago. | Escenario 1: Consulta exitosa Dado que el usuario accede a la sección de tarifas, Cuando selecciona un horario, Entonces visualiza las tarifas correctas. <br>---<br> Escenario 2: Error en consulta Dado que el usuario consulta tarifas, Cuando hay un error de carga, Entonces el sistema muestra mensaje de indisponibilidad. | EP03 |
| US20 | Procesamiento de pagos frontend | **Como** usuario **quiero** pagar mi estacionamiento desde la app usando distintos métodos **para** agilizar la salida. | Escenario 1: Pago exitoso Dado que el usuario selecciona método y datos válidos, Cuando confirma el pago, Entonces la transacción se procesa y se emite comprobante. <br>---<br> Escenario 2: Pago fallido Dado que el usuario intenta pagar con datos incorrectos o fondos insuficientes, Cuando confirma el pago, Entonces el sistema rechaza la transacción e informa el motivo. | EP03 |
| US21 | Recepción de notificaciones | **Como** usuario u operador **quiero** recibir notificaciones sobre reservas, pagos o incidencias **para** actuar a tiempo. | Escenario 1: Notificación exitosa Dado que ocurre un evento importante, Cuando el usuario tiene notificaciones activas, Entonces recibe el aviso en tiempo real. <br>---<br> Escenario 2: Notificación fallida Dado que ocurre un evento, Cuando el usuario no tiene notificaciones activas o hay error, Entonces no recibe aviso y el sistema registra el fallo. | EP01 |
| US22 | Gestión de incidencias | **Como** operador **quiero** registrar y visualizar incidencias en el estacionamiento **para** dar seguimiento y solución. | Escenario 1: Registro exitoso Dado que el operador llena el formulario de incidencia, Cuando envía la información, Entonces la incidencia se registra y queda visible. <br>---<br> Escenario 2: Error en registro Dado que el operador omite datos obligatorios, Cuando intenta registrar la incidencia, Entonces el sistema indica el error y solicita completar los campos. | EP01 |
| US23 | Edición de perfil de usuario | **Como** usuario **quiero** modificar mis datos personales y de contacto **para** mantener mi perfil actualizado. | Escenario 1: Edición exitosa Dado que el usuario ingresa nuevos datos válidos, Cuando guarda los cambios, Entonces el perfil se actualiza correctamente. <br>---<br> Escenario 2: Error en edición Dado que el usuario ingresa datos inválidos o incompletos, Cuando intenta guardar, Entonces el sistema informa el error y no guarda los cambios. | EP02 |
| US24 | Soporte y ayuda online | **Como** usuario **quiero** acceder a recursos de ayuda y soporte en la app **para** resolver dudas durante el uso. | Escenario 1: Acceso exitoso Dado que el usuario selecciona ayuda, Cuando accede a la sección, Entonces visualiza recursos y contacto de soporte. <br>---<br> Escenario 2: Sin recursos Dado que el usuario accede a ayuda, Cuando no existen recursos disponibles, Entonces el sistema muestra un mensaje de disculpa. | EP05 |
| US25 | Cierre de sesión seguro | **Como** usuario **quiero** cerrar mi sesión manualmente y automáticamente por inactividad **para** proteger mi cuenta. | Escenario 1: Cierre exitoso Dado que el usuario selecciona salir o la sesión expira, Cuando se cierra sesión, Entonces el usuario es redirigido al login. <br>---<br> Escenario 2: Error en cierre Dado que el usuario intenta cerrar sesión, Cuando ocurre un error, Entonces el sistema informa el fallo y mantiene la sesión activa. | EP02 |
| US26 | API de gestión de espacios | **Como** desarrollador **quiero** una API REST para gestionar los espacios de estacionamiento **para** integraciones externas y automatizaciones. | Escenario 1: Solicitud exitosa Dado que el desarrollador envía una petición válida, Cuando utiliza la API, Entonces recibe la respuesta esperada. <br>---<br> Escenario 2: Solicitud inválida Dado que el desarrollador envía una petición con datos incorrectos, Cuando usa la API, Entonces el sistema retorna un mensaje de error detallado. | EP01 |
| US27 | API de usuarios y roles | **Como** desarrollador **quiero** endpoints para alta, baja, modificación y consulta de usuarios y roles **para** facilitar la administración. | Escenario 1: Operación exitosa Dado que la petición contiene datos válidos y permisos adecuados, Cuando se ejecuta la operación, Entonces el sistema responde correctamente. <br>---<br> Escenario 2: Error de permisos o datos Dado que los datos faltan o el usuario no tiene permisos, Cuando se realiza la operación, Entonces se retorna un error claro. | EP02 |
| US28 | API de pagos y reservas | **Como** desarrollador **quiero** exponer endpoints para procesar pagos y gestionar reservas **para** integración con apps de terceros. | Escenario 1: Procesamiento exitoso Dado que se envía una solicitud válida, Cuando se procesa el pago o reserva, Entonces la operación se completa y retorna confirmación. <br>---<br> Escenario 2: Fallo en procesamiento Dado que se envía una solicitud incorrecta o con fondos insuficientes, Cuando se procesa, Entonces se retorna un error y no se realiza la transacción. | EP03 |
| US29 | API de reportes y analíticas | **Como** desarrollador **quiero** obtener reportes de ocupación, ingresos y uso **para** análisis externo. | Escenario 1: Reporte exitoso Dado que la solicitud contiene filtros válidos, Cuando se consulta el endpoint, Entonces se recibe el reporte solicitado. <br>---<br> Escenario 2: Error de consulta Dado que los filtros no son válidos o hay error de sistema, Cuando se consulta, Entonces se retorna mensaje de error. | EP04 |
| US30 | Gestión de logs y auditoría | **Como** administrador **quiero** acceder a registros de acciones críticas en el sistema **para** auditorías y seguridad. | Escenario 1: Consulta exitosa Dado que el usuario tiene permisos y selecciona filtros, Cuando consulta logs, Entonces recibe los registros solicitados. <br>---<br> Escenario 2: Error en consulta Dado que el usuario no tiene permisos o filtros incorrectos, Cuando consulta, Entonces el sistema informa el error. | EP04 |
| US31 | Validación de integridad de datos | **Como** backend **quiero** validar y proteger la integridad de los datos de ocupación y pagos **para** evitar errores y fraudes. | Escenario 1: Validación exitosa Dado que se recibe información válida, Cuando se valida, Entonces los datos se almacenan correctamente. <br>---<br> Escenario 2: Validación fallida Dado que se recibe información corrupta o alterada, Cuando se valida, Entonces el sistema rechaza los datos y registra el intento. | EP03 |
| US32 | Gestión de backups y restauración | **Como** responsable técnico **quiero** programar backups automáticos y restaurar datos **para** prevenir pérdidas. | Escenario 1: Backup exitoso Dado que la programación está activa, Cuando se ejecuta el backup, Entonces los datos se guardan correctamente. <br>---<br> Escenario 2: Error de backup Dado que ocurre una falla durante el proceso, Cuando se ejecuta el backup, Entonces el sistema notifica el error y registra el fallo. | EP01 |
| US33 | Integración con sistemas de pago externos | **Como** desarrollador **quiero** conectar EasyPark con pasarelas de pago externas **para** ampliar opciones de cobro. | Escenario 1: Integración exitosa Dado que la configuración es correcta, Cuando se realiza un pago, Entonces la transacción se procesa por la pasarela externa. <br>---<br> Escenario 2: Error en integración Dado que la configuración es incorrecta, Cuando se intenta un pago, Entonces el sistema retorna un error y no procesa la transacción. | EP03 |
| US34 | Autenticación y autorización | **Como** backend **quiero** implementar mecanismos robustos de autenticación y control de acceso **para** proteger los recursos. | Escenario 1: Acceso autorizado Dado que el usuario tiene credenciales válidas, Cuando accede a un recurso, Entonces el acceso es permitido. <br>---<br> Escenario 2: Acceso denegado Dado que el usuario no tiene permisos o credenciales inválidas, Cuando accede a un recurso, Entonces el sistema deniega el acceso y registra el intento. | EP02 |
| US35 | Monitoreo de disponibilidad | **Como** responsable técnico **quiero** monitorear la disponibilidad y salud de los servicios backend **para** detectar caídas. | Escenario 1: Monitoreo activo Dado que el sistema está operativo, Cuando ocurre una caída, Entonces se genera una alerta automática. <br>---<br> Escenario 2: Fallo de monitoreo Dado que el sistema de monitoreo no está configurado, Cuando ocurre una caída, Entonces no se genera alerta y se registra la falla. | EP01 |
| US36 | Generación automática de reportes | **Como** administrador **quiero** recibir reportes automáticos por email **para** mantenerme actualizado sin ingresar al sistema. | Escenario 1: Envío exitoso Dado que el reporte está programado, Cuando se genera, Entonces el administrador recibe el email con el reporte. <br>---<br> Escenario 2: Error de envío Dado que existe un problema en la generación o el envío de email, Cuando se intenta enviar, Entonces el sistema informa el error. | EP04 |
| US37 | Gestión de incidencias desde backend | **Como** backend **quiero** permitir registro y consulta de incidencias vía API **para** integración con sistemas de soporte. | Escenario 1: Registro exitoso Dado que la solicitud contiene datos válidos, Cuando se registra la incidencia, Entonces se almacena correctamente. <br>---<br> Escenario 2: Error en registro Dado que la solicitud es inválida o faltan datos, Cuando se intenta registrar, Entonces el sistema retorna error detallado. | EP01 |
| US38 | Versionado de API | **Como** desarrollador **quiero** que las APIs estén versionadas **para** evitar rupturas en integraciones existentes. | Escenario 1: Uso de versión correcta Dado que se llama a un endpoint con versión soportada, Cuando se realiza la petición, Entonces el sistema responde correctamente. <br>---<br> Escenario 2: Versión no soportada Dado que se llama a una versión deprecated, Cuando se realiza la petición, Entonces el sistema retorna mensaje de obsolescencia. | EP01 |
| US39 | Control de concurrencia | **Como** backend **quiero** evitar conflictos por operaciones simultáneas sobre el mismo espacio **para** mantener la consistencia. | Escenario 1: Operación exitosa Dado que no existen operaciones simultáneas, Cuando se realiza un cambio, Entonces se guarda correctamente. <br>---<br> Escenario 2: Conflicto detectado Dado que existen dos operaciones simultáneas sobre el mismo recurso, Cuando se intenta guardar ambos cambios, Entonces el sistema detecta y rechaza uno. | EP01 |
| US40 | Exportación de datos | **Como** administrador **quiero** exportar datos históricos de ocupación, pagos y usuarios **para** análisis externo. | Escenario 1: Exportación exitosa Dado que el usuario selecciona exportar datos, Cuando elige el formato y periodo, Entonces el sistema genera y descarga el archivo solicitado. <br>---<br> Escenario 2: Error en exportación Dado que el usuario selecciona exportar, Cuando ocurre un error de sistema, Entonces el sistema informa el fallo y no genera el archivo. | EP04 |
| TS01 | Pruebas automatizadas frontend | **Como** equipo técnico **quiero** implementar pruebas unitarias y de integración en frontend **para** asegurar la calidad de la interfaz. | Escenario 1: Pruebas exitosas Dado que se ejecutan las pruebas automáticas, Cuando el código es válido, Entonces todas las pruebas pasan correctamente y se genera reporte. <br>---<br> Escenario 2: Pruebas fallidas Dado que el código presenta errores, Cuando se ejecutan las pruebas, Entonces se reportan fallos y se detiene el despliegue. | - |
| TS02 | Pruebas automatizadas backend | **Como** equipo técnico **quiero** desarrollar tests unitarios y de integración para backend **para** garantizar la robustez de servicios. | Escenario 1: Pruebas exitosas Dado que se ejecutan pruebas sobre los endpoints backend, Cuando el código es correcto, Entonces todas las pruebas pasan exitosamente. <br>---<br> Escenario 2: Pruebas fallidas Dado que existen errores en el backend, Cuando se ejecutan las pruebas, Entonces se reportan los fallos y se impide el merge. | - |
| TS03 | Integración continua y despliegue automático | **Como** equipo técnico **quiero** configurar pipelines de CI/CD **para** agilizar pruebas y despliegues en cada push. | Escenario 1: Pipeline exitoso Dado que el repositorio recibe un push, Cuando se ejecuta el pipeline, Entonces las pruebas y despliegue se realizan automáticamente y sin errores. <br>---<br> Escenario 2: Fallo en pipeline Dado que ocurre un error en pruebas o build, Cuando se ejecuta el pipeline, Entonces se detiene el despliegue y se notifica al equipo. | - |
| TS04 | Seguridad y revisión de vulnerabilidades | **Como** responsable técnico **quiero** analizar el código en busca de vulnerabilidades **para** proteger los datos y usuarios. | Escenario 1: Análisis exitoso Dado que se ejecuta el análisis de seguridad, Cuando no existen vulnerabilidades, Entonces el sistema reporta código seguro. <br>---<br> Escenario 2: Vulnerabilidades detectadas Dado que se detectan fallos de seguridad, Cuando se ejecuta el análisis, Entonces se reportan y bloquea el despliegue hasta corregir. | - |
| TS05 | Documentación técnica automatizada | **Como** desarrollador **quiero** generar y mantener documentación técnica de APIs y arquitectura **para** facilitar el mantenimiento. | Escenario 1: Documentación generada Dado que se actualiza el código, Cuando se ejecuta la herramienta de documentación, Entonces se actualizan los archivos y quedan accesibles. <br>---<br> Escenario 2: Error en documentación Dado que existen errores en los comentarios o formato, Cuando se ejecuta la herramienta, Entonces el sistema reporta los errores y solicita corrección. | - |

## 3.2. Impact Mapping
### Goal 1

<img src="/assets/images/chapter-III/Impact%20Mapping.png" alt="Impact Mapping 1" style="width: 900px; margin-right: 900px;"/>

### Goal 2

<img src="/assets/images/chapter-III/Impact%20Mapping%202.png" alt="Impact Mapping 2" style="width: 900px; margin-right: 900px;"/>

### Goal 3

<img src="/assets/images/chapter-III/Impact%20Mapping%203.png" alt="Impact Mapping 3" style="width: 900px; margin-right: 900px;"/>

### Goal 4

<img src="/assets/images/chapter-III/Impact%20Mapping%204.png" alt="Impact Mapping 4" style="width: 900px; margin-right: 900px;"/>

## 3.3. Product Backlog

A continuación se detalla el Product Backlog del proyecto EasyPark. El Product Backlog mostrara una lista ordenada de las user stories, priorizadas de acuerdo con el consenso del equipo. Para estimar la complejidad de cada tarea, empleamos la secuencia de Fibonacci (1, 2, 3, 5, 8) como referencia.

<table>
  <tr>
    <td><strong>#Orden</strong></td>
    <td><strong>User Story Id</strong></td>
    <td><strong>Título</strong></td>
    <td><strong>Descripción</strong></td>
    <td><strong>Story Points (1 / 2 / 3 / 5 / 8)</strong></td>
  </tr>
  <tr>
    <td>1</td>
    <td>US14</td>
    <td>Visualización de dashboard</td>
    <td>Como administrador quiero acceder a un dashboard central para ver el estado general de los estacionamientos</td>
    <td>5</td>
  </tr>
  <tr>
    <td>2</td>
    <td>US15</td>
    <td>Gestión visual de espacios</td>
    <td>Como operador quiero ver y actualizar el estado de los espacios (libre/ocupado/reservado) para mantener la información al día</td>
    <td>5</td>
  </tr>
  <tr>
    <td>3</td>
    <td>US17</td>
    <td>Gestión de reservas desde frontend</td>
    <td>Como usuario quiero reservar un espacio de estacionamiento desde la aplicación para asegurar disponibilidad</td>
    <td>5</td>
  </tr>
  <tr>
    <td>4</td>
    <td>US20</td>
    <td>Procesamiento de pagos frontend</td>
    <td>Como usuario quiero pagar mi estacionamiento desde la app usando distintos métodos para agilizar la salida</td>
    <td>5</td>
  </tr>
  <tr>
    <td>5</td>
    <td>US26</td>
    <td>API de gestión de espacios</td>
    <td>Como desarrollador quiero una API REST para gestionar los espacios de estacionamiento para integraciones externas y automatizaciones</td>
    <td>5</td>
  </tr>
  <tr>
    <td>6</td>
    <td>US27</td>
    <td>API de usuarios y roles</td>
    <td>Como desarrollador quiero endpoints para alta, baja, modificación y consulta de usuarios y roles para facilitar la administración</td>
    <td>5</td>
  </tr>
  <tr>
    <td>7</td>
    <td>US28</td>
    <td>API de pagos y reservas</td>
    <td>Como desarrollador quiero exponer endpoints para procesar pagos y gestionar reservas para integración con apps de terceros</td>
    <td>5</td>
  </tr>
  <tr>
    <td>8</td>
    <td>US32</td>
    <td>Gestión de backups y restauración</td>
    <td>Como responsable técnico quiero programar backups automáticos y restaurar datos para prevenir pérdidas</td>
    <td>5</td>
  </tr>
  <tr>
    <td>9</td>
    <td>US33</td>
    <td>Integración con sistemas de pago externos</td>
    <td>Como desarrollador quiero conectar EasyPark con pasarelas de pago externas para ampliar opciones de cobro</td>
    <td>5</td>
  </tr>
  <tr>
    <td>10</td>
    <td>US34</td>
    <td>Autenticación y autorización</td>
    <td>Como backend quiero implementar mecanismos robustos de autenticación y control de acceso para proteger los recursos</td>
    <td>5</td>
  </tr>
  <tr>
    <td>11</td>
    <td>US39</td>
    <td>Control de concurrencia</td>
    <td>Como backend quiero evitar conflictos por operaciones simultáneas sobre el mismo espacio para mantener la consistencia</td>
    <td>5</td>
  </tr>
  <tr>
    <td>12</td>
    <td>TS03</td>
    <td>Integración continua y despliegue automático</td>
    <td>Como equipo técnico quiero configurar pipelines de CI/CD para agilizar pruebas y despliegues en cada push</td>
    <td>5</td>
  </tr>
  <tr>
    <td>13</td>
    <td>TS04</td>
    <td>Seguridad y revisión de vulnerabilidades</td>
    <td>Como responsable técnico quiero analizar el código en busca de vulnerabilidades para proteger los datos y usuarios</td>
    <td>5</td>
  </tr>
  <tr>
    <td>14</td>
    <td>US11</td>
    <td>Registro de usuario</td>
    <td>Como operador o administrador quiero crear una cuenta en EasyPark para acceder a las funcionalidades del sistema</td>
    <td>3</td>
  </tr>
  <tr>
    <td>15</td>
    <td>US12</td>
    <td>Inicio de sesión</td>
    <td>Como usuario registrado quiero iniciar sesión de forma segura para acceder al panel de gestión</td>
    <td>3</td>
  </tr>
  <tr>
    <td>16</td>
    <td>US18</td>
    <td>Cancelación de reservas</td>
    <td>Como usuario quiero cancelar una reserva activa para liberar el espacio sin penalización (cuando aplica)</td>
    <td>3</td>
  </tr>
  <tr>
    <td>17</td>
    <td>US19</td>
    <td>Visualización de tarifas</td>
    <td>Como conductor quiero consultar las tarifas vigentes según horario y espacio para planificar mi pago</td>
    <td>3</td>
  </tr>
  <tr>
    <td>18</td>
    <td>US21</td>
    <td>Recepción de notificaciones</td>
    <td>Como usuario u operador quiero recibir notificaciones sobre reservas, pagos o incidencias para actuar a tiempo</td>
    <td>3</td>
  </tr>
  <tr>
    <td>19</td>
    <td>US22</td>
    <td>Gestión de incidencias</td>
    <td>Como operador quiero registrar y visualizar incidencias en el estacionamiento para dar seguimiento y solución</td>
    <td>3</td>
  </tr>
  <tr>
    <td>20</td>
    <td>US16</td>
    <td>Consulta de historial de ocupación</td>
    <td>Como administrador quiero ver el historial de ocupación de los espacios para analizar tendencias</td>
    <td>3</td>
  </tr>
  <tr>
    <td>21</td>
    <td>US29</td>
    <td>API de reportes y analíticas</td>
    <td>Como desarrollador quiero obtener reportes de ocupación, ingresos y uso para análisis externo</td>
    <td>3</td>
  </tr>
  <tr>
    <td>22</td>
    <td>US30</td>
    <td>Gestión de logs y auditoría</td>
    <td>Como administrador quiero acceder a registros de acciones críticas en el sistema para auditorías y seguridad</td>
    <td>3</td>
  </tr>
  <tr>
    <td>23</td>
    <td>US31</td>
    <td>Validación de integridad de datos</td>
    <td>Como backend quiero validar y proteger la integridad de los datos de ocupación y pagos para evitar errores y fraudes</td>
    <td>3</td>
  </tr>
  <tr>
    <td>24</td>
    <td>US35</td>
    <td>Monitoreo de disponibilidad</td>
    <td>Como responsable técnico quiero monitorear la disponibilidad y salud de los servicios backend para detectar caídas</td>
    <td>3</td>
  </tr>
  <tr>
    <td>25</td>
    <td>US37</td>
    <td>Gestión de incidencias desde backend</td>
    <td>Como backend quiero permitir registro y consulta de incidencias vía API para integración con sistemas de soporte</td>
    <td>3</td>
  </tr>
  <tr>
    <td>26</td>
    <td>US38</td>
    <td>Versionado de API</td>
    <td>Como desarrollador quiero que las APIs estén versionadas para evitar rupturas en integraciones existentes</td>
    <td>3</td>
  </tr>
  <tr>
    <td>27</td>
    <td>TS01</td>
    <td>Pruebas automatizadas frontend</td>
    <td>Como equipo técnico quiero implementar pruebas unitarias y de integración en frontend para asegurar la calidad de la interfaz</td>
    <td>3</td>
  </tr>
  <tr>
    <td>28</td>
    <td>TS02</td>
    <td>Pruebas automatizadas backend</td>
    <td>Como equipo técnico quiero desarrollar tests unitarios y de integración para backend para garantizar la robustez de servicios</td>
    <td>3</td>
  </tr>
  <tr>
    <td>29</td>
    <td>US23</td>
    <td>Edición de perfil de usuario</td>
    <td>Como usuario quiero modificar mis datos personales y de contacto para mantener mi perfil actualizado</td>
    <td>2</td>
  </tr>
  <tr>
    <td>30</td>
    <td>US25</td>
    <td>Cierre de sesión seguro</td>
    <td>Como usuario quiero cerrar mi sesión manualmente y automáticamente por inactividad para proteger mi cuenta</td>
    <td>2</td>
  </tr>
  <tr>
    <td>31</td>
    <td>US13</td>
    <td>Recuperación de contraseña</td>
    <td>Como usuario quiero recuperar mi contraseña olvidada para restablecer acceso a mi cuenta</td>
    <td>2</td>
  </tr>
  <tr>
    <td>32</td>
    <td>US24</td>
    <td>Soporte y ayuda online</td>
    <td>Como usuario quiero acceder a recursos de ayuda y soporte en la app para resolver dudas durante el uso</td>
    <td>2</td>
  </tr>
  <tr>
    <td>33</td>
    <td>US01</td>
    <td>Información general EasyPark</td>
    <td>Como visitante quiero ver una descripción clara de EasyPark en la landing page para entender de qué trata la solución</td>
    <td>2</td>
  </tr>
  <tr>
    <td>34</td>
    <td>US02</td>
    <td>Características destacadas</td>
    <td>Como potencial cliente quiero ver una lista de beneficios y características clave en la landing para decidir si EasyPark es adecuado para mi negocio</td>
    <td>2</td>
  </tr>
  <tr>
    <td>35</td>
    <td>US03</td>
    <td>Planes y precios</td>
    <td>Como interesado quiero consultar los planes y precios desde la landing para evaluar la oferta y tomar decisiones</td>
    <td>2</td>
  </tr>
  <tr>
    <td>36</td>
    <td>US04</td>
    <td>Formulario de contacto</td>
    <td>Como visitante quiero enviar una consulta o solicitar información a través de un formulario en la landing para recibir atención personalizada</td>
    <td>2</td>
  </tr>
  <tr>
    <td>37</td>
    <td>US05</td>
    <td>Testimonios de clientes</td>
    <td>Como visitante quiero conocer opiniones de otros usuarios para confiar en la solución EasyPark</td>
    <td>2</td>
  </tr>
  <tr>
    <td>38</td>
    <td>US06</td>
    <td>Preguntas frecuentes (FAQs)</td>
    <td>Como visitante quiero consultar un listado de preguntas frecuentes para resolver dudas rápidamente</td>
    <td>2</td>
  </tr>
  <tr>
    <td>39</td>
    <td>US36</td>
    <td>Generación automática de reportes</td>
    <td>Como administrador quiero recibir reportes automáticos por email para mantenerme actualizado sin ingresar al sistema</td>
    <td>2</td>
  </tr>
  <tr>
    <td>40</td>
    <td>US40</td>
    <td>Exportación de datos</td>
    <td>Como administrador quiero exportar datos históricos de ocupación, pagos y usuarios para análisis externo</td>
    <td>2</td>
  </tr>
  <tr>
    <td>41</td>
    <td>TS05</td>
    <td>Documentación técnica automatizada</td>
    <td>Como desarrollador quiero generar y mantener documentación técnica de APIs y arquitectura para facilitar el mantenimiento</td>
    <td>2</td>
  </tr>
  <tr>
    <td>42</td>
    <td>US07</td>
    <td>Acceso a demo o tour virtual</td>
    <td>Como potencial usuario quiero acceder a una demo interactiva o tour virtual para conocer cómo funciona EasyPark</td>
    <td>3</td>
  </tr>
  <tr>
    <td>43</td>
    <td>US08</td>
    <td>Enlaces a redes sociales</td>
    <td>Como visitante quiero encontrar enlaces a redes sociales oficiales para seguir novedades y contacto alternativo</td>
    <td>1</td>
  </tr>
  <tr>
    <td>44</td>
    <td>US09</td>
    <td>Registro de interés (newsletter)</td>
    <td>Como usuario interesado quiero dejar mi correo para recibir novedades y promociones para mantenerme informado</td>
    <td>1</td>
  </tr>
  <tr>
    <td>45</td>
    <td>US10</td>
    <td>Accesibilidad y responsive</td>
    <td>Como visitante quiero que la landing page funcione correctamente en cualquier dispositivo y sea accesible para tener una buena experiencia</td>
    <td>1</td>
  </tr>
</table>
