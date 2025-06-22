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
| US01 | Registrar cuenta de gestor | Como gestor de taller, quiero registrarme en la plataforma, para obtener una cuenta que me permita acceder a mis funciones. | **Scenario:** Registro exitoso de gestor<br>**Given** el gestor está en el formulario "Registro"<br>**When** completa email, firstname, lastname, username y password (≥ 6 caracteres)<br>**And** el email y el username no existen en la base de datos<br>**And** pulsa "Registrarse"<br>**Then** el sistema guarda la cuenta con la contraseña encriptada (bcrypt)<br>**And** redirige al inicio de sesión | |
| US02 | Iniciar sesión | Como gestor de taller, quiero iniciar sesión con mis credenciales, para acceder a la plataforma. | **Scenario:** Inicio de sesión válido<br>**Given** el gestor está en la pantalla "Login"<br>**When** ingresa email y password correctos<br>**Then** el sistema emite un JWT<br>**And** redirige al dashboard u onboarding según corresponda<br><br>**Scenario:** Inicio de sesión inválido<br>**Given** el gestor está en la pantalla "Login"<br>**When** ingresa email o password incorrectos<br>**Then** el sistema muestra "Credenciales inválidas"<br>**And** permanece en la misma pantalla | |
| US03 | Actualizar perfil personal | Como gestor de taller, quiero actualizar mis datos personales, para mantener mi información al día. | **Scenario:** Actualización exitosa del perfil<br>**Given** el gestor está autenticado y en "Mi perfil"<br>**When** modifica firstname, lastname o username (dejando email y password sin cambios)<br>**And** el nuevo username no existe en otro usuario<br>**And** pulsa "Guardar"<br>**Then** el sistema actualiza los datos en la base de datos<br>**And** muestra el mensaje "Datos actualizados" | |
| US04 | Cerrar sesión | Como gestor de taller, quiero cerrar sesión, para finalizar mi acceso de forma segura. | **Scenario:** Cierre de sesión<br>**Given** el gestor está autenticado en la plataforma<br>**When** pulsa "Cerrar sesión"<br>**Then** el sistema invalida el JWT actual<br>**And** redirige al inicio de sesión<br>**And** muestra "Sesión cerrada" | |
| US05 | Registrar información del taller | Como gestor de taller, quiero registrar la información básica de mi taller, para que aparezca en la plataforma y los clientes puedan encontrarlo. | **Scenario:** Registro exitoso del taller<br>**Given** el gestor está en el formulario "Registrar taller"<br>**When** completa photo (png/jpg), address, email, name, phone, description y selecciona ubicación Región → Provincia → Distrito → Ciudad<br>**And** el email tiene formato válido y todos los campos son obligatorios<br>**Then** el sistema guarda la ficha del taller en la BD<br>**And** muestra el mensaje "Taller registrado" | |
| US06 | Editar información del taller | Como gestor de taller, quiero editar la información básica de mi taller cuando cambie, para mantener en la plataforma datos siempre correctos y actualizados. | **Scenario:** Actualización de datos del taller<br>**Given** el gestor abre la pantalla "Editar taller" y los campos se autocompletan<br>**When** modifica photo, address, description, email, name, phone o ubicación (cascada Región → Provincia → Distrito → Ciudad)<br>**And** pulsa "Guardar"<br>**Then** el sistema actualiza la información del taller en la BD<br>**And** muestra el mensaje "Taller actualizado" | |
| US07 | Configurar horarios regulares | Como gestor de taller, quiero configurar los días y horarios regulares de atención de mi taller, para que los clientes sepan cuándo pueden agendar una cita. | **Scenario:** Definir horarios iniciales<br>**Given** el gestor está en la sección "Horarios"<br>**When** añade entradas para cada día de la semana con StartTime y EndTime válidos (StartTime < EndTime, ≤ 24 h)<br>**And** puede marcar un día como "No atiende" mediante Enabled = false<br>**Then** el sistema guarda la lista completa en la BD<br>**And** muestra confirmación de guardado | |
| US08 | Actualizar horarios de atención | Como gestor de taller, quiero actualizar los días y horarios de atención cuando cambien, para mantener la información siempre al día. | **Scenario:** Edición de horarios existentes<br>**Given** el gestor abre "Editar horarios" y las entradas existentes se cargan<br>**When** modifica StartTime, EndTime, Enabled o añade/elimina días<br>**And** pulsa "Guardar"<br>**Then** el sistema persiste los cambios en la BD<br>**And** muestra el mensaje "Horarios actualizados" | |
| US09 | Explorar talleres filtrados | Como conductor, quiero explorar una lista de talleres filtrada por región → provincia → distrito → ciudad (o por mi ubicación actual), para encontrar rápidamente uno cercano. | **Scenario:** Filtrar por ciudad y listar talleres<br>**Given** el conductor está en la pantalla "Explorar talleres"<br>**When** no ha seleccionado aún la cascada completa Región → Provincia → Distrito → Ciudad<br>**Then** el sistema muestra "Selecciona tu ciudad para ver talleres disponibles"<br><br>**Scenario:** Mostrar resultados de la ciudad seleccionada<br>**Given** el conductor selecciona una ciudad válida en el filtro<br>**When** la API devuelve talleres de esa ciudad<br>**Then** el sistema muestra cards con photo miniatura, name, short description, address y botón "Ver más"<br><br>**Scenario:** Sin talleres en la ciudad<br>**Given** el conductor selecciona una ciudad sin talleres<br>**Then** el sistema muestra "No se encontraron talleres en esta ubicación" | |
| US10 | Ver detalle de taller | Como conductor, quiero ver la ficha detallada de un taller seleccionado, para decidir si se ajusta a mis necesidades. | **Scenario:** Visualizar detalle y contactar<br>**Given** el conductor está en la lista de talleres filtrados<br>**When** pulsa el botón "Ver más" de un taller<br>**Then** se abre la página de detalle del taller con photo grande, name, description extendida, address, email, phone<br>**And** se listan los horarios (DayOfWeek, Start–End, Enabled)<br>**And** hay un botón "Contactar" que abre https://wa.me/&lt;phone&gt; en nueva pestaña<br>**And** un enlace "← Volver" regresa al listado conservando el filtro<br>**And** si algún campo está vacío se muestra "Información no disponible" | |
| US11 | Registrar vehículo | Como gestor de taller, quiero registrar un vehículo de cliente (carBrand, carModel, fuelType, licensePlate, year), para poder asociarlo luego a órdenes de reparación. | **Scenario:** Registro exitoso de vehículo<br>**Given** el gestor está en el formulario "Registrar vehículo"<br>**When** completa carBrand, carModel, fuelType, licensePlate y year (1980 – año actual)<br>**And** la placa no existe en otro vehículo del taller<br>**Then** el sistema guarda el vehículo en la BD<br>**And** muestra "Vehículo registrado" | |
| US12 | Listar vehículos del taller | Como gestor de taller, quiero listar mis vehículos registrados, para ver rápidamente los que ya están cargados o crear uno nuevo. | **Scenario:** Sin vehículos registrados<br>**Given** el gestor accede a "Mis vehículos"<br>**And** no hay vehículos en la BD<br>**Then** el sistema muestra "Aún no tienes vehículos registrados" y un botón "Registrar vehículo"<br><br>**Scenario:** Con vehículos registrados<br>**Given** existen vehículos asociados al taller<br>**Then** el sistema muestra cards con carBrand, carModel, licensePlate, year y color (si existe), cada una con botón "Crear reparación" | |
| US13 | Crear orden de reparación | Como gestor de taller, quiero crear una orden de reparación a partir de un vehículo, para llevar el control del trabajo. | **Scenario:** Creación de reparación cuando no existe una abierta<br>**Given** el gestor visualiza un vehículo sin reparaciones abiertas<br>**When** pulsa "Crear reparación"<br>**Then** el sistema genera *repairCode* = *licensePlate-NN* (correlativo por vehículo)<br>**And** crea la reparación con estado inicial "Por revisar" y *updatedAt* actual<br><br>**Scenario:** Reparación abierta impide una nueva<br>**Given** el vehículo ya tiene una reparación no entregada<br>**Then** el botón "Crear reparación" aparece deshabilitado<br>**And** muestra el tooltip "Ya existe una reparación abierta" | |
| US14 | Cambiar estado de reparación | Como gestor de taller, quiero cambiar el estado de una reparación entre Por revisar → En revisión → Revisado → Entregado, para reflejar su avance. | **Scenario:** Avanzar al siguiente estado<br>**Given** el gestor está en la orden con estado actual *S* (donde *S* ≠ "Entregado")<br>**When** selecciona avanzar al siguiente estado permitido<br>**Then** el sistema actualiza el estado<br>**And** registra la fecha y hora en *updatedAt*<br><br>**Scenario:** Cerrar reparación al marcar "Entregado"<br>**Given** la reparación está en estado "Revisado"<br>**When** el gestor marca "Entregado"<br>**Then** la reparación queda cerrada<br>**And** el botón "Crear reparación" se habilita de nuevo para ese vehículo | |
| US15 | Filtrar reparaciones por estado | Como gestor de taller, quiero filtrar mis reparaciones por estado, para ver rápidamente qué autos requieren atención. | **Scenario:** Filtrar reparaciones exitosamente<br>**Given** el gestor está en la vista de reparaciones y elige un estado (Por revisar, En revisión, Revisado, Entregado, Todas)<br>**When** selecciona el estado<br>**Then** la lista se actualiza en ≤ 1 s mostrando solo las reparaciones que coinciden<br><br>**Scenario:** Sin reparaciones para el estado elegido<br>**Given** el gestor selecciona un estado sin coincidencias<br>**Then** el sistema muestra "Sin resultados" | |
| US16 | Tracking de reparación (conductor) | Como conductor, quiero ingresar el código de seguimiento (repairCode) que me dio el taller, para conocer el estado de la reparación de mi vehículo. | **Scenario:** Código válido<br>**Given** el conductor está en la pantalla "Tracking"<br>**When** ingresa un *repairCode* existente en formato *LICENSE-NN*<br>**Then** el sistema redirige a la vista Detalle de reparación<br><br>**Scenario:** Código inexistente<br>**Given** el conductor está en la pantalla "Tracking"<br>**When** ingresa un *repairCode* que no existe<br>**Then** el sistema muestra "Código no encontrado" | |
| US17 | Ver detalle de reparación | Como conductor, quiero ver el estado actual y los detalles de mi reparación, para estar informado sin llamar ni visitar el taller. | **Scenario:** Visualizar detalles de la reparación<br>**Given** el conductor accede a la página de detalle usando un *repairCode* válido<br>**Then** el sistema muestra:<br> • Estado (Por revisar / En revisión / Revisado / Entregado)<br> • *UpdatedAt* (fecha y hora de la última actualización)<br> • Datos del vehículo: *carBrand, carModel, fuelType, licensePlate, year*<br> • Datos del taller: *name, dirección completa, ciudad/distrito*<br>**And** presenta un botón "Contactar taller" que abre `https://wa.me/<phone>` en nueva pestaña<br>**And** si el estado es "Entregado", se destaca con un icono/etiqueta verde y el botón de contacto permanece disponible | |


















## 3.3. Impact Mapping

<img src="./src/Impact map 1.png " alt="Impact map 1" style="display: block; margin: 50px auto 0 auto;"/> 


## 3.4. Product Backlog
This section lists the prioritized product backlog items, including features, enhancements, and technical tasks.

## Product Backlog

| #Orden | User Story ID | Título | Descripción (resumen) | Story Points |
|--------|---------------|--------|-----------------------|--------------|
| 1 | **US01** | Registrar cuenta de gestor | Alta de usuario gestor (email, username únicos, pwd ≥ 6, bcrypt) | **5** |
| 2 | **US02** | Iniciar sesión | Autenticación (JWT) y ruteo a dashboard / onboarding | **3** |
| 3 | **US03** | Actualizar perfil personal | Cambiar firstname, lastname, username | **2** |
| 4 | **US04** | Cerrar sesión | Invalidar JWT y redirigir al login | **1** |
| 5 | **US05** | Registrar taller | Formulario completo + cascada Región → Ciudad + validaciones | **8** |
| 6 | **US06** | Editar taller | Actualizar datos del taller con autocompletado | **5** |
| 7 | **US07** | Configurar horarios | Crear calendario regular de atención con validaciones | **5** |
| 8 | **US08** | Actualizar horarios | Modificar o eliminar entradas de horario existentes | **3** |
| 9 | **US09** | Explorar talleres filtrados | Búsqueda por Región → Ciudad y cards de resultado | **5** |
| 10 | **US10** | Ver detalle de taller | Ficha completa + horarios + botón WhatsApp | **3** |
| 11 | **US11** | Registrar vehículo | Alta de vehículo (placa única, año válido) | **5** |
| 12 | **US12** | Listar vehículos | Cards de vehículos + botón “Crear reparación” | **3** |
| 13 | **US13** | Crear orden de reparación | Generar `repairCode` y estado inicial “Por revisar” | **8** |
| 14 | **US14** | Cambiar estado de reparación | Flujo Por revisar→En revisión→Revisado→Entregado con `updatedAt` | **5** |
| 15 | **US15** | Filtrar reparaciones | Lista filtrable por estado, respuesta ≤ 1 s | **3** |
| 16 | **US16** | Tracking de reparación (conductor) | Campo `repairCode`, validación y redirección | **3** |
| 17 | **US17** | Ver detalle de reparación | Estado + vehículo + taller + botón WhatsApp | **3** |


