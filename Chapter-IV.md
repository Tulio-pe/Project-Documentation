# Capítulo IV: Product Design

## 4.1. Style Guidelines

Nuestra plataforma Tallerazo tiene como objetivo principal transformar la experiencia del servicio automotriz, conectando a conductores y talleres de manera eficiente, confiable y digitalizada. A través de una interfaz moderna y simple e intuitiva, Tallerazo permite agendar citas, realizar seguimientos en tiempo real y mantener una comunicación directa entre ambas partes. El diseño visual de nuestro sistema está centrado en generar confianza, facilitar la navegación y transmitir innovación tecnológica. Se busca ofrecer a los usuarios una experiencia intuitiva, accesible y profesional, entregándoles transparencia y la interacción fluida en cada punto de contacto. Nuestra línea visual apunta a mantener una identidad limpia, clara y moderna, utilizando colores que transmiten frescura y profesionalismo, tipografías fácilmente entendibles y una estructura de contenidos optimizada para diferentes dispositivos.

### 4.1.1. General Style Guidelines:

### 🟩Typography:
Se hará uso de la tipografía Inter. Este tipo de letra es moderna, profesional y altamente legible, diseñada especialmente para pantallas digitales. Inter ofrece una excelente lectura en diferentes dispositivos y resoluciones, gracias a su estructura limpia, sus proporciones equilibradas y su optimización para contenido web y móvil. Es ideal para títulos, subtítulos y cuerpos de texto, permitiendo transmitir un tono confiable y accesible.

![inter](https://github.com/user-attachments/assets/b92b18bf-d88f-4018-ae2e-67b2edbbcd60)

### 🟩Colors:
La paleta de colores de Tallerazo está basada en tonos de azul y verde, transmitiendo modernidad, confianza y tecnología. El fondo blanco y los acentos en azul y verde permiten una navegación ligera y placentera, evitando la saturación visual.
## Principal:

#1D4ED8 – Azul intenso: Para botones principales y llamadas a la acción.

#22C55E – Verde brillante: Para destacar acciones positivas o confirmaciones.

Fondo:

#FFFFFF – Blanco: Color de fondo predominante para mantener una sensación de limpieza.

![color](https://github.com/user-attachments/assets/c358631c-53cb-4a4e-9d5c-6fadff203dcd) ![color2](https://github.com/user-attachments/assets/8a3796eb-d827-4fb9-969e-4c25b1efc32e) ![color3](https://github.com/user-attachments/assets/4d3842c5-7cd2-4888-b6ff-7db196b3222a) ![color4](https://github.com/user-attachments/assets/5aa18b36-34d3-46a6-8d65-1f3e7a6f9476) 

### Tone of Communication:

✅Confiable: Se priorizará un lenguaje que transmita seguridad, respaldando cada interacción entre usuario y taller.

✅Ágil: El tono será claro y directo, permitiendo a los usuarios encontrar soluciones o acciones rápidamente.

✅Humano: El estilo será cercano y accesible, buscando generar una conexión genuina.

✅Profesional: Se mantendrá siempre un enfoque formal y técnico en secciones como condiciones de servicio, políticas y soporte.

✅Motivador: Se destacarán logros como el seguimiento exitoso de un servicio o el cumplimiento de citas.



### 4.1.2. Web Style Guidelines

Dado que Tallerazo está enfocado en facilitar el acceso a servicios automotrices de manera ágil, la interfaz web ha sido diseñada para ofrecer una navegación limpia y sin distracciones. Se prioriza la simplicidad, evitando el exceso de botones o elementos saturados. La landing page cumple una función de recepción, informando de forma clara las ventajas de la plataforma y guiando al usuario rápidamente a la acción deseada: registrarse y agendar su primera cita. El uso de fondos blancos, degradados suaves en azul y verde, y botones destacados en azul intenso, permite un entorno visualmente agradable, moderno y fácil de usar tanto en computadoras como en móviles.

![landing](https://github.com/user-attachments/assets/20d49669-5b8e-4fc0-8251-c8c6803850de)


## 4.2. Information Architecture:

La arquitectura de la información de Tallerazo ha sido diseñada para ofrecer una experiencia simple, intuitiva y confiable, enfocada en conectar a propietarios de vehículos con talleres automotrices de manera eficiente y transparente. La organización y etiquetado del contenido permiten a los usuarios identificar rápidamente los servicios, agendar citas y seguir el estado de sus reparaciones, priorizando la facilidad de uso, el control del proceso y la confianza. Esta arquitectura se implementa mediante jerarquías visuales claras, categorización por funciones específicas, acciones directas y navegación centrada en el usuario.

### 4.2.1. Organization Systems:


### 4.2.2. Labeling Systems
Lineamientos para los sistemas de etiquetado.

### 4.2.3. SEO Tags and Meta Tags
Uso de etiquetas SEO y metaetiquetas para optimización.

### 4.2.4. Searching Systems
Diseño y funcionalidad de los sistemas de búsqueda.

### 4.2.5. Navigation Systems
Estructura y diseño de los sistemas de navegación.

## 4.3. Landing Page UI Design

### 4.3.1. Landing Page Wireframe
Esquema inicial de la página de aterrizaje.

### 4.3.2. Landing Page Mock-up
Prototipo visual de la página de aterrizaje.

## 4.4. Web Applications UX/UI Design

### 4.4.1. Web Applications Wireframes
Esquemas iniciales para aplicaciones web.

### 4.4.2. Web Applications Wireflow Diagrams
Diagramas de flujo de interacción para aplicaciones web.

### 4.4.3. Web Applications Mock-ups
Prototipos visuales para aplicaciones web.

### 4.4.4. Web Applications User Flow Diagrams
Diagramas de flujo de usuario para aplicaciones web.

## 4.5. Web Applications Prototyping
Proceso de creación de prototipos para aplicaciones web.

## 4.6. Domain-Driven Software Architecture

### 4.6.1. Software Architecture Context Diagram
Diagrama de contexto de la arquitectura de software.

### 4.6.2. Software Architecture Container Diagrams
Diagramas de contenedores de la arquitectura de software.

### 4.6.3. Software Architecture Components Diagrams
Diagramas de componentes de la arquitectura de software.

## 4.7. Software Object-Oriented Design

### 4.7.1. Class Diagrams
Diagramas de clases para el diseño orientado a objetos.
![Diagram class](https://github.com/Tulio-pe/Project-Documentation/blob/main/src/class%20diagram.jpeg)

### 4.7.2. Class Dictionary
<h3>Class User</h3>
<table border="1">
  <tr><th>Visibility</th><th>Name</th><th>Type</th><th>Description</th></tr>
  <tr><td>private</td><td>userId</td><td>int</td><td>User ID</td></tr>
  <tr><td>private</td><td>name</td><td>string</td><td>Full name</td></tr>
  <tr><td>private</td><td>email</td><td>string</td><td>Email address</td></tr>
  <tr><td>private</td><td>password</td><td>string</td><td>User password</td></tr>
  <tr><td>private</td><td>role</td><td>UserRole</td><td>User role</td></tr>
  <tr><td>public</td><td>login()</td><td>void</td><td>Logs the user into the system</td></tr>
  <tr><td>public</td><td>updateProfile()</td><td>void</td><td>Updates user profile information</td></tr>
</table>

<h3>Class Client</h3>
<table border="1">
  <tr><th>Visibility</th><th>Name</th><th>Type</th><th>Description</th></tr>
  <tr><td>private</td><td>dni</td><td>string</td><td>National identity document</td></tr>
  <tr><td>private</td><td>city</td><td>string</td><td>City of residence</td></tr>
</table>

<h3>Class WorkshopAdministrator</h3>
<table border="1">
  <tr><th>Visibility</th><th>Name</th><th>Type</th><th>Description</th></tr>
  <tr><td>private</td><td>workshopId</td><td>int</td><td>Workshop ID</td></tr>
  <tr><td>private</td><td>workshopName</td><td>string</td><td>Workshop name</td></tr>
  <tr><td>private</td><td>address</td><td>string</td><td>Workshop address</td></tr>
</table>

<h3>Class Mechanic</h3>
<table border="1">
  <tr><th>Visibility</th><th>Name</th><th>Type</th><th>Description</th></tr>
  <tr><td>private</td><td>specialty</td><td>string</td><td>Mechanic specialty</td></tr>
</table>

<h3>Class Workshop</h3>
<table border="1">
  <tr><th>Visibility</th><th>Name</th><th>Type</th><th>Description</th></tr>
  <tr><td>private</td><td>workshopId</td><td>int</td><td>Workshop ID</td></tr>
  <tr><td>private</td><td>name</td><td>string</td><td>Workshop name</td></tr>
  <tr><td>private</td><td>address</td><td>string</td><td>Workshop address</td></tr>
  <tr><td>private</td><td>description</td><td>string</td><td>Workshop description</td></tr>
</table>

<h3>Class Appointment</h3>
<table border="1">
  <tr><th>Visibility</th><th>Name</th><th>Type</th><th>Description</th></tr>
  <tr><td>private</td><td>appointmentId</td><td>int</td><td>Appointment ID</td></tr>
  <tr><td>private</td><td>dateTime</td><td>DateTime</td><td>Date and time of the appointment</td></tr>
  <tr><td>private</td><td>status</td><td>AppointmentStatus</td><td>Current status of the appointment</td></tr>
</table>

<h3>Class Vehicle</h3>
<table border="1">
  <tr><th>Visibility</th><th>Name</th><th>Type</th><th>Description</th></tr>
  <tr><td>private</td><td>vehicleId</td><td>int</td><td>Vehicle ID</td></tr>
  <tr><td>private</td><td>licensePlate</td><td>string</td><td>License plate number</td></tr>
  <tr><td>private</td><td>brand</td><td>string</td><td>Vehicle brand</td></tr>
  <tr><td>private</td><td>model</td><td>string</td><td>Vehicle model</td></tr>
  <tr><td>private</td><td>year</td><td>int</td><td>Manufacture year</td></tr>
  <tr><td>private</td><td>color</td><td>string</td><td>Vehicle color</td></tr>
</table>

<h3>Class Maintenance</h3>
<table border="1">
  <tr><th>Visibility</th><th>Name</th><th>Type</th><th>Description</th></tr>
  <tr><td>private</td><td>maintenanceId</td><td>int</td><td>Maintenance ID</td></tr>
  <tr><td>private</td><td>description</td><td>string</td><td>Description of the maintenance</td></tr>
  <tr><td>private</td><td>status</td><td>string</td><td>Maintenance status</td></tr>
  <tr><td>private</td><td>estimatedCost</td><td>float</td><td>Estimated cost</td></tr>
</table>

<h3>Class Review</h3>
<table border="1">
  <tr><th>Visibility</th><th>Name</th><th>Type</th><th>Description</th></tr>
  <tr><td>private</td><td>reviewId</td><td>int</td><td>Review ID</td></tr>
  <tr><td>private</td><td>rating</td><td>int</td><td>Rating score</td></tr>
  <tr><td>private</td><td>comment</td><td>string</td><td>Client comment</td></tr>
  <tr><td>private</td><td>date</td><td>Date</td><td>Date of submission</td></tr>
</table>

<h3>Class ChatMessage</h3>
<table border="1">
  <tr><th>Visibility</th><th>Name</th><th>Type</th><th>Description</th></tr>
  <tr><td>private</td><td>messageId</td><td>int</td><td>Message ID</td></tr>
  <tr><td>private</td><td>content</td><td>string</td><td>Message content</td></tr>
  <tr><td>private</td><td>dateTime</td><td>DateTime</td><td>Date and time of sending</td></tr>
</table>

<h3>Class UserRole (Enum)</h3>
<table border="1">
  <tr><th>Value</th><th>Description</th></tr>
  <tr><td>CLIENT</td><td>Client role</td></tr>
  <tr><td>WORKSHOP_ADMIN</td><td>Workshop administrator role</td></tr>
  <tr><td>MECHANIC</td><td>Mechanic role</td></tr>
</table>

<h3>Class AppointmentStatus (Enum)</h3>
<table border="1">
  <tr><th>Value</th><th>Description</th></tr>
  <tr><td>PENDING</td><td>Pending appointment</td></tr>
  <tr><td>CONFIRMED</td><td>Confirmed appointment</td></tr>
  <tr><td>IN_PROGRESS</td><td>Ongoing service</td></tr>
  <tr><td>COMPLETED</td><td>Completed service</td></tr>
  <tr><td>CANCELLED</td><td>Cancelled appointment</td></tr>
</table>


## 4.8. Database Design

### 4.8.1. Database Diagram
Diagrama de la base de datos:

![Diagram data base](https://github.com/Tulio-pe/Project-Documentation/blob/main/src/Diagram%20data%20base.jpeg)

Enlace del diagrama: https://editor.plantuml.com/uml/hLN1Qjmm4Bqlx3-8FRMKGDgobn12bar2IqbfboNjpIZIP2DgIOuanvXi_hrZMKvaMquRoCqpRpJpvir8FhME6bVAV3u3vOIhoJeN-4KUvZD2FZ1lP8AJ8_Br-vOS7__uTdBIG3V2M9SfAW6XgzLc_MMrURSyVDzWEPs4k1AHy-FIErbJTnHQMZ2399zRfA3MLjhmEDDX0ptEPyzzKDCrGKsgWt5l5m4fSkgWbzoNlJPKyJ5FgJdaOtSDIC1dziLqhisu4mwM6L4ueLK4VbeEc_cbpHzxgulGKHNCL5i3oLfX2A6S6x2s9twBc9AX5rtRVirBAfG3HHM3K5O-UvA2zdNkr4oHxR1-_zlptruit4bNsg5QCRUVfSQOvbJBxAwpKxmcQ7SScBOEdPTQGTtOO9sGk00yu-qQdAssvmDfWDrI9LYdIp3Vy9vCYvRYaOrdbT8XGVFYVpIQs8erPjjrzPWtNdVFdWZzQq9jxlIo6BWhSMJJmzh0lO0gq3JUU2NDbzaPN3orYw-wbCqB6bFqHSSCmrkxtnySw0V_OXsHXQwKNI26LW3YwMA00GRY7fgWftSX7OcwyTm7na0Jkzz7TyX79jDrUuuH88jSrpvNvnr4POFg-4gBdG9Ed4umUE5WgnSUlAuNOvd66-YF-2qOj1hmH-qRdYedr8qsqYPAXTN1cCe8bnIo5nLDvXGKzx_Llm00
