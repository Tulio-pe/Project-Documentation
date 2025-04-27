# Capítulo III: Requirements Specification

## 3.1. To-Be Scenario Mapping
>Segmento 1

<img src="./src/To-Be_segmento1.png " alt="To-Be_segmento1" style="display: block; margin: 50px auto 0 auto;"/> 

>Segmento 2

<img src="./src/To-be_segmento2.png " alt="To-be_segmento2" style="display: block; margin: 50px auto 0 auto;"/> 

## 3.2. User Stories
This section provides a collection of user stories that describe the functionalities and features from the end-user perspective.

## Historias de Usuario

| Epic/User Story ID | Título | Descripción | Criterios de Aceptación | Relacionado con (Epic ID) |
|--------------------|--------|-------------|-------------------------|---------------------------|
| US01 | Agendamiento de Citas en Talleres | Como propietario de un vehículo que necesita mantenimiento o reparación, quiero tener la posibilidad de buscar talleres disponibles, revisar sus horarios y agendar una cita directamente desde la plataforma, para evitar perder tiempo y asegurarme de que el taller esté disponible. | Given que el usuario ha iniciado sesión en la plataforma,<br> When accede a la sección de agendamiento,<br> Then puede buscar talleres y ver los disponibles. | |
| US02 | Notificaciones de Mantenimiento | Como propietario de un vehículo, quiero recibir notificaciones automáticas cuando se acerque la fecha de mantenimiento sugerida, para poder mantener mi vehículo en buen estado. | Given que el vehículo tiene una fecha programada de mantenimiento,<br> When se acerque dicha fecha,<br> Then el usuario recibirá una notificación en la plataforma o por correo electrónico. | |
| US03 | Historial de Servicios | Como usuario de la plataforma, quiero poder ver el historial de servicios realizados a mi vehículo, para tener un registro detallado de mantenimientos y reparaciones. | Given que el usuario accede a su perfil de vehículo,<br> When consulta el historial,<br> Then puede ver una lista con fechas, talleres y detalles de cada servicio realizado. | |
| US04 | Evaluación de Talleres | Como usuario, quiero poder calificar y dejar comentarios sobre los talleres que he utilizado, para ayudar a otros a tomar decisiones informadas. | Given que el usuario ha completado una cita en un taller,<br> When accede a la sección de evaluación,<br> Then puede dejar una calificación de 1 a 5 estrellas y un comentario. | |
| US05 | Gestión de Múltiples Vehículos | Como usuario que posee más de un vehículo, quiero poder registrar y gestionar varios vehículos en una misma cuenta, para administrarlos fácilmente desde un solo lugar. | Given que el usuario accede a su cuenta,<br> When entra a la sección de "Mis Vehículos",<br> Then puede añadir, editar o eliminar información de múltiples vehículos. | |
| US06 | Visualización en Tiempo Real del Servicio | Como usuario, quiero ver en tiempo real el estado y los avances del servicio realizado en mi vehículo, para mantenerme informado durante todo el proceso. | Given que el vehículo esté en servicio,<br> When el usuario acceda al seguimiento,<br> Then podrá ver actualizaciones del progreso en tiempo real. | |
| US07 | Acceso Rápido desde Landing | Como visitante de la landing page, quiero tener un botón "Ver Más" que me lleve directamente a la plataforma, para explorar más sobre los servicios ofrecidos. | Given que el visitante esté en la landing,<br> When haga clic en "Ver Más",<br> Then será redirigido a la aplicación web. | |
| US08 | Información sobre los Planes Disponibles | Como visitante de la landing page, quiero ver los diferentes planes ofrecidos (gratuito, premium, etc.), para escoger el que mejor se adapte a mis necesidades. | Given que el visitante esté en la landing,<br> When acceda a la sección de planes,<br> Then podrá visualizar y comparar las características de cada plan. | |
| US09 | Conocer al Equipo de Desarrollo | Como visitante, quiero poder leer quiénes son los desarrolladores del proyecto en la landing page, para generar mayor confianza en la plataforma. | Given que el visitante acceda a "Acerca de nosotros",<br> When consulte el equipo,<br> Then verá una breve descripción de los desarrolladores. | |
| US10 | Crear Cuenta como Cliente | Como usuario nuevo, quiero poder registrarme en la plataforma con mis datos personales y de mi vehículo, para acceder a todos los servicios disponibles. | Given que el usuario acceda a la página de registro,<br> When complete el formulario,<br> Then se creará una nueva cuenta asociada a su vehículo. | |
| US11 | Recuperar Contraseña | Como usuario registrado, quiero poder recuperar mi contraseña en caso de olvido, para volver a acceder a mi cuenta sin problemas. | Given que el usuario olvidó su contraseña,<br> When solicite recuperación,<br> Then recibirá un enlace para resetear su contraseña. | |
| US12 | Filtrar Talleres por Especialidad | Como usuario, quiero poder buscar talleres filtrándolos por especialidad (mecánica, pintura, frenos, etc.), para encontrar rápidamente el servicio que necesito. | Given que el usuario acceda a la búsqueda de talleres,<br> When seleccione un filtro de especialidad,<br> Then verá solo talleres que ofrecen ese servicio. | |
| US13 | Ver Detalles del Taller | Como usuario, quiero poder ver información detallada de cada taller (dirección, fotos, horarios, servicios), para decidir cuál visitar. | Given que el usuario vea un taller listado,<br> When haga clic en "ver detalles",<br> Then podrá acceder a su información completa. | |
| US14 | Notificación de Finalización de Servicio | Como usuario, quiero recibir una notificación inmediata cuando el servicio de mi vehículo haya finalizado, para poder recogerlo a tiempo. | Given que el taller marque el servicio como finalizado,<br> When eso ocurra,<br> Then el usuario recibirá una notificación en su cuenta o correo. | |
| US15 | Landing Page Responsiva | Como visitante, quiero que la landing page se vea bien tanto en computadora como en dispositivos móviles, para poder navegar cómodamente desde cualquier lugar. | Given que el visitante acceda desde cualquier dispositivo,<br> When abra la landing page,<br> Then verá una versión adaptada a su pantalla. | |


## 3.3. Impact Mapping

<img src="./src/Impact map 1.png " alt="Impact map 1" style="display: block; margin: 50px auto 0 auto;"/> 


## 3.4. Product Backlog
This section lists the prioritized product backlog items, including features, enhancements, and technical tasks.

## Product Backlog

| #Orden | User Story ID | Título | Descripción | Story Points |
|--------|---------------|--------|-------------|--------------|
| 1 | US01 | Agendamiento de Citas en Talleres | Agendar citas en talleres disponibles. | 8 |
| 2 | US02 | Notificaciones de Mantenimiento | Recibir alertas de mantenimiento de vehículo. | 5 |
| 3 | US03 | Historial de Servicios | Consultar historial de servicios de un vehículo. | 5 |
| 4 | US04 | Evaluación de Talleres | Dejar calificaciones y comentarios sobre talleres. | 5 |
| 5 | US05 | Gestión de Múltiples Vehículos | Registrar y administrar varios vehículos. | 8 |
| 6 | US06 | Visualización en Tiempo Real del Servicio | Ver en tiempo real qué se le está haciendo al vehículo. | 13 |
| 7 | US07 | Acceso Rápido desde Landing | Botón "Ver Más" que redirige a la app. | 3 |
| 8 | US08 | Información sobre los Planes Disponibles | Mostrar y comparar planes de servicio en la landing. | 5 |
| 9 | US09 | Conocer al Equipo de Desarrollo | Sección en landing con información del equipo. | 3 |
| 10 | US10 | Crear Cuenta como Cliente | Registro de nuevos usuarios y vehículos. | 8 |
| 11 | US11 | Recuperar Contraseña | Sistema de recuperación de contraseñas olvidadas. | 5 |
| 12 | US12 | Filtrar Talleres por Especialidad | Filtros de búsqueda por tipo de servicio. | 5 |
| 13 | US13 | Ver Detalles del Taller | Vista completa de información de talleres. | 5 |
| 14 | US14 | Notificación de Finalización de Servicio | Notificación de término de servicio del vehículo. | 5 |
| 15 | US15 | Landing Page Responsiva | Diseño adaptable a computadoras y móviles. | 5 |

