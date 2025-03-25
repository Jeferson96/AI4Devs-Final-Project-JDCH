# **📌 Épicas Iniciales para la Configuración del Proyecto**

1️⃣ **Épica: Configuración del Proyecto Frontend**

-   📍 Objetivo: Crear la estructura base del frontend, definir tecnologías y garantizar integración con el backend.
-   📌 Historias de usuario y tickets a definir:
    -   Inicialización del proyecto con **Next.js**.
    -   Configuración de **Eslint y Prettier** para estándares de código.
    -   Implementación de **TailwindCSS** para estilos.
    -   Conexión inicial con el backend mediante **API REST**.
    -   Definición de **estructura de carpetas y componentes**.
---
# Historias de usuario
---

#### **Historia de Usuario 1: Inicialización del Proyecto Frontend**

📌 **Épica:** Configuración del Proyecto Frontend

**Título:** Como desarrollador, quiero inicializar el proyecto frontend con Next.js asegurando que la estructura siga los principios de arquitectura definidos.

**Descripción:**  
Para garantizar un desarrollo estructurado y alineado con los principios arquitectónicos, se debe inicializar el frontend con **Next.js y TypeScript**, estableciendo una **estructura modular** que siga los principios de **Clean Architecture, Screaming Architecture y Vertical Slicing**.

**Criterios de Aceptación:**  
✅ Se crea el proyecto utilizando **Next.js con TypeScript**.  
✅ Se configura **Eslint y Prettier** para mantener estándares de código.  
✅ Se agrega **TailwindCSS** como framework de estilos.  
✅ Se define una **estructura de carpetas modular**, separando lógica de negocio, presentación e infraestructura.  
✅ Se implementa un **módulo base** para verificar la separación de responsabilidades.  
✅ Se documenta la configuración inicial y su alineación con **los principios arquitectónicos**.  
✅ Se verifica que la aplicación se ejecuta correctamente en **modo desarrollo** y **producción**.

**Prioridad:** Alta  

----------

### **Historia de Usuario 2: Configuración de Estilos Base con TailwindCSS**

📌 **Épica:** Configuración del Proyecto Frontend

**Título:** Como desarrollador, quiero configurar los estilos base en el frontend utilizando TailwindCSS para garantizar coherencia visual y mantenibilidad.

**Descripción:**  
Se debe integrar **TailwindCSS** y definir un **sistema de estilos modular**, asegurando que la estructura de estilos siga los principios de **Clean Architecture y Vertical Slicing**.

**Criterios de Aceptación:**  
✅ Se integra **TailwindCSS** en el proyecto frontend.  
✅ Se configura un **sistema de diseño** con variables globales (colores, tipografía, espaciados).  
✅ Se documenta la estructura de estilos y su aplicación en la arquitectura del proyecto.  
✅ Se validan los estilos en componentes iniciales para asegurar su correcta implementación.  
✅ Se asegura la compatibilidad con futuras personalizaciones de temas.

**Prioridad:** Alta  
**Dependencias:** Inicialización del proyecto frontend.

----------

### **Historia de Usuario 3: Implementación de shadcn/ui y Soporte para Modo Oscuro**

📌 **Épica:** Configuración del Proyecto Frontend

**Título:** Como desarrollador, quiero implementar **shadcn/ui** y la funcionalidad de cambio de tema (modo oscuro/claro) para mejorar la experiencia visual del usuario.

**Descripción:**  
Se debe integrar **shadcn/ui** como la librería de componentes UI y establecer una **gestión de temas**, permitiendo el cambio entre **modo claro y oscuro** desde el inicio.

**Criterios de Aceptación:**  
✅ Se instala e integra **shadcn/ui** en el proyecto frontend.  
✅ Se configura el cambio de tema entre **modo claro y oscuro** utilizando **Next.js Theme Provider**.  
✅ Se implementa un **componente de selección de tema** en la interfaz.  
✅ Se asegura la persistencia del tema seleccionado en el almacenamiento local del navegador.  
✅ Se documenta la integración de **shadcn/ui** y su compatibilidad con TailwindCSS.

**Prioridad:** Alta  
**Dependencias:** Configuración de Estilos Base con TailwindCSS.

----------
### **Historia de Usuario 4: Definición de la Estructura de Carpetas y Organización del Código**

📌 **Épica:** Configuración del Proyecto Frontend

**Título:** Como desarrollador, quiero definir la estructura de carpetas y la organización del código en el frontend para asegurar modularidad y escalabilidad.

**Descripción:**  
Se debe establecer una estructura de carpetas siguiendo **Screaming Architecture, Clean Architecture y Vertical Slicing**, asegurando una separación clara entre presentación, lógica de negocio e infraestructura.

**Criterios de Aceptación:**  
✅ Se define una estructura modular que refleje la funcionalidad principal del sistema.  
✅ Se separan las capas de **componentes, páginas, servicios, hooks y utilidades**.  
✅ Se implementa una carpeta dedicada para **contextos globales y estados compartidos**.  
✅ Se documenta la estructura y sus principios en un archivo de referencia dentro del repositorio.  
✅ Se verifica que la organización permite escalar y mantener el proyecto de manera eficiente.

**Prioridad:** Alta  
**Dependencias:** Inicialización del proyecto frontend.

----------
### **Historia de Usuario 5: Configuración de Rutas y Navegación en el Frontend**

📌 **Épica:** Configuración del Proyecto Frontend

**Título:** Como desarrollador, quiero configurar el sistema de rutas y navegación en el frontend para garantizar una estructura clara y mantenible.

**Descripción:**  
Se debe establecer un sistema de enrutamiento utilizando el enrutador de **Next.js**, asegurando que las rutas sigan una estructura organizada y escalable. También se debe definir una estrategia de **layouts** para reutilización de componentes globales.

**Criterios de Aceptación:**  
✅ Se configura el sistema de enrutamiento utilizando el enrutador de **Next.js**.  
✅ Se definen rutas base para páginas principales (Ejemplo: `/`, `/login`, `/dashboard`).  
✅ Se implementa un sistema de **layouts globales** para la reutilización de encabezados, pies de página y menús de navegación.  
✅ Se crea un archivo de **mapeo de rutas** para mantener consistencia y facilitar modificaciones.  
✅ Se documenta la configuración de rutas y navegación dentro del repositorio.

**Prioridad:** Alta  
**Dependencias:** Definición de la estructura de carpetas y organización del código.

----------
### **Historia de Usuario 6: Configuración de Comunicación con el Backend**

📌 **Épica:** Configuración del Proyecto Frontend

**Título:** Como desarrollador, quiero configurar la comunicación con el backend para asegurar una integración eficiente y escalable.

**Descripción:**  
Se debe establecer un sistema modular para la comunicación con el backend, asegurando una correcta gestión de solicitudes **API REST** mediante **fetch o axios**, y organizando los servicios según **Clean Architecture y Vertical Slicing**.

**Criterios de Aceptación:**  
✅ Se define un módulo centralizado para realizar peticiones al backend.  
✅ Se implementa una **configuración global** para manejar URLs base y encabezados.  
✅ Se asegura el manejo adecuado de **errores y estados de carga** en las peticiones.  
✅ Se documenta la estructura de comunicación en el repositorio.  
✅ Se prepara la configuración para soportar autenticación en futuras implementaciones.

**Prioridad:** Alta  
**Dependencias:** Definición de la estructura de carpetas y organización del código.

----------
### **Historia de Usuario 7: Configuración de Manejo de Estado Global**

📌 **Épica:** Configuración del Proyecto Frontend

**Título:** Como desarrollador, quiero configurar el manejo de estado global en el frontend para facilitar la gestión de datos compartidos entre componentes.

**Descripción:**  
Se debe establecer un sistema eficiente de manejo de estado utilizando **React Context API o Zustand**, asegurando una estructura modular y alineada con **Clean Architecture y Vertical Slicing**.

**Criterios de Aceptación:**  
✅ Se define un sistema de estado global para datos compartidos como usuario autenticado y configuración del tema.  
✅ Se separan los estados en **módulos organizados** para facilitar la escalabilidad.  
✅ Se implementan **proveedores de contexto** o **stores de Zustand** para gestionar el estado de manera eficiente.  
✅ Se documenta la estrategia de manejo de estado y su implementación en el repositorio.  
✅ Se realizan pruebas en componentes clave para verificar la correcta propagación del estado.

**Prioridad:** Alta  
**Dependencias:** Configuración de la comunicación con el backend.

----------

### **Historia de Usuario 8: Configuración del Sistema de Autenticación en el Frontend**

📌 **Épica:** Configuración del Proyecto Frontend

**Título:** Como desarrollador, quiero configurar el sistema de autenticación en el frontend para permitir el acceso seguro de los usuarios.

**Descripción:**  
Se debe implementar un mecanismo de autenticación basado en **tokens JWT**, asegurando la integración con el backend y gestionando sesiones de manera segura. Se debe utilizar un almacenamiento seguro para los tokens y garantizar que los usuarios autenticados puedan acceder a las rutas protegidas.

**Criterios de Aceptación:**  
✅ Se establece un flujo de autenticación utilizando **API REST con JWT**.  
✅ Se configuran **rutas protegidas** para usuarios autenticados.  
✅ Se implementa un mecanismo de **almacenamiento seguro** del token (ejemplo: HttpOnly cookies o localStorage con medidas de seguridad).  
✅ Se documenta la estrategia de autenticación y autorización.  
✅ Se realizan pruebas para validar el flujo de login y persistencia de sesión.

**Prioridad:** Alta  
**Dependencias:** Configuración de la comunicación con el backend.

----------

### **📌 Validación de Alcance y Alineación con el MVP**

✅ **Es esencial para el MVP**, ya que permitirá gestionar sesiones de usuario en el sistema.  
✅ **No introduce complejidad innecesaria**, ya que se limita a la autenticación básica con JWT sin integración con OAuth u otros métodos avanzados.  
✅ **Está alineada con el MVP**, asegurando que solo los usuarios autorizados puedan acceder a las funcionalidades del sistema.

----------

### **Historia de Usuario 9: Configuración del Manejo de Errores y Validaciones en el Frontend**

📌 **Épica:** Configuración del Proyecto Frontend

**Título:** Como desarrollador, quiero configurar un sistema de manejo de errores y validaciones en el frontend para mejorar la experiencia del usuario y la estabilidad del sistema.

**Descripción:**  
Se debe implementar un mecanismo estandarizado para manejar errores en la comunicación con el backend y validaciones de formularios. Esto garantizará que los mensajes de error sean claros y que los usuarios reciban retroalimentación inmediata en caso de entradas inválidas o fallos en el sistema.

**Criterios de Aceptación:**  
✅ Se implementa un **gestor global de errores** para capturar y manejar respuestas del backend.  
✅ Se configuran **mensajes de error personalizados** para solicitudes fallidas.  
✅ Se implementan validaciones en formularios utilizando **Zod o React Hook Form**.  
✅ Se asegura que los errores se muestren de manera clara en la interfaz de usuario.  
✅ Se documenta la estrategia de manejo de errores y validaciones en el repositorio.

**Prioridad:** Alta  
**Dependencias:** Configuración de la comunicación con el backend, Configuración del sistema de autenticación.

----------
### **Historia de Usuario 10: Configuración de la Documentación Técnica del Frontend**

📌 **Épica:** Configuración del Proyecto Frontend

**Título:** Como desarrollador, quiero establecer una documentación técnica clara del frontend para facilitar el mantenimiento y la escalabilidad del proyecto.

**Descripción:**  
Se debe crear y estructurar la documentación técnica del frontend, asegurando que el equipo de desarrollo pueda comprender la arquitectura del sistema, las convenciones de código y las integraciones clave.

**Criterios de Aceptación:**  
✅ Se documenta la **estructura del proyecto**, incluyendo la organización de carpetas y módulos.  
✅ Se definen convenciones de código y buenas prácticas para el desarrollo.  
✅ Se detallan las **integraciones clave**, como API REST y autenticación.  
✅ Se crea una guía de instalación y configuración para nuevos desarrolladores.  
✅ Se almacena la documentación en el repositorio (ejemplo: `README.md` o Wiki interna).

**Prioridad:** Media  
**Dependencias:** Configuración del manejo de errores y validaciones en el frontend.

----------

2️⃣ **Épica: Configuración del Proyecto Backend**

-   📍 Objetivo: Crear la base del backend, establecer la arquitectura y definir endpoints esenciales.
-   📌 Historias de usuario y tickets a definir:
    -   Inicialización del backend con **NestJS**.
    -   Configuración de **Prisma ORM** para conexión con PostgreSQL.
    -   Definición de **estructura de carpetas** siguiendo Clean Architecture.
    -   Creación de **endpoints base** para autenticación y manejo de datos iniciales.
    -   Implementación de **Swagger** para documentación de la API.

---
## Historias de usuario
---
### **Historia de Usuario 1: Inicialización del Proyecto Backend**

📌 **Épica:** Configuración del Proyecto Backend

**Título:** Como desarrollador, quiero inicializar el proyecto backend con NestJS para establecer la base del sistema.

**Descripción:**  
Se debe inicializar el backend con **NestJS**, asegurando que la estructura del proyecto siga los principios de **Clean Architecture, Hexagonal Architecture y DDD**, permitiendo una organización modular y escalable.

**Criterios de Aceptación:**  
✅ Se inicializa el proyecto backend con **NestJS y TypeScript**.  
✅ Se configura **Eslint y Prettier** para mantener estándares de código.  
✅ Se define una estructura modular alineada con **DDD y Clean Architecture**.  
✅ Se crea una **configuración base de dependencias** (ejemplo: configuración de env variables, scripts de ejecución).  
✅ Se documenta la configuración inicial en el repositorio.

**Prioridad:** Alta  
**Dependencias:** Ninguna (es el primer paso del backend).

----------


### **Historia de Usuario 2: Configuración de la Base de Datos con Supabase**

📌 **Épica:** Configuración del Proyecto Backend

**Título:** Como desarrollador, quiero configurar la base de datos con Supabase PostgreSQL para garantizar una gestión escalable y segura de los datos.

**Descripción:**  
Se debe establecer la conexión con **Supabase PostgreSQL**, asegurando compatibilidad con el ORM y alineación con **Clean Architecture y DDD**. También se debe configurar la seguridad de acceso a la base de datos utilizando **Row Level Security (RLS)**.

**Criterios de Aceptación:**  
✅ Se configura **Supabase PostgreSQL** como base de datos del backend.  
✅ Se establece la conexión con **Prisma ORM**, asegurando compatibilidad con Supabase.  
✅ Se implementa **Row Level Security (RLS)** para controlar acceso a los datos según roles.  
✅ Se configuran **variables de entorno seguras** para conexión con la base de datos.  
✅ Se documenta la configuración de la base de datos y su integración con Prisma en el repositorio.

**Prioridad:** Alta  
**Dependencias:** Inicialización del proyecto backend.

----------
### **Historia de Usuario 3: Definición de la Estructura de Carpetas y Organización del Código en el Backend**

📌 **Épica:** Configuración del Proyecto Backend

**Título:** Como desarrollador, quiero definir la estructura de carpetas y la organización del código en el backend para asegurar modularidad y escalabilidad.

**Descripción:**  
Se debe establecer una estructura de carpetas alineada con **Clean Architecture, Hexagonal Architecture y DDD**, asegurando una separación clara entre las capas de dominio, aplicación, infraestructura y presentación.

**Criterios de Aceptación:**  
✅ Se define una estructura modular que refleje la funcionalidad principal del sistema (**Screaming Architecture**).  
✅ Se separan las capas de **dominio, aplicación, infraestructura y presentación**.  
✅ Se implementa una carpeta dedicada para **entidades, repositorios, servicios y controladores**.  
✅ Se documenta la estructura de carpetas y su alineación con los principios arquitectónicos en el repositorio.  
✅ Se verifica que la organización permite escalar y mantener el proyecto de manera eficiente.

**Prioridad:** Alta  
**Dependencias:** Inicialización del proyecto backend, Configuración de la base de datos y ORM.

----------

### **Historia de Usuario 4: Configuración de Controladores, Servicios y Repositorios Base**

📌 **Épica:** Configuración del Proyecto Backend

**Título:** Como desarrollador, quiero configurar la capa de controladores, servicios y repositorios en el backend para garantizar una estructura modular y escalable.

**Descripción:**  
Se debe establecer la arquitectura base de **Controladores (Controllers), Servicios (Services) y Repositorios (Repositories)** siguiendo los principios de **DDD, Clean Architecture y Hexagonal Architecture**. Esto asegurará una correcta separación de responsabilidades y facilitará la escalabilidad del sistema.

**Criterios de Aceptación:**  
✅ Se implementa un **controlador base** que gestione peticiones HTTP.  
✅ Se configura una capa de **servicios** que maneje la lógica de negocio.  
✅ Se implementa una capa de **repositorios** que gestione la interacción con la base de datos mediante Prisma.  
✅ Se establece la inyección de dependencias para desacoplar módulos y facilitar pruebas unitarias.  
✅ Se documenta la arquitectura y cómo deben crearse nuevos módulos siguiendo esta estructura.

**Prioridad:** Alta  
**Dependencias:** Definición de la estructura de carpetas y organización del código en el backend.

----------

### **Historia de Usuario 5: Configuración del Sistema de Autenticación con Supabase**

📌 **Épica:** Configuración del Proyecto Backend

**Título:** Como desarrollador, quiero configurar el sistema de autenticación utilizando Supabase Auth para gestionar el acceso seguro de los usuarios.

**Descripción:**  
Se debe implementar **Supabase Auth** como el sistema de autenticación del backend, asegurando que el manejo de sesiones y validación de usuarios cumpla con **los principios de seguridad y regulación de datos**. Se debe establecer una estrategia de gestión de **roles y permisos** basada en **Row Level Security (RLS)**.

**Criterios de Aceptación:**  
✅ Se configura **Supabase Auth** como el proveedor de autenticación del backend.  
✅ Se establecen **roles y permisos** diferenciados para pacientes y profesionales.  
✅ Se implementa la validación de **tokens JWT** emitidos por Supabase.  
✅ Se configuran **rutas protegidas** en el backend que solo acepten tokens válidos.  
✅ Se documenta el flujo de autenticación y cómo interactúa con el frontend.

**Prioridad:** Alta  
**Dependencias:** Configuración de la base de datos con Supabase.

----------

### **Historia de Usuario 6: Configuración de la Gestión de Roles y Permisos con Supabase**

📌 **Épica:** Configuración del Proyecto Backend

**Título:** Como desarrollador, quiero configurar la gestión de roles y permisos en Supabase para controlar el acceso a los datos según el tipo de usuario.

**Descripción:**  
Se debe implementar un esquema de **roles y permisos** en Supabase utilizando **Row Level Security (RLS)** para diferenciar entre **pacientes y profesionales**. Además, se debe definir una estrategia para que el backend pueda validar y aplicar estos permisos correctamente en las consultas a la base de datos.

**Criterios de Aceptación:**  
✅ Se configuran los roles de **paciente y profesional** en Supabase.  
✅ Se implementan **políticas de acceso** con **Row Level Security (RLS)** para garantizar que cada usuario solo pueda acceder a sus propios datos.  
✅ Se asegura que el backend valide los permisos de los usuarios antes de ejecutar operaciones en la base de datos.  
✅ Se documenta la estrategia de roles y cómo se aplican en Supabase.

**Prioridad:** Alta  
**Dependencias:** Configuración del sistema de autenticación con Supabase.

----------
### **Historia de Usuario 7: Configuración de la Comunicación entre el Backend y Supabase**

📌 **Épica:** Configuración del Proyecto Backend

**Título:** Como desarrollador, quiero configurar la comunicación entre el backend y Supabase para garantizar la correcta interacción con la base de datos y autenticación.

**Descripción:**  
Se debe establecer una integración eficiente entre el backend y Supabase para manejar peticiones a la base de datos y validar autenticaciones. Es fundamental garantizar que todas las consultas y operaciones cumplan con los **principios de seguridad y escalabilidad** definidos.

**Criterios de Aceptación:**  
✅ Se implementa una **capa de abstracción** para manejar la comunicación con Supabase.  
✅ Se configuran métodos en el backend para interactuar con **Supabase Auth y la base de datos**.  
✅ Se establece una estrategia de **validación de tokens JWT** en cada solicitud al backend.  
✅ Se documenta la configuración y el flujo de comunicación con Supabase.

**Prioridad:** Alta  
**Dependencias:** Configuración de la base de datos y autenticación con Supabase.

----------

### **Historia de Usuario 8: Configuración de Seguridad y Protección de Datos en el Backend**

📌 **Épica:** Configuración del Proyecto Backend

**Título:** Como desarrollador, quiero configurar medidas de seguridad en el backend para garantizar la protección de datos sensibles y el cumplimiento normativo.

**Descripción:**  
Se deben implementar medidas de seguridad en el backend para proteger la información de los usuarios, asegurando el cumplimiento de normativas como la **Ley 1581 de 2012 (Protección de Datos en Colombia)** y **GDPR** en caso de usuarios internacionales.

**Criterios de Aceptación:**  
✅ Se implementa **cifrado en reposo** para datos sensibles almacenados en Supabase.  
✅ Se configura **TLS/HTTPS** para el cifrado en tránsito en todas las comunicaciones.  
✅ Se aseguran **prácticas de almacenamiento seguro de tokens JWT**, evitando exposición de credenciales.  
✅ Se establecen políticas de **retención y eliminación de datos**, alineadas con regulaciones de privacidad.  
✅ Se documentan las medidas de seguridad implementadas en el repositorio.

**Prioridad:** Alta  
**Dependencias:** Configuración de la comunicación entre el backend y Supabase.

----------

### **Historia de Usuario 9: Configuración del Sistema de Logs y Monitoreo en el Backend**

📌 **Épica:** Configuración del Proyecto Backend

**Título:** Como desarrollador, quiero configurar un sistema de logs y monitoreo en el backend para detectar errores y mejorar la estabilidad del sistema.

**Descripción:**  
Se debe establecer un mecanismo de **registro de eventos y monitoreo de actividad** en el backend para garantizar una gestión efectiva de errores y la supervisión del rendimiento del sistema.

**Criterios de Aceptación:**  
✅ Se implementa un **sistema de logs estructurados** para registrar eventos importantes (errores, autenticaciones, accesos a la base de datos).  
✅ Se configura un **servicio de monitoreo** para capturar métricas de rendimiento y disponibilidad.  
✅ Se asegura que los registros sean almacenados de manera segura y accesibles para auditoría.  
✅ Se documenta la configuración del sistema de logs y monitoreo en el repositorio.

**Prioridad:** Media  
**Dependencias:** Configuración de seguridad y protección de datos en el backend.

----------

### **Historia de Usuario 10: Configuración de la Documentación Técnica del Backend**

📌 **Épica:** Configuración del Proyecto Backend

**Título:** Como desarrollador, quiero establecer una documentación técnica clara del backend para facilitar su mantenimiento y escalabilidad.

**Descripción:**  
Se debe documentar la configuración del backend, incluyendo su arquitectura, integración con Supabase y estrategias de seguridad. Esto garantizará que el equipo de desarrollo pueda comprender el diseño del sistema y realizar futuras mejoras sin afectar la estabilidad.

**Criterios de Aceptación:**  
✅ Se documenta la **arquitectura del backend**, incluyendo la separación de capas y patrones utilizados.  
✅ Se detallan las **integraciones con Supabase**, tanto en autenticación como en base de datos.  
✅ Se documentan las **convenciones de código y buenas prácticas** utilizadas en el backend.  
✅ Se crea una guía de instalación y despliegue para nuevos desarrolladores.  
✅ Se almacena la documentación en el repositorio (`README.md`, Wiki interna o Notion).

**Prioridad:** Media  
**Dependencias:** Configuración del sistema de logs y monitoreo en el backend.

----------

---

3️⃣ **Épicas para Funcionalidades Principales** (Pendiente de desarrollo tras configuración inicial)

-   📍 Objetivo: Agrupar historias de usuario relacionadas con cada módulo funcional del sistema.
-   📌 Ejemplos de épicas futuras:
    -   **Gestión de Citas** (Agendamiento, cancelación y modificaciones).
    -   **Gestión de Disponibilidad** (Bloqueo de agenda y horarios).
    -   **Sistema de Notificaciones** (Envío de correos automáticos).
    -   **Monitoreo y Seguridad** (Auditoría de cambios y logs).

---

# Historias de usuario 


### **Historia de Usuario 1: Agendamiento de Citas**

**Título:** Como paciente, quiero agendar una cita con un profesional disponible para recibir atención en un horario conveniente.

**Descripción:**  
Los pacientes deben poder seleccionar un profesional, ver su disponibilidad y programar una cita dentro del horario permitido. Una vez confirmada, la cita debe registrarse en el sistema y enviarse una notificación de confirmación por correo electrónico.

**Criterios de Aceptación:**  
✅ El paciente puede ver una lista de profesionales disponibles.  
✅ El paciente puede seleccionar un profesional y ver sus horarios disponibles.  
✅ El paciente puede elegir una fecha y hora dentro de la disponibilidad del profesional.  
✅ La cita se registra en la base de datos con el estado "Agendada".  
✅ Se envía una notificación de confirmación por correo electrónico al paciente y al profesional.  
✅ Si no hay disponibilidad en la fecha seleccionada, el paciente recibe un mensaje indicándolo.

**Prioridad:** Alta  
**Dependencias:** Gestión de disponibilidad de los profesionales, Sistema de notificaciones.

----------

### **Historia de Usuario 2: Modificación y Cancelación de Citas**

**Título:** Como paciente, quiero modificar o cancelar una cita con al menos 24 horas de anticipación para ajustar mi disponibilidad.

**Descripción:**  
Los pacientes deben tener la posibilidad de modificar o cancelar sus citas siempre que lo hagan con **al menos 24 horas de antelación**, según la configuración del sistema. Cualquier cambio debe reflejarse en la base de datos y generar una notificación automática para el paciente y el profesional.

**Criterios de Aceptación:**  
✅ El paciente puede acceder a su historial de citas.  
✅ El paciente puede seleccionar una cita y optar por modificarla o cancelarla.  
✅ El sistema valida que la acción se realiza con al menos **24 horas de anticipación**.  
✅ Si la acción no está permitida (menos de 24 horas antes), el sistema muestra un mensaje indicando la restricción.  
✅ Si la modificación/cancelación es válida, se actualiza el estado de la cita en la base de datos.  
✅ Se envía una **notificación por correo** al paciente y al profesional sobre el cambio.

**Prioridad:** Alta  
**Dependencias:** Gestión de citas, Sistema de notificaciones.

----------

### **Historia de Usuario 3: Gestión de Disponibilidad por Parte del Profesional**

**Título:** Como profesional, quiero gestionar manualmente mi disponibilidad para definir los horarios en los que puedo atender citas.

**Descripción:**  
Los profesionales deben poder establecer su disponibilidad dentro del horario permitido (**7:00 a.m. - 5:00 p.m., parametrizable**). Deben poder bloquear horarios específicos o días completos cuando no estén disponibles.

**Criterios de Aceptación:**  
✅ El profesional puede acceder a su panel de disponibilidad.  
✅ El profesional puede definir sus horarios disponibles dentro del rango permitido.  
✅ El profesional puede bloquear horarios específicos o días completos.  
✅ Los cambios en la disponibilidad se reflejan en el sistema en tiempo real.  
✅ Si un horario bloqueado ya tiene citas agendadas, el sistema muestra una advertencia y evita el bloqueo hasta que las citas sean reprogramadas o canceladas.  
✅ Los pacientes solo pueden ver y seleccionar horarios disponibles según la configuración del profesional.

**Prioridad:** Alta  
**Dependencias:** Agendamiento de citas, Base de datos de disponibilidad.

----------

### **Historia de Usuario 4: Notificaciones Automáticas de Citas**  

**Título:** Como paciente y profesional, quiero recibir notificaciones automáticas sobre mis citas para estar informado oportunamente.  

**Descripción:**  
El sistema debe enviar notificaciones por correo electrónico en diferentes momentos clave del ciclo de una cita. Las notificaciones deben generarse **de manera asíncrona** mediante un **sistema basado en eventos internos y una cola de procesamiento**, evitando bloqueos en la API.  

**Criterios de Aceptación:**  
✅ El sistema emite un **evento interno** cuando se agenda, modifica o cancela una cita.  
✅ Un **listener de eventos** recibe la información y procesa el envío de la notificación.  
✅ Se integran **recordatorios automáticos** en los siguientes momentos:  
   - **Confirmación inmediata** tras agendar una cita.  
   - **Recordatorio 24 horas antes** de la cita.  
   - **Recordatorio 1 hora antes** de la cita.  
   - **Notificación en caso de modificación o cancelación de la cita.**  
✅ La cola de procesamiento de notificaciones **gestiona los envíos de manera eficiente** y permite reintentos en caso de fallos.  
✅ Existe una documentación clara en el repositorio sobre el sistema de notificaciones y su integración con eventos internos.  

**Prioridad:** Alta  
**Dependencias:** Implementación del Agendamiento de Citas.  


----------

### **Historia de Usuario 5: Restricciones de Cancelación y Modificación de Citas**

**Título:** Como paciente, quiero que el sistema me impida cancelar o modificar una cita con menos de 24 horas de anticipación para respetar la disponibilidad del profesional.

**Descripción:**  
El sistema debe validar que las cancelaciones y modificaciones solo puedan realizarse con **al menos 24 horas de anticipación**. Si un paciente intenta modificar o cancelar una cita fuera de este plazo, el sistema debe bloquear la acción y mostrar un mensaje explicativo.

**Criterios de Aceptación:**  
✅ El sistema valida la fecha y hora de la cita antes de permitir su cancelación o modificación.  
✅ Si faltan menos de **24 horas**, la acción es bloqueada y se muestra un mensaje al usuario.  
✅ Si la cancelación/modificación es válida, se actualiza la base de datos y se envían notificaciones a las partes involucradas.  
✅ Los profesionales deben poder ver el historial de cancelaciones/modificaciones de sus citas.  
✅ Se debe considerar la posibilidad de **parametrizar** este límite en el futuro.

**Prioridad:** Alta  
**Dependencias:** Agendamiento de citas, Gestión de disponibilidad, Sistema de notificaciones.

----------

### **Historia de Usuario 6: Mensajes de Disponibilidad en Tiempo Real**  

**Título:** Como paciente, quiero que el sistema me informe en tiempo real si un profesional no tiene disponibilidad para evitar intentos fallidos de agendamiento.  

**Descripción:**  
Cuando un paciente intenta agendar una cita, el sistema debe validar la disponibilidad del profesional en tiempo real. Para ello, se utilizará **suscripción a eventos en Supabase o WebSockets**, en lugar de consultas recurrentes a la base de datos, asegurando que la información reflejada en la interfaz sea siempre actualizada.  

**Criterios de Aceptación:**  
✅ La disponibilidad de los profesionales se **actualiza en tiempo real** en la interfaz del paciente.  
✅ Si un horario ya no está disponible al momento de seleccionarlo, se muestra un **mensaje claro en la interfaz**.  
✅ El sistema utiliza **suscripción a cambios en Supabase** o **WebSockets** en lugar de consultas directas a la base de datos.  
✅ Se documenta la estrategia de actualización en tiempo real en el repositorio.  

**Prioridad:** Media  
**Dependencias:** Gestión de disponibilidad, Agendamiento de citas.  

----------

### **Historia de Usuario 7: Bloqueo de Agenda por Parte del Profesional**  

**Título:** Como profesional, quiero poder bloquear mi agenda por horas o días completos para gestionar mi disponibilidad sin afectar citas ya agendadas.  

**Descripción:**  
El sistema debe permitir que los profesionales bloqueen horarios específicos o días completos cuando no puedan atender citas. Si un profesional intenta bloquear un horario en el que ya existen citas agendadas, el sistema debe **ofrecer la opción de reprogramación automática** antes de aplicar el bloqueo, garantizando que los pacientes sean informados y puedan seleccionar un nuevo horario.  

**Criterios de Aceptación:**  
✅ El profesional puede seleccionar un rango de horas o un día completo para bloquear su disponibilidad.  
✅ El sistema **valida que no existan citas programadas** en los horarios bloqueados.  
✅ Si hay citas agendadas en el horario a bloquear, el sistema:  
   - **Muestra una advertencia al profesional.**  
   - **Ofrece la opción de reprogramar automáticamente las citas afectadas.**  
   - **Notifica a los pacientes sobre la reprogramación.**  
✅ Los pacientes no pueden agendar citas en horarios bloqueados.  
✅ Los cambios en la disponibilidad se reflejan en **tiempo real** en el sistema.  
✅ Existe documentación clara en el repositorio sobre la funcionalidad de bloqueo de agenda y reprogramación de citas.  

**Prioridad:** Alta  
**Dependencias:** Gestión de disponibilidad, Agendamiento de citas.  


----------

### **Historia de Usuario 8: Registro y Auditoría de Cambios en las Citas**  

**Título:** Como administrador del sistema, quiero que se registre un historial inmutable de cambios en las citas para garantizar trazabilidad y control.  

**Descripción:**  
Cada vez que una cita sea creada, modificada o cancelada, el sistema debe registrar un **historial inmutable de cambios** con la información relevante, asegurando que los datos sean accesibles para auditoría y análisis. Además, los registros deben contener **metadata adicional**, incluyendo IP del usuario y tipo de dispositivo utilizado en la acción.  

**Criterios de Aceptación:**  
✅ El sistema registra automáticamente cualquier cambio en una cita (**creación, modificación, cancelación**).  
✅ Los registros incluyen **fecha y hora del evento, usuario que realizó la acción, IP y dispositivo utilizado**.  
✅ Los administradores y profesionales pueden **consultar el historial de cambios**, pero **no pueden modificar ni eliminar registros**.  
✅ Se garantiza la **inmutabilidad de los registros**, evitando alteraciones indebidas.  
✅ Existe documentación clara en el repositorio sobre la implementación del registro de auditoría.  

**Prioridad:** Media  
**Dependencias:** Agendamiento de citas, Seguridad de datos, Base de datos de auditoría.  

----------

### **Historia de Usuario 9: Configuración Parametrizable de Reglas del Sistema**  

**Título:** Como administrador, quiero poder configurar parámetros clave del sistema sin afectar citas ya programadas.  

**Descripción:**  
El sistema debe permitir que ciertos parámetros, como el **límite de tiempo para cancelaciones/modificaciones y el horario de atención de los profesionales**, sean configurables a través de una interfaz de administración o un archivo de configuración. Los cambios en la configuración **solo deben afectar nuevas citas**, garantizando que las reservas existentes mantengan las condiciones con las que fueron creadas.  

**Criterios de Aceptación:**  
✅ El administrador puede modificar las **reglas del sistema** desde una interfaz o archivo de configuración.  
✅ Los cambios en las reglas del sistema **no afectan citas ya programadas**, sino únicamente nuevas reservas.  
✅ Se implementa una **validación en el backend** para asegurar que las citas existentes mantengan su configuración original.  
✅ Se registra cualquier cambio en la configuración en un **historial de auditoría**.  
✅ Existe documentación clara en el repositorio sobre la parametrización de reglas del sistema.  

**Prioridad:** Alta  
**Dependencias:** Gestión de citas, Auditoría de cambios, Panel de administración.  

----------

### **Historia de Usuario 10: Monitoreo y Alertas del Sistema**

**Título:** Como administrador, quiero recibir alertas y monitorear el estado del sistema para detectar problemas de disponibilidad o rendimiento.

**Descripción:**  
El sistema debe contar con un mecanismo de monitoreo que permita detectar posibles problemas de disponibilidad, rendimiento o errores en el agendamiento de citas. Si se detecta una anomalía, se debe enviar una alerta al administrador.

**Criterios de Aceptación:**  
✅ El sistema registra métricas clave como tiempo de respuesta de la API, tasa de error y carga del servidor.  
✅ Se generan **alertas automáticas** si el sistema presenta tiempos de respuesta altos, fallas recurrentes o indisponibilidad.  
✅ El administrador recibe una notificación por correo en caso de fallos críticos.  
✅ Se almacena un registro de las alertas generadas para análisis posterior.  
✅ Se permite la consulta de métricas en tiempo real desde un panel de monitoreo.

**Prioridad:** Media  
**Dependencias:** Infraestructura del sistema, Registro de errores, Sistema de notificaciones.

----------

