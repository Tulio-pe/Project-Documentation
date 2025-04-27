## 4.1. Style Guidelines

Nuestra plataforma Tallerazo tiene como objetivo principal transformar la experiencia del servicio automotriz, conectando a conductores y talleres de manera eficiente, confiable y digitalizada. A través de una interfaz moderna y simple e intuitiva, Tallerazo permite agendar citas, realizar seguimientos en tiempo real y mantener una comunicación directa entre ambas partes. El diseño visual de nuestro sistema está centrado en generar confianza, facilitar la navegación y transmitir innovación tecnológica. Se busca ofrecer a los usuarios una experiencia intuitiva, accesible y profesional, entregándoles transparencia y la interacción fluida en cada punto de contacto. Nuestra línea visual apunta a mantener una identidad limpia, clara y moderna, utilizando colores que transmiten frescura y profesionalismo, tipografías fácilmente entendibles y una estructura de contenidos optimizada para diferentes dispositivos.

### 4.1.1. General Style Guidelines:

### 🟩Branding:

Tallerazo es una plataforma que conecta a propietarios de vehículos con talleres automotrices de confianza, ofreciendo una experiencia digital moderna y segura. Su identidad visual refleja los valores de eficiencia, transparencia y profesionalismo.
El diseño busca transmitir confianza y dinamismo, utilizando una interfaz limpia, moderna y enfocada en la acción rápida. Con una paleta de colores frescos en azul y verde, combinada con elementos gráficos claros como el automóvil y la llave inglesa, la aplicación facilita la navegación, la gestión de servicios y la conexión directa entre conductor y taller.

![Tallerazo logo](https://github.com/user-attachments/assets/d74f5970-bed6-4bdc-b806-03d5555758fe)

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

![landing](./src/chapter-4/landing/design_hero-section.png)

## 4.2. Information Architecture:

La arquitectura de la información de Tallerazo ha sido diseñada para ofrecer una experiencia simple, intuitiva y confiable, enfocada en conectar a propietarios de vehículos con talleres automotrices de manera eficiente y transparente. La organización y etiquetado del contenido permiten a los usuarios identificar rápidamente los servicios, agendar citas y seguir el estado de sus reparaciones, priorizando la facilidad de uso, el control del proceso y la confianza. Esta arquitectura se implementa mediante jerarquías visuales claras, categorización por funciones específicas, acciones directas y navegación centrada en el usuario.

### 4.2.1. Organization Systems:

Hemos diseñado el sistema de organización de tallerazo para atender las necesidades específicas de los dos principales perfiles de usuarios: propietarios de vehículos (clientes) y talleres automotrices (proveedores). Aunque ambas audiencias acceden a funcionalidades similares, el enfoque y flujo de navegación cambia de acuerdo al tipo de usuario, garantizando una experiencia personalizada.

## Propietarios de Vehículos:

Los usuarios acceden a una interfaz pensada para facilitar la gestión de citas, el seguimiento de servicios y la comunicación directa con talleres. Se utiliza una estructura jerárquica que destaca primero las acciones prioritarias y los estados activos del vehículo.

🟩Inicio: Organización matricial de módulos visuales que muestra servicios disponibles, próximos seguimientos, citas activas y mensajes recientes del taller. Cada sección permite un acceso inmediato a las acciones principales.

🟩Agenda de Citas: Visualización jerárquica tipo calendario que presenta las citas programadas, con opciones rápidas para reprogramar o cancelar.

🟩Seguimiento de Servicio: Organización secuencial que permite al usuario ver el progreso de su vehículo en tiempo real, detallando fases de diagnóstico, reparación y finalización.

🟩Historial del Vehículo: Organización cronológica, donde se almacenan registros de servicios anteriores, cotizaciones, fotos de reparaciones y evaluaciones recibidas.

🟩FAQ / Soporte: Organización temática por preguntas frecuentes y asistencia rápida en casos de cambios de cita, cancelaciones o consultas sobre el estado de servicio.

## Talleres Automotrices:

El módulo para talleres está orientado a la gestión operativa de servicios, seguimiento de citas y comunicación con clientes. Se aplica una organización matricial enfocada en optimizar los procesos internos y mejorar la atención al usuario.

🟩Agenda de Trabajo: Vista de calendario diario, organizada por horarios y tipo de servicio. Permite la visualización inmediata de las citas asignadas y los servicios en progreso.

🟩Gestión de Clientes: Organización jerárquica que lista a los propietarios de vehículos, permitiendo contacto rápido, visualización del historial de servicios y asignación de técnicos.

🟩Control de Progresos: Organización secuencial que facilita el seguimiento interno de cada servicio, desde el diagnóstico inicial hasta la entrega del vehículo.

🟩Perfil del Taller: Sección jerárquica que permite administrar la información pública del taller, servicios disponibles, precios estimados y calificaciones recibidas.

🟩Capacitación y Actualización: Acceso a módulos de formación y guías prácticas orientadas a mejorar la calidad del servicio ofrecido y fomentar buenas prácticas operativas.

### 4.2.2. Labeling Systems

Las etiquetas utilizadas en la plataforma Tallerazo priorizan la claridad, simplicidad y orientación a la acción. Se evita el uso de términos técnicos complejos, optando por palabras clave comprensibles y directas, que guíen al usuario de manera intuitiva a través de las funcionalidades principales.

### Landing Page:

| Etiqueta          | Descripción                                                                                              |
| ----------------- | -------------------------------------------------------------------------------------------------------- |
| Home              | PPresenta el mensaje principal de la plataforma y acceso a los servicios destacados.                     |
| Servicios         | Acceso directo a las funciones principales: gestión de citas, seguimiento en tiempo real y comunicación. |
| Nosotros          | Sección informativa sobre la misión, visión y valores de Tallerazo.                                      |
| Empezar           | Botón CTA para iniciar el proceso de registro o navegación en los servicios.                             |
| Agendar Cita      | Botón para acceder directamente a la agenda de citas disponibles en talleres.                            |
| Seguir Reparación | Botón que permite al usuario visualizar el estado actual de su servicio automotriz.                      |
| Contact Support   | Campo para ingresar correo y enviar consulta                                                             |
| Contactar Taller  | Enlace directo para iniciar comunicación con el taller asignado.                                         |

### Interfaces de Login / Registro:

| Etiqueta                         | Descripción                                                         |
| -------------------------------- | ------------------------------------------------------------------- |
| Email                            | Campo de ingreso para correo electrónico                            |
| Password                         | Campo de ingreso para contraseña                                    |
| Iniciar sesión                   | Botón para usuarios registrados que desean acceder a su cuenta.     |
| Crear cuenta                     | Botón para nuevos usuarios que desean registrarse en la plataforma. |
| ¿Ya tienes cuenta? Inicia sesión | Enlace alternativo para cambiar entre registro e inicio de sesión.  |

### 4.2.3. SEO Tags and Meta Tags:

🟩Title: Tallerazo – Conecta con talleres de confianza y gestiona tu vehículo en línea

🟩Meta Description: Plataforma innovadora para agendar citas, seguir reparaciones en tiempo real y comunicarte directamente con talleres automotrices. Vive una experiencia automotriz más transparente y digitalizada.

🟩Keywords: talleres mecánicos, servicio automotriz, agendar cita taller, seguimiento de reparaciones, Tallerazo Perú, plataforma de talleres

🟩Author: Tallerazo Team

### Servicios:

🟩Title: Servicios Tallerazo – Agenda, Sigue y Comunica tu reparación automotriz

🟩Meta Description: Descubre cómo agendar citas en talleres de confianza, seguir el avance de tu reparación en tiempo real y comunicarte directamente con tu mecánico a través de Tallerazo.

🟩Keywords: cita taller online, reparaciones en tiempo real, comunicación con talleres, servicios automotrices digitales, Tallerazo.

### Seguimiento de Reparaciones:

🟩Title: Seguimiento Tallerazo – Control total de la reparación de tu vehículo

🟩Meta Description: Revisa en tiempo real el estado de tu vehículo en proceso de reparación. Tallerazo te ofrece control y transparencia en cada etapa de tu servicio automotriz.

🟩Keywords: seguimiento de reparaciones, control de servicio automotriz, avance reparación taller, servicio transparente, Tallerazo

### 4.2.4. Searching Systems:

| Filtro           | Descripción                                                                                                                           |
| ---------------- | ------------------------------------------------------------------------------------------------------------------------------------- |
| Buscar en FAQ    | Permite ingresar palabras clave relacionadas a citas, reparaciones, seguimiento de vehículos o problemas frecuentes en la plataforma. |
| Filtrar por Plan | Permite ver únicamente los servicios según su estado actual (En diagnóstico, En reparación, Listo para entrega).                      |
| Buscar Servicio  | Navegación rápida para encontrar talleres disponibles según ubicación, tipo de servicio o reputación.                                 |

### 4.2.5. Navigation Systems:

El sistema de navegación de Tallerazo ha sido diseñado para facilitar el recorrido del usuario tanto en la landing page como dentro de la aplicación, garantizando una experiencia fluida, clara y enfocada en el cumplimiento de objetivos. La navegación se basa en principios de diseño centrado en el usuario, utilizando estructuras modernas que aseguran accesibilidad, claridad y bajo esfuerzo cognitivo.

## Landing Page

Estructura: Presentación general de MascotaMatch con llamada a la acción visible, acceso a servicios, planes, preguntas frecuentes y contacto.

- **Estructura:** Presentación general de Tallerazo con llamado a la acción visible, acceso a servicios, gestión de citas, seguimiento de reparaciones y contacto.
- **Incluye acceso rápido a:**
  - Registro / Inicio de sesión
  - Agendar cita
  - Seguir reparación
  - Servicios destacados
  - Contactar taller
- **Acción del Usuario:** Explorar contenido, agendar servicios, seguir el avance de su vehículo, contactar con talleres y resolver dudas operativas.

#### Aplicación Web – Clientes

- **Inicio:**
  - Muestra citas activas, próximos seguimientos y acceso directo a historial de servicios.
  - Organización matricial con bloques de acción rápida.
- **Agenda de citas:**
  - Visualización de citas programadas en formato calendario.
  - Botones rápidos para reprogramar o cancelar.
- **Seguimiento de Servicio:**
  - Vista secuencial del avance de la reparación.
  - Indicadores de progreso por fases (Diagnóstico, Reparación, Entrega).
- **Historial del Vehículo:**
  - Listado cronológico de servicios anteriores, incluyendo cotizaciones y documentos adjuntos.
- **Soporte:**
- Acceso directo a FAQs y contacto con soporte desde el menú principal.

#### Aplicación Web – Talleres

- **Inicio:**
  - Vista resumida de citas próximas, servicios activos y alertas de seguimiento.
- **Agenda de trabajo:**
  - Calendario organizado por hora y tipo de servicio.
- **Clientes asignados:**
  - Listado diario de propietarios con acceso a la ficha de servicio e historial del vehículo.
- **Perfil del taller:**
  - Sección para administrar información pública, servicios disponibles, precios y reputación recibida.
- **Capacitación / Recursos:**
  - Acceso a materiales de actualización profesional y mejores prácticas de atención automotriz.

## 4.3. Landing Page UI Design

### 4.3.1. Landing Page Wireframe

Esquema inicial de la página de aterrizaje.

![full landing page wireframe](./src/chapter-4/landing/wireframe_full-landing.png)

### 4.3.2. Landing Page Mock-up

Prototipo visual de la página de aterrizaje.

![full landing page design](./src/chapter-4/landing/design_full-landing.png)

## 4.4. Web Applications UX/UI Design

### 4.4.1. Web Applications Wireframes

Esquemas iniciales para aplicaciones web.

### VISTA DEL USUARIO

#### Dashboard principal

![dashboard principal](./src/chapter-4/web-app/wireframe/wireframe_dashboard-principal.png)

#### Detalles del taller

![detalles del taller](./src/chapter-4/web-app/wireframe/wireframe_detalles-del-taller.png)

#### Agendar cita en el taller

![agendar cita](./src/chapter-4/web-app/wireframe/wireframe_agendar-cita-con-el-taller.png)

### VISTA DEL TALLER

![Agendar cita management](./src/chapter-4/web-app/wireframe/wireframe_dashboard_admin.png)
![Agendar cita calendar](./src/chapter-4/web-app/wireframe/wireframe_dashboard_admin_agenda.png)

### 4.4.2. Web Applications Wireflow Diagrams

Diagramas de flujo de interacción para aplicaciones web.

#### TALLER

```
flowchart LR
    A[Login] --> B[Dashboard Admin]

    B --> C[Gestión de Citas]
    C --> C1[Listado de Citas]
    C1 --> C2[Detalles de Cita (Modal)]
    C2 --> C3[Crear Reparación (Modal)]
    C3 --> C1

    B --> D[Gestión de Reparaciones]
    D --> D1[Listado de Reparaciones]
    D1 --> D2[Actualizar Estado (Modal)]
    D2 --> D1

    B --> E[Gestión de Servicios]
    E --> E1[Listado de Servicios]
    E1 --> E2[Editar/Eliminar Servicio (Modal)]
    E2 --> E1
    E1 --> E3[Nuevo Servicio (Modal)]
    E3 --> E1

    B --> F[Configuración]
    F --> F1[Pestaña Perfil]
    F1 --> F1a[Editar Info del Taller]
    F1a --> F1b[Guardar Cambios]

    F --> F2[Pestaña Horario]
    F2 --> F2a[Editar Franjas Horarias]
    F2a --> F2b[Guardar Horario]

    F --> F3[Pestaña Notificaciones]
    F3 --> F3a[Activar/Desactivar Canales]
    F3a --> F3b[Activar/Desactivar Tipos]
    F3b --> F3c[Guardar Configuración]
```

#### USUARIO

```
flowchart LR
    U1[Login Usuario] --> U2[Dashboard Usuario]

    U2 --> U3[Buscar Taller]
    U3 --> U4[Filtrar por Región/Provincia/Distrito/Localidad]
    U4 --> U5[Listado de Talleres]
    U5 --> U6[Detalle Taller]
    U6 --> U7[Solicitar Cita (Formulario)]
    U7 --> U8[Confirmación de Cita]

    U2 --> U9[Mis Citas]
    U9 --> U9a[Listado de Citas]
    U9a --> U9b[Detalle Cita (Modal)]
    U9b --> U9c[Seguimiento Cita (Modal)]

    U2 --> U10[Mis Reparaciones]
    U10 --> U10a[Listado de Reparaciones]
    U10a --> U10b[Detalle Reparación (Modal)]
    U10b --> U10c[Seguimiento Reparación (Modal)]

    U2 --> U11[Historial de Mantenimientos]
    U11 --> U11a[Listado de Mantenimientos]
    U11a --> U11b[Detalle Mantenimiento (Modal)]
```

### 4.4.3. Web Applications Mock-ups

Prototipos visuales para aplicaciones web.

### VISTA DEL USUARIO

#### Dashboard principal

![Dashboard principal](./src/chapter-4/web-app/design/design_user_dashboard-principal.png)

#### Detalles de un taller

![Detalles del taller](./src/chapter-4/web-app/design/design_detalles_taller.png)

#### Agendar Cita

![Agendar cita](./src/chapter-4/web-app/design/design_agendar_cita.png)

#### Seguimiento de citas

![Seguimiento de citas](./src/chapter-4/web-app/design/design_seguimiento-de-citas.png)

#### Detalles de la cita

![Detalles de la cita](./src/chapter-4/web-app/design/design_detalles_cita.png)

#### Seguimiento de reparaciones users

![Seguimiento de reparaciones](./src/chapter-4/web-app/design/design_reparaciones.png)

#### Detalles de las repaciones

![Seguimiento de reparaciones](./src/chapter-4/web-app/design/design_detalles_reparaciones.png)

### VISTA DEL TALLER

#### Dashboard Principal

![Dashboard principal del taller](./src/chapter-4/web-app/design/design_admin_dashboard-principal.png)

#### Gestión de citas del taller

![Gestión de citas del taller](./src/chapter-4/web-app/design/design_admin_gestion-de-citas.png)

### Gestión de las reparaciones

![Gestión de las reparaciones](./src/chapter-4/web-app/design/design_admin_gestión-de-reparaciones.png)

### Configuración de los servicios

![Gestión de los servicios](./src/chapter-4/web-app/design/design_admin_gestion-de-servicios.png)

### Configuración del perfil de taller

![Configuración del perfil](./src/chapter-4/web-app/design/design_admin_configuracion-perfil.png)

### Configuración de los horarios

![Configuración de horarios](./src/chapter-4/web-app/design/design_admin_configuracion-horario.png)

### Configuración de Notificaciones

![Configuración de horarios](./src/chapter-4/web-app/design/design_admin_configuracion-notificaciones.png)

### 4.4.4. Web Applications User Flow Diagrams

#### USUARIO

```
flowchart TD
    A[Inicio de sesión] --> B[Dashboard Usuario]

    B --> C[Encontrar taller]
    C --> C1[Seleccionar región/provincia/distrito/localidad]
    C1 --> C2[Ver lista de talleres]
    C2 --> C3[Seleccionar taller]
    C3 --> C4[Ver detalles del taller]
    C4 --> C5[Solicitar cita]
    C5 --> C6[Completar formulario de cita]
    C6 --> C7[Confirmación de cita]

    B --> D[Mis citas y reparaciones]
    D --> D1[Ver Mis Citas]
    D1 --> D1a[Seleccionar cita]
    D1a --> D1b[Ver detalles de la cita]
    D1b --> D1c[Abrir seguimiento de cita]

    D --> D2[Ver Mis Reparaciones]
    D2 --> D2a[Seleccionar reparación]
    D2a --> D2b[Ver detalles de reparación]
    D2b --> D2c[Abrir seguimiento de reparación]

    B --> E[Historial de mantenimientos]
    E --> E1[Ver lista de mantenimientos]
    E1 --> E1a[Seleccionar registro]
    E1a --> E1b[Ver detalles de mantenimiento]
```

#### TALLER

```mermaid
flowchart TD
    A[Inicio de sesión] --> B[Panel de Administración]

    B --> C[Dashboard Principal]
    C --> C1[Ver próximas citas]
    C --> C2[Gestionar cita<br/>→ Crear reparación]

    B --> D[Gestión de Citas]
    D --> D1[Ver lista / Calendario]
    D1 --> D1a[Buscar / Filtrar]
    D1 --> D1b[Crear nueva cita]
    D1 --> D1c[Actualizar estado]

    B --> E[Gestión de Reparaciones]
    E --> E1[Ver Activas / Completadas / Canceladas]
    E1 --> E1a[Nueva reparación]
    E1 --> E1b[Actualizar estado]

    B --> F[Gestión de Servicios]
    F --> F1[Buscar / Filtrar por categoría]
    F1 --> F1a[Nuevo servicio]
    F1 --> F1b[Editar / Eliminar servicio]

    B --> G[Configuración]
    G --> G1[Perfil]
    G --> G2[Horario]
    G --> G3[Notificaciones]

    G1 --> G1a[Editar info del taller]
    G1 --> G1b[Cambiar logo]
    G1 --> G1c[Guardar cambios]

    G2 --> G2a[Activar/desactivar días]
    G2 --> G2b[Seleccionar franjas horarias]
    G2 --> G2c[Guardar horario]

    G3 --> G3a[Activar canales email/SMS]
    G3 --> G3b[Activar tipos de notificación]
    G3 --> G3c[Guardar configuración]
```

## 4.6. Domain-Driven Software Architecture

### 4.6.1. Software Architecture Context Diagram

Diagrama de contexto de la arquitectura de software.

![Context](./src/Context.png)

### 4.6.2. Software Architecture Container Diagrams

Diagramas de contenedores de la arquitectura de software.

![Container](./src/Container.png)

### 4.6.3. Software Architecture Components Diagrams

Diagramas de componentes de la arquitectura de software.

![Components](./src/Components.png)

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
