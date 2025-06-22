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
| US05 | Registrar cuenta de gestor | Como gestor de taller, quiero registrarme en la plataforma, para obtener una cuenta que me permita acceder a mis funciones. | ```gherkin
Scenario: Registro exitoso de gestor
  Given el gestor está en el formulario "Registro"
  When completa email, firstname, lastname, username y password (>= 6 caracteres)
  And el email y el username no existen en la base de datos
  And pulsa "Registrarse"
  Then el sistema guarda la cuenta con la contraseña encriptada (bcrypt)
  And redirige al inicio de sesión
``` | |
| US06 | Iniciar sesión | Como gestor de taller, quiero iniciar sesión con mis credenciales, para acceder a la plataforma. | ```gherkin
Scenario: Inicio de sesión válido
  Given el gestor está en la pantalla "Login"
  When ingresa email y password correctos
  Then el sistema emite un JWT
  And redirige al dashboard si ya registró taller
  And redirige al onboarding si aún no lo hizo

Scenario: Inicio de sesión inválido
  Given el gestor está en la pantalla "Login"
  When ingresa email o password incorrectos
  Then el sistema muestra "Credenciales inválidas"
  And permanece en la misma pantalla
``` | |
| US07 | Actualizar perfil personal | Como gestor de taller, quiero actualizar mis datos personales, para mantener mi información al día. | ```gherkin
Scenario: Actualización exitosa del perfil
  Given el gestor está autenticado y en "Mi perfil"
  When modifica firstname, lastname o username (dejando email y password sin cambios)
  And el nuevo username no existe en otro usuario
  And pulsa "Guardar"
  Then el sistema actualiza los datos en la base de datos
  And muestra el mensaje "Datos actualizados"
``` | |
| US08 | Cerrar sesión | Como gestor de taller, quiero cerrar sesión, para finalizar mi acceso de forma segura. | ```gherkin
Scenario: Cierre de sesión
  Given el gestor está autenticado en la plataforma
  When pulsa "Cerrar sesión"
  Then el sistema invalida el JWT actual
  And redirige al inicio de sesión
  And muestra "Sesión cerrada"
``` | |



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

