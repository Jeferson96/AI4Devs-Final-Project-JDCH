## **📌 Tickets Frontend**

#### **🎯 Ticket 1: Inicialización del Proyecto Frontend**

📌 **Épica:** Configuración del Proyecto Frontend

**Título:** Inicializar el proyecto frontend con Next.js y TypeScript

**Descripción:**  
Se debe crear la base del proyecto frontend utilizando **Next.js con TypeScript**, asegurando una estructura modular y alineada con los principios de **Clean Architecture, Screaming Architecture y Vertical Slicing**.

**Tareas:**

-   Crear el proyecto con **Next.js y TypeScript** mediante `npx create-next-app@latest`.
-   Configurar **Eslint y Prettier** para asegurar estándares de código.
-   Definir una **estructura inicial de carpetas** basada en los principios arquitectónicos.
-   Verificar que el entorno de desarrollo y producción funcionan correctamente.
-   Agregar documentación en el repositorio (`README.md`) con instrucciones de instalación y ejecución.

**Criterios de Aceptación:**  
✅ El proyecto se crea correctamente con **Next.js y TypeScript**.  
✅ Eslint y Prettier están configurados y aplicados en el código.  
✅ La estructura de carpetas refleja una organización modular.  
✅ La aplicación se ejecuta sin errores en **modo desarrollo y producción**.  
✅ La documentación está disponible en el repositorio.

**Prioridad:** Alta  
**Dependencias:** Ninguna (es el primer paso del frontend).

----------

### **📌 Ticket 2: Configuración de Estilos Base con TailwindCSS**

📌 **Épica:** Configuración del Proyecto Frontend

**Título:** Configurar TailwindCSS como sistema de estilos base

**Descripción:**  
Se debe integrar **TailwindCSS** en el proyecto frontend, asegurando una estructura modular y alineada con **Clean Architecture y Vertical Slicing** para facilitar la escalabilidad y el mantenimiento del sistema de estilos.

**Tareas:**

-   Instalar **TailwindCSS** en el proyecto Next.js.
-   Configurar los archivos de **Tailwind (`tailwind.config.js`) y `postcss.config.js`**.
-   Definir un **sistema de diseño** con variables globales (colores, tipografía, espaciados).
-   Aplicar estilos base en un **archivo global de CSS**.
-   Agregar documentación en el repositorio sobre el uso de TailwindCSS en el proyecto.

**Criterios de Aceptación:**  
✅ **TailwindCSS está instalado y configurado** en el proyecto.  
✅ Se han definido variables globales de estilos en la configuración de Tailwind.  
✅ Se ha aplicado un archivo global de estilos con los ajustes base del diseño.  
✅ La documentación sobre el uso de TailwindCSS está disponible en el repositorio.

**Prioridad:** Alta  
**Dependencias:** Inicialización del Proyecto Frontend.

----------

### **📌 Ticket 3: Implementación de shadcn/ui y Soporte para Modo Oscuro**

📌 **Épica:** Configuración del Proyecto Frontend

**Título:** Integrar shadcn/ui y configurar el soporte para modo oscuro/claro

**Descripción:**  
Se debe instalar e integrar **shadcn/ui** como la librería de componentes de interfaz de usuario y configurar la funcionalidad de **cambio de tema (modo oscuro y claro)** para mejorar la experiencia visual del usuario.

**Tareas:**

-   Instalar **shadcn/ui** en el proyecto frontend.
-   Configurar **Next.js Theme Provider** para la gestión de temas.
-   Implementar un **componente de selección de tema** en la interfaz.
-   Asegurar la **persistencia del tema seleccionado** en el almacenamiento local del navegador.
-   Documentar la integración de **shadcn/ui** y la configuración del sistema de temas.

**Criterios de Aceptación:**  
✅ **shadcn/ui está instalado y operativo** en el proyecto.  
✅ El usuario puede cambiar entre **modo claro y oscuro** desde la interfaz.  
✅ La selección de tema se mantiene al recargar la página (persistencia en localStorage).  
✅ La documentación de integración y uso está disponible en el repositorio.

**Prioridad:** Alta  
**Dependencias:** Configuración de Estilos Base con TailwindCSS.

----------

### **📌 Ticket 4: Definición de la Estructura de Carpetas y Organización del Código**

📌 **Épica:** Configuración del Proyecto Frontend

**Título:** Definir la estructura de carpetas y la organización del código en el frontend

**Descripción:**  
Se debe establecer una **estructura de carpetas modular** siguiendo los principios de **Screaming Architecture, Clean Architecture y Vertical Slicing**, asegurando una separación clara entre presentación, lógica de negocio e infraestructura.

**Tareas:**

-   Definir y crear las **carpetas principales** del proyecto (ejemplo: `components`, `pages`, `services`, `hooks`, `context`, `utils`).
-   Separar las capas de **presentación, lógica de negocio e infraestructura** de acuerdo con las mejores prácticas.
-   Implementar una carpeta dedicada para **contextos globales y estados compartidos**.
-   Asegurar que la estructura permite la **escalabilidad y mantenibilidad** del proyecto.
-   Documentar la estructura y principios de organización del código en el repositorio.

**Criterios de Aceptación:**  
✅ La estructura de carpetas refleja una organización modular y escalable.  
✅ Se han separado correctamente las capas de presentación, lógica de negocio e infraestructura.  
✅ Existe una documentación clara en el repositorio sobre la organización del código.

**Prioridad:** Alta  
**Dependencias:** Inicialización del Proyecto Frontend.

----------

### **📌 Ticket 5: Configuración de Rutas y Navegación en el Frontend**

📌 **Épica:** Configuración del Proyecto Frontend

**Título:** Configurar el sistema de rutas y navegación en el frontend

**Descripción:**  
Se debe establecer un **sistema de enrutamiento utilizando Next.js**, asegurando que las rutas sigan una estructura organizada y escalable. También se debe definir una estrategia de **layouts** para la reutilización de componentes globales en la navegación.

**Tareas:**

-   Configurar el sistema de **enrutamiento dinámico de Next.js**.
-   Definir rutas base para **páginas principales** (`/`, `/login`, `/dashboard`).
-   Implementar **layouts globales** para reutilizar encabezados, pies de página y menús de navegación.
-   Crear un **archivo centralizado de rutas** para facilitar modificaciones y evitar errores en la navegación.
-   Documentar la configuración de rutas y navegación en el repositorio.

**Criterios de Aceptación:**  
✅ El sistema de enrutamiento de Next.js está configurado correctamente.  
✅ Las rutas base del proyecto están definidas y operativas.  
✅ Se han implementado layouts globales para la navegación.  
✅ Existe una documentación clara en el repositorio sobre la gestión de rutas.

**Prioridad:** Alta  
**Dependencias:** Definición de la Estructura de Carpetas y Organización del Código.

----------

### **📌 Ticket 6: Configuración de Comunicación con el Backend**

📌 **Épica:** Configuración del Proyecto Frontend

**Título:** Configurar la comunicación con el backend mediante API REST

**Descripción:**  
Se debe establecer un **módulo de comunicación con el backend** utilizando **fetch o axios**, asegurando una gestión eficiente de las solicitudes y respuestas. Este módulo debe seguir los principios de **Clean Architecture y Vertical Slicing** para garantizar una integración estructurada y escalable.

**Tareas:**

-   Instalar y configurar **axios** como cliente HTTP (opcional si se decide usar fetch).
-   Crear un **servicio centralizado** para gestionar las peticiones al backend.
-   Configurar **manejo global de errores** en las solicitudes API.
-   Definir una **configuración global** para URLs base y encabezados.
-   Documentar la estructura y el uso del módulo de comunicación en el repositorio.

**Criterios de Aceptación:**  
✅ El sistema de comunicación con el backend está implementado y centralizado.  
✅ Se ha configurado un manejo de errores adecuado en las solicitudes API.  
✅ La configuración global de URLs y encabezados está correctamente definida.  
✅ Existe una documentación clara en el repositorio sobre la integración con el backend.

**Prioridad:** Alta  
**Dependencias:** Configuración de Rutas y Navegación en el Frontend.

----------

### **📌 Ticket 7: Configuración de Manejo de Estado Global**

📌 **Épica:** Configuración del Proyecto Frontend

**Título:** Configurar el manejo de estado global en el frontend

**Descripción:**  
Se debe establecer un **sistema eficiente de manejo de estado** utilizando **React Context API o Zustand**, asegurando una arquitectura modular que permita la **gestión centralizada de datos compartidos** dentro de la aplicación.

**Tareas:**

-   Definir e implementar **proveedores de contexto** o **stores de Zustand** según la estrategia seleccionada.
-   Configurar un **módulo de estado global** para datos compartidos como usuario autenticado y configuración del tema.
-   Separar los estados en **módulos organizados** para mejorar la escalabilidad.
-   Integrar el estado global con el sistema de autenticación y configuración del frontend.
-   Documentar la estrategia de manejo de estado y su implementación en el repositorio.

**Criterios de Aceptación:**  
✅ El sistema de estado global está implementado y operativo.  
✅ Se ha configurado correctamente la gestión de sesión de usuario y preferencias de tema.  
✅ La arquitectura del estado global permite la escalabilidad y modularidad del código.  
✅ Existe una documentación clara en el repositorio sobre la gestión del estado global.

**Prioridad:** Alta  
**Dependencias:** Configuración de Comunicación con el Backend.

----------

### **📌 Ticket 8: Configuración del Sistema de Autenticación en el Frontend**

📌 **Épica:** Configuración del Proyecto Frontend

**Título:** Configurar el sistema de autenticación en el frontend utilizando Supabase Auth

**Descripción:**  
Se debe establecer la autenticación en el frontend utilizando **Supabase Auth**, garantizando una integración segura con el backend. El sistema debe permitir el inicio de sesión, cierre de sesión y protección de rutas para usuarios autenticados.

**Tareas:**

-   Integrar **Supabase Auth** en el frontend.
-   Implementar el flujo de **inicio de sesión y cierre de sesión**.
-   Configurar **protección de rutas** para que solo los usuarios autenticados puedan acceder a secciones privadas.
-   Manejar la **persistencia de sesión** en el navegador.
-   Documentar el flujo de autenticación y su integración en el repositorio.

**Criterios de Aceptación:**  
✅ Los usuarios pueden iniciar y cerrar sesión correctamente.  
✅ Las rutas protegidas solo son accesibles para usuarios autenticados.  
✅ La sesión del usuario se mantiene activa entre recargas de la página.  
✅ Existe una documentación clara en el repositorio sobre el sistema de autenticación.

**Prioridad:** Alta  
**Dependencias:** Configuración de Manejo de Estado Global.

----------

### **📌 Ticket 9: Configuración del Manejo de Errores y Validaciones en el Frontend**

📌 **Épica:** Configuración del Proyecto Frontend

**Título:** Configurar el sistema de manejo de errores y validaciones en el frontend

**Descripción:**  
Se debe establecer un **mecanismo de manejo de errores y validaciones** en la aplicación frontend, asegurando que los mensajes de error sean claros y que las entradas de usuario sean correctamente validadas antes de ser enviadas al backend.

**Tareas:**

-   Implementar un **gestor global de errores** para capturar y manejar respuestas del backend.
-   Configurar **mensajes de error personalizados** para solicitudes fallidas.
-   Implementar validaciones de formularios utilizando **Zod o React Hook Form**.
-   Garantizar que los errores se muestren de manera clara en la interfaz de usuario.
-   Documentar la estrategia de manejo de errores y validaciones en el repositorio.

**Criterios de Aceptación:**  
✅ Se ha implementado un **sistema global de manejo de errores** en la aplicación.  
✅ Los mensajes de error se muestran de manera clara y comprensible en la interfaz.  
✅ Las validaciones de formularios impiden el envío de datos incorrectos.  
✅ Existe una documentación clara en el repositorio sobre el manejo de errores y validaciones.

**Prioridad:** Alta  
**Dependencias:** Configuración del Sistema de Autenticación en el Frontend.

----------

### **📌 Ticket 10: Configuración de la Documentación Técnica del Frontend**

📌 **Épica:** Configuración del Proyecto Frontend

**Título:** Crear la documentación técnica del frontend para facilitar su mantenimiento y escalabilidad

**Descripción:**  
Se debe documentar la **arquitectura del frontend**, las convenciones de código y las integraciones clave, asegurando que el equipo de desarrollo tenga una referencia clara sobre el sistema.

**Tareas:**

-   Documentar la **estructura del proyecto**, incluyendo la organización de carpetas y módulos.
-   Definir y documentar **convenciones de código y buenas prácticas**.
-   Crear una guía de **instalación y configuración del entorno de desarrollo**.
-   Documentar la integración del frontend con el backend y **Supabase Auth**.
-   Almacenar la documentación en el repositorio (`README.md`, Wiki interna o Notion).

**Criterios de Aceptación:**  
✅ Existe un documento detallado sobre la **arquitectura del frontend**.  
✅ Se han definido y documentado las **convenciones de código** para el equipo de desarrollo.  
✅ La documentación incluye una **guía de instalación y configuración** del proyecto.  
✅ Se han documentado las integraciones clave, incluyendo la comunicación con **Supabase y el backend**.  
✅ La documentación está accesible en el repositorio para consulta del equipo.

**Prioridad:** Media  
**Dependencias:** Configuración del Manejo de Errores y Validaciones en el Frontend.

----------

## **📌 Tickets Backend**


### **📌 Ticket 1: Inicialización del Proyecto Backend**

📌 **Épica:** Configuración del Proyecto Backend

**Título:** Inicializar el proyecto backend con NestJS y TypeScript

**Descripción:**  
Se debe crear la base del proyecto backend utilizando **NestJS con TypeScript**, asegurando que la arquitectura siga los principios de **Clean Architecture, Hexagonal Architecture y DDD**, permitiendo modularidad y escalabilidad.

**Tareas:**

-   Crear el proyecto con **NestJS y TypeScript** mediante `npx nest new backend`.
-   Configurar **Eslint y Prettier** para mantener estándares de código.
-   Definir una **estructura inicial de carpetas** basada en principios arquitectónicos.
-   Verificar que el entorno de desarrollo y producción funcionan correctamente.
-   Agregar documentación en el repositorio (`README.md`) con instrucciones de instalación y ejecución.

**Criterios de Aceptación:**  
✅ El proyecto se crea correctamente con **NestJS y TypeScript**.  
✅ Eslint y Prettier están configurados y aplicados en el código.  
✅ La estructura de carpetas refleja una organización modular.  
✅ La aplicación se ejecuta sin errores en **modo desarrollo y producción**.  
✅ La documentación está disponible en el repositorio.

**Prioridad:** Alta  
**Dependencias:** Ninguna (es el primer paso del backend).

----------

### **📌 Ticket 2: Configuración de la Base de Datos con Supabase**

📌 **Épica:** Configuración del Proyecto Backend

**Título:** Configurar Supabase PostgreSQL como base de datos del backend

**Descripción:**  
Se debe establecer la conexión con **Supabase PostgreSQL**, asegurando compatibilidad con el ORM y alineación con **Clean Architecture y DDD**. También se debe configurar la seguridad de acceso a la base de datos utilizando **Row Level Security (RLS)** para gestionar permisos de usuarios.

**Tareas:**

-   Configurar **Supabase PostgreSQL** como la base de datos del backend.
-   Establecer la conexión con **Prisma ORM**, asegurando compatibilidad con Supabase.
-   Implementar **Row Level Security (RLS)** para restringir acceso a los datos según roles.
-   Configurar **variables de entorno seguras** para la conexión con la base de datos.
-   Documentar la configuración de la base de datos y su integración con Prisma en el repositorio.

**Criterios de Aceptación:**  
✅ Supabase PostgreSQL está correctamente configurado como la base de datos del backend.  
✅ Prisma ORM está integrado y conectado con Supabase.  
✅ Row Level Security (RLS) está implementado y funcional para restringir accesos.  
✅ La documentación de configuración y conexión está disponible en el repositorio.

**Prioridad:** Alta  
**Dependencias:** Inicialización del Proyecto Backend.

----------

### **📌 Ticket 3: Definición de la Estructura de Carpetas y Organización del Código en el Backend**

📌 **Épica:** Configuración del Proyecto Backend

**Título:** Definir la estructura de carpetas y organización del código en el backend

**Descripción:**  
Se debe establecer una **estructura modular y escalable** en el backend siguiendo **Clean Architecture, Hexagonal Architecture y DDD**, asegurando una separación clara entre las capas de dominio, aplicación, infraestructura y presentación.

**Tareas:**

-   Definir y crear las **carpetas principales** del backend (`src/domain`, `src/application`, `src/infrastructure`, `src/presentation`).
-   Separar las capas de **dominio (entidades), aplicación (casos de uso), infraestructura (repositorios, conexión a BD) y presentación (controladores y rutas)**.
-   Implementar una carpeta dedicada para **configuración global** (variables de entorno, seguridad).
-   Asegurar que la estructura permite la **escalabilidad y mantenibilidad** del proyecto.
-   Documentar la estructura de carpetas y principios de organización en el repositorio.

**Criterios de Aceptación:**  
✅ La estructura de carpetas sigue los principios de **Clean Architecture y DDD**.  
✅ Se han separado correctamente las capas de dominio, aplicación, infraestructura y presentación.  
✅ Existe una documentación clara en el repositorio sobre la organización del código.

**Prioridad:** Alta  
**Dependencias:** Configuración de la Base de Datos con Supabase.

----------

### **📌 Ticket 4: Configuración de Controladores, Servicios y Repositorios Base**

📌 **Épica:** Configuración del Proyecto Backend

**Título:** Configurar la arquitectura base de controladores, servicios y repositorios en el backend

**Descripción:**  
Se debe establecer la arquitectura base en el backend implementando las capas de **controladores (controllers), servicios (services) y repositorios (repositories)**, siguiendo **Clean Architecture, Hexagonal Architecture y DDD**. Esto garantizará una correcta separación de responsabilidades y escalabilidad del sistema.

**Tareas:**

-   Crear una **estructura de controladores**, asegurando que manejen la comunicación con el frontend.
-   Implementar una **capa de servicios** para encapsular la lógica de negocio.
-   Configurar una **capa de repositorios** que gestione la interacción con la base de datos a través de Prisma.
-   Integrar **inyección de dependencias** para desacoplar módulos y facilitar pruebas unitarias.
-   Documentar la arquitectura y la forma en que deben crearse nuevos módulos en el repositorio.

**Criterios de Aceptación:**  
✅ Los controladores están implementados y manejan las peticiones HTTP correctamente.  
✅ La lógica de negocio está encapsulada en los servicios.  
✅ La interacción con la base de datos se realiza a través de la capa de repositorios.  
✅ Se han aplicado correctamente los principios de **inyección de dependencias**.  
✅ Existe una documentación clara en el repositorio sobre la estructura del backend.

**Prioridad:** Alta  
**Dependencias:** Definición de la Estructura de Carpetas y Organización del Código en el Backend.

----------

### **📌 Ticket 5: Configuración del Sistema de Autenticación con Supabase**

📌 **Épica:** Configuración del Proyecto Backend

**Título:** Configurar el sistema de autenticación en el backend utilizando Supabase Auth

**Descripción:**  
Se debe establecer la autenticación de usuarios en el backend utilizando **Supabase Auth**, asegurando que la validación de credenciales y la gestión de sesiones sean seguras y escalables.

**Tareas:**

-   Integrar **Supabase Auth** en el backend para la autenticación de usuarios.
-   Configurar el flujo de **inicio de sesión, registro y cierre de sesión**.
-   Implementar validación de **tokens JWT** emitidos por Supabase.
-   Proteger rutas privadas asegurando que solo los usuarios autenticados puedan acceder.
-   Documentar la configuración del sistema de autenticación en el repositorio.

**Criterios de Aceptación:**  
✅ Supabase Auth está configurado y funcionando correctamente en el backend.  
✅ Los usuarios pueden autenticarse utilizando el flujo de login y logout de Supabase.  
✅ Las rutas protegidas solo permiten el acceso a usuarios autenticados con tokens JWT válidos.  
✅ Existe una documentación clara en el repositorio sobre el sistema de autenticación.

**Prioridad:** Alta  
**Dependencias:** Configuración de Controladores, Servicios y Repositorios Base.

----------

### **📌 Ticket 6: Configuración de la Gestión de Roles y Permisos con Supabase**

📌 **Épica:** Configuración del Proyecto Backend

**Título:** Configurar la gestión de roles y permisos en Supabase para restringir el acceso a los datos según el tipo de usuario

**Descripción:**  
Se debe implementar un sistema de **roles y permisos** en Supabase utilizando **Row Level Security (RLS)** para garantizar que los pacientes y profesionales solo puedan acceder a los datos que les corresponden.

**Tareas:**

-   Configurar **roles de usuario** en Supabase (paciente y profesional).
-   Implementar políticas de acceso con **Row Level Security (RLS)** para restringir la consulta y modificación de datos.
-   Asegurar que el backend valide los permisos de los usuarios antes de ejecutar operaciones en la base de datos.
-   Crear pruebas para validar que los permisos funcionan correctamente.
-   Documentar la estrategia de gestión de roles y permisos en el repositorio.

**Criterios de Aceptación:**  
✅ Los roles de usuario están correctamente configurados en Supabase.  
✅ Row Level Security (RLS) restringe el acceso a los datos según el rol del usuario.  
✅ El backend valida los permisos antes de ejecutar cualquier operación sobre la base de datos.  
✅ Existe una documentación clara en el repositorio sobre la gestión de roles y permisos.

**Prioridad:** Alta  
**Dependencias:** Configuración del Sistema de Autenticación con Supabase.

----------

### **📌 Ticket 7: Configuración de la Comunicación entre el Backend y Supabase**

📌 **Épica:** Configuración del Proyecto Backend

**Título:** Establecer la comunicación entre el backend y Supabase para la gestión de autenticación y base de datos

**Descripción:**  
Se debe configurar una integración eficiente entre el backend y Supabase para manejar la autenticación de usuarios y las operaciones sobre la base de datos de manera segura y estructurada.

**Tareas:**

-   Implementar una **capa de abstracción** en el backend para interactuar con Supabase.
-   Configurar métodos para **autenticación, validación de tokens y recuperación de usuarios**.
-   Establecer un sistema de **consultas seguras** a la base de datos mediante Prisma y Supabase.
-   Implementar un mecanismo de **manejo de errores y reintentos** para solicitudes fallidas.
-   Documentar la estrategia de comunicación con Supabase en el repositorio.

**Criterios de Aceptación:**  
✅ La comunicación entre el backend y Supabase está correctamente establecida.  
✅ Los métodos de autenticación y validación de tokens funcionan sin errores.  
✅ La interacción con la base de datos es segura y estructurada.  
✅ Existe documentación clara en el repositorio sobre la comunicación con Supabase.

**Prioridad:** Alta  
**Dependencias:** Configuración de la Gestión de Roles y Permisos con Supabase.

----------

### **📌 Ticket 8: Configuración de Seguridad y Protección de Datos en el Backend**

📌 **Épica:** Configuración del Proyecto Backend

**Título:** Implementar medidas de seguridad en el backend para proteger los datos sensibles y garantizar el cumplimiento normativo

**Descripción:**  
Se deben establecer e implementar medidas de **seguridad y protección de datos** en el backend, asegurando el cumplimiento de regulaciones como la **Ley 1581 de 2012 (Protección de Datos en Colombia)** y **GDPR** en caso de usuarios internacionales.

**Tareas:**

-   Configurar **cifrado en reposo** para datos sensibles en la base de datos de Supabase.
-   Implementar **TLS/HTTPS** para garantizar el cifrado en tránsito en todas las comunicaciones.
-   Aplicar mejores prácticas para el **almacenamiento seguro de tokens JWT**.
-   Establecer **políticas de retención y eliminación de datos**, alineadas con regulaciones de privacidad.
-   Documentar todas las medidas de seguridad implementadas en el repositorio.

**Criterios de Aceptación:**  
✅ Los datos sensibles almacenados en Supabase están cifrados correctamente.  
✅ Todas las comunicaciones entre el frontend, backend y Supabase utilizan **TLS/HTTPS**.  
✅ Se han aplicado medidas para evitar la exposición de tokens JWT en el backend.  
✅ Existe documentación clara en el repositorio sobre la seguridad y protección de datos en el backend.

**Prioridad:** Alta  
**Dependencias:** Configuración de la Comunicación entre el Backend y Supabase.

----------

### **📌 Ticket 9: Configuración del Sistema de Logs y Monitoreo en el Backend**

📌 **Épica:** Configuración del Proyecto Backend

**Título:** Implementar un sistema de logs y monitoreo para detectar errores y optimizar el rendimiento del backend

**Descripción:**  
Se debe establecer un **sistema de registro de eventos y monitoreo** en el backend para garantizar una gestión efectiva de errores, auditoría de acciones y supervisión del rendimiento del sistema.

**Tareas:**

-   Implementar un **sistema de logs estructurados** para registrar eventos importantes (errores, autenticaciones, accesos a la base de datos).
-   Configurar un **servicio de monitoreo** para capturar métricas de rendimiento y disponibilidad.
-   Asegurar que los registros sean **almacenados de manera segura** y accesibles para auditoría.
-   Definir alertas automáticas para errores críticos o eventos anómalos en el backend.
-   Documentar la estrategia de logs y monitoreo en el repositorio.

**Criterios de Aceptación:**  
✅ El sistema de logs registra eventos críticos del backend de manera estructurada.  
✅ Se han configurado métricas de monitoreo del sistema.  
✅ Se han definido alertas automáticas para errores o comportamientos inesperados.  
✅ Existe documentación clara en el repositorio sobre el sistema de logs y monitoreo.

**Prioridad:** Media  
**Dependencias:** Configuración de Seguridad y Protección de Datos en el Backend.

----------

### **📌 Ticket 10: Configuración de la Documentación Técnica del Backend**

📌 **Épica:** Configuración del Proyecto Backend

**Título:** Crear la documentación técnica del backend para facilitar su mantenimiento y escalabilidad

**Descripción:**  
Se debe documentar la **arquitectura del backend**, las convenciones de código y las integraciones clave, asegurando que el equipo de desarrollo tenga una referencia clara sobre el sistema.

**Tareas:**

-   Documentar la **estructura del backend**, incluyendo la separación de capas y patrones utilizados.
-   Definir y documentar **convenciones de código y buenas prácticas**.
-   Crear una guía de **instalación y configuración del entorno de desarrollo**.
-   Documentar la integración del backend con **Supabase (autenticación y base de datos)**.
-   Almacenar la documentación en el repositorio (`README.md`, Wiki interna o Notion).

**Criterios de Aceptación:**  
✅ Existe un documento detallado sobre la **arquitectura del backend**.  
✅ Se han definido y documentado las **convenciones de código** para el equipo de desarrollo.  
✅ La documentación incluye una **guía de instalación y configuración** del proyecto.  
✅ Se han documentado las integraciones clave, incluyendo la comunicación con **Supabase y el frontend**.  
✅ La documentación está accesible en el repositorio para consulta del equipo.

**Prioridad:** Media  
**Dependencias:** Configuración del Sistema de Logs y Monitoreo en el Backend.

----------

## **📌 Tickets Funcionalidades Principales**


### **📌 Ticket 1: Implementación del Agendamiento de Citas**

📌 **Épica:** Gestión de Citas

**Título:** Implementar la funcionalidad de agendamiento de citas en el sistema

**Descripción:**  
Se debe desarrollar la funcionalidad que permita a los **pacientes** agendar citas con los **profesionales** según su disponibilidad. La cita debe registrarse en la base de datos y generar una confirmación por correo electrónico.

**Tareas:**

-   Crear el **endpoint en el backend** para registrar una cita.
-   Validar que la fecha y hora seleccionadas estén **disponibles** antes de confirmar la cita.
-   Implementar la **interfaz en el frontend** para que los pacientes puedan seleccionar un profesional y su disponibilidad.
-   Integrar la funcionalidad con el sistema de **notificaciones** para enviar confirmaciones por correo.
-   Documentar el flujo de agendamiento en el repositorio.

**Criterios de Aceptación:**  
✅ Un paciente puede seleccionar un **profesional, fecha y hora** para agendar su cita.  
✅ La cita se **registra correctamente en la base de datos** con estado "Agendada".  
✅ Se **envía una confirmación por correo** al paciente y al profesional.  
✅ Se valida la disponibilidad antes de confirmar la cita.  
✅ Existe una documentación clara en el repositorio sobre el flujo de agendamiento.

**Prioridad:** Alta  
**Dependencias:** Configuración del Backend y Frontend completada.

----------

### **📌 Ticket 2: Implementación de la Modificación y Cancelación de Citas**

📌 **Épica:** Gestión de Citas

**Título:** Implementar la funcionalidad de modificación y cancelación de citas

**Descripción:**  
Se debe desarrollar la funcionalidad que permita a los **pacientes** modificar o cancelar sus citas, siempre que se haga con al menos **24 horas de anticipación**. El sistema debe reflejar los cambios en la base de datos y notificar tanto al paciente como al profesional.

**Tareas:**

-   Crear **endpoints en el backend** para modificar y cancelar citas.
-   Implementar **validaciones** que impidan cambios con menos de 24 horas de anticipación.
-   Diseñar la **interfaz en el frontend** para que los pacientes puedan gestionar sus citas.
-   Integrar la funcionalidad con el **sistema de notificaciones** para alertar sobre cambios.
-   Documentar el flujo de modificación y cancelación de citas en el repositorio.

**Criterios de Aceptación:**  
✅ Un paciente puede **modificar o cancelar** su cita con **al menos 24 horas de anticipación**.  
✅ Se **actualiza la base de datos** reflejando los cambios en la cita.  
✅ Se **envía una notificación** al paciente y al profesional informando el cambio.  
✅ Si la solicitud se hace con menos de 24 horas de anticipación, el sistema **bloquea la acción** y muestra un mensaje.  
✅ Existe una documentación clara en el repositorio sobre esta funcionalidad.

**Prioridad:** Alta  
**Dependencias:** Implementación del Agendamiento de Citas.

----------

### **📌 Ticket 3: Implementación de la Gestión de Disponibilidad por Parte del Profesional**

📌 **Épica:** Gestión de Disponibilidad

**Título:** Implementar la funcionalidad para que los profesionales gestionen su disponibilidad

**Descripción:**  
Se debe desarrollar la funcionalidad que permita a los **profesionales** definir y actualizar sus **horarios de disponibilidad**, asegurando que los pacientes solo puedan agendar citas dentro de estos períodos.

**Tareas:**

-   Crear el **endpoint en el backend** para que los profesionales configuren su disponibilidad.
-   Implementar la **interfaz en el frontend** para la gestión de disponibilidad.
-   Validar que cualquier cambio en la disponibilidad **no afecte citas ya agendadas**.
-   Integrar la funcionalidad con el sistema de **mensajes en tiempo real** para actualizar la disponibilidad visible en el frontend.
-   Documentar el flujo de gestión de disponibilidad en el repositorio.

**Criterios de Aceptación:**  
✅ Un profesional puede **definir y modificar sus horarios de disponibilidad**.  
✅ La información de disponibilidad se **actualiza en la base de datos** correctamente.  
✅ Si hay citas ya agendadas en un horario que el profesional quiere bloquear, el sistema **muestra una advertencia y no permite el cambio**.  
✅ Los cambios de disponibilidad se reflejan en **tiempo real** en el frontend.  
✅ Existe una documentación clara en el repositorio sobre la gestión de disponibilidad.

**Prioridad:** Alta  
**Dependencias:** Implementación del Agendamiento de Citas.

----------

### **📌 Ticket 4: Implementación de Notificaciones Automáticas de Citas**

📌 **Épica:** Sistema de Notificaciones

**Título:** Implementar el sistema de notificaciones automáticas mediante eventos internos

**Descripción:**  
Se debe desarrollar un **sistema de notificaciones basado en eventos internos** para informar a los pacientes y profesionales sobre sus citas en distintos momentos clave. Las notificaciones deben enviarse automáticamente sin necesidad de un endpoint específico, asegurando un **flujo desacoplado y escalable**.

**Tareas:**

-   Implementar un **sistema de eventos internos** en el backend para gestionar notificaciones (`AppointmentCreated`, `AppointmentCancelled`).
-   Crear un **listener de eventos** que escuche cambios en las citas y genere notificaciones en consecuencia.
-   Configurar un **proveedor de correo** (ejemplo: SendGrid o Supabase Auth con Magic Links).
-   Configurar **notificaciones en los siguientes eventos**:
    -   Confirmación inmediata tras agendar una cita.
    -   Recordatorio 24 horas antes de la cita.
    -   Recordatorio 1 hora antes de la cita.
    -   Notificación en caso de modificación o cancelación de la cita.
-   Implementar una **cola de procesamiento de notificaciones** para evitar bloqueos en la API.
-   Documentar el sistema de notificaciones en el repositorio.

**Criterios de Aceptación:**  
✅ Se emite un **evento interno** cuando se agenda, modifica o cancela una cita.  
✅ Un **listener de eventos** recibe la información y envía las notificaciones correspondientes.  
✅ Se integran **recordatorios automáticos** (24 horas y 1 hora antes).  
✅ Se notifica al paciente y al profesional en caso de modificación o cancelación.  
✅ Existe documentación clara en el repositorio sobre el sistema de notificaciones y su integración con eventos internos.

**Prioridad:** Alta  
**Dependencias:** Implementación del Agendamiento de Citas.

----------

### **📌 Ticket 5: Implementación de Restricciones de Cancelación y Modificación de Citas**

📌 **Épica:** Gestión de Citas

**Título:** Implementar restricciones para la cancelación y modificación de citas según reglas del sistema

**Descripción:**  
Se debe desarrollar un sistema que **restrinja la cancelación y modificación de citas con menos de 24 horas de anticipación**, asegurando que las reglas del sistema sean aplicadas correctamente y reflejadas en la interfaz de usuario.

**Tareas:**

-   Implementar una **validación en el backend** que impida la cancelación/modificación si faltan menos de 24 horas para la cita.
-   Configurar **mensajes de error claros** en la API cuando la acción no esté permitida.
-   Adaptar la **interfaz en el frontend** para reflejar estas restricciones.
-   Documentar las restricciones en el repositorio, asegurando su claridad para el equipo de desarrollo.

**Criterios de Aceptación:**  
✅ Si el paciente intenta modificar o cancelar una cita con menos de **24 horas de anticipación**, el sistema **rechaza la acción y muestra un mensaje claro**.  
✅ Las reglas de restricción están implementadas tanto en **backend (validaciones API)** como en **frontend (mensajes de interfaz)**.  
✅ Existe documentación clara sobre cómo se aplican las restricciones en el sistema.

**Prioridad:** Alta  
**Dependencias:** Implementación de la Modificación y Cancelación de Citas.

----------

### **📌 Ticket 6: Implementación de Mensajes de Disponibilidad en Tiempo Real**

📌 **Épica:** Gestión de Disponibilidad

**Título:** Mostrar mensajes en tiempo real sobre la disponibilidad de los profesionales

**Descripción:**  
Se debe desarrollar un sistema que **actualice en tiempo real la disponibilidad de los profesionales**, asegurando que los pacientes solo puedan seleccionar horarios realmente disponibles.

**Tareas:**

-   Implementar **WebSockets o suscripción a cambios en Supabase** para actualizar la disponibilidad en tiempo real.
-   Configurar la lógica en el **frontend** para recibir y reflejar los cambios sin necesidad de recargar la página.
-   Validar en el **backend** que al momento de agendar una cita, la disponibilidad no haya cambiado simultáneamente.
-   Implementar un **mensaje en la interfaz** que notifique al paciente si un horario seleccionado ya no está disponible.
-   Documentar la estrategia de actualización en tiempo real en el repositorio.

**Criterios de Aceptación:**  
✅ La disponibilidad de los profesionales se **actualiza en tiempo real** en la interfaz del paciente.  
✅ Si un horario ya no está disponible al momento de seleccionarlo, se muestra un **mensaje claro en la interfaz**.  
✅ Se ha implementado una estrategia eficiente para evitar **conflictos de disponibilidad** en el backend.  
✅ Existe una documentación clara sobre la actualización en tiempo real de la disponibilidad.

**Prioridad:** Media  
**Dependencias:** Implementación de la Gestión de Disponibilidad por Parte del Profesional.

----------

### **📌 Ticket 7: Implementación del Bloqueo de Agenda por Parte del Profesional**

📌 **Épica:** Gestión de Disponibilidad

**Título:** Permitir que los profesionales bloqueen su agenda para definir horarios no disponibles

**Descripción:**  
Se debe desarrollar la funcionalidad que permita a los **profesionales** bloquear horarios específicos o días completos en su agenda, evitando que los pacientes puedan agendar citas en esos períodos.

**Tareas:**

-   Crear el **endpoint en el backend** para que los profesionales bloqueen su agenda.
-   Implementar la **interfaz en el frontend** para que los profesionales puedan seleccionar horarios o días completos a bloquear.
-   Validar que un profesional **no pueda bloquear horarios donde ya existan citas agendadas** sin una acción previa.
-   Reflejar los **bloqueos en tiempo real** en el sistema de disponibilidad del paciente.
-   Documentar la funcionalidad de bloqueo en el repositorio.

**Criterios de Aceptación:**  
✅ Un profesional puede **bloquear horarios o días completos** en su agenda.  
✅ El sistema **impide bloquear horarios con citas ya agendadas**, mostrando un mensaje de advertencia.  
✅ Los horarios bloqueados **se actualizan en tiempo real** y no están disponibles para los pacientes.  
✅ Existe documentación clara en el repositorio sobre la funcionalidad de bloqueo de agenda.

**Prioridad:** Alta  
**Dependencias:** Implementación de la Gestión de Disponibilidad por Parte del Profesional.

----------

### **📌 Ticket 8: Implementación del Registro y Auditoría de Cambios en las Citas**

📌 **Épica:** Monitoreo y Seguridad

**Título:** Registrar y auditar todos los cambios realizados en las citas para trazabilidad del sistema

**Descripción:**  
Se debe desarrollar un sistema que registre automáticamente cualquier **creación, modificación o cancelación de citas**, almacenando información relevante para auditoría y control de cambios.

**Tareas:**

-   Implementar una **tabla de auditoría en la base de datos** para registrar cambios en las citas.
-   Configurar la lógica en el **backend** para registrar cada evento de cambio (`created`, `updated`, `cancelled`).
-   Incluir información relevante en cada registro de auditoría (ejemplo: usuario que realizó el cambio, fecha/hora, cambios específicos).
-   Implementar una **interfaz en el frontend** para que los administradores puedan consultar el historial de cambios.
-   Documentar la estrategia de auditoría en el repositorio.

**Criterios de Aceptación:**  
✅ Cada acción sobre una cita (creación, modificación, cancelación) se **registra en la base de datos** con detalles específicos.  
✅ Los administradores pueden **consultar el historial de cambios** desde el frontend.  
✅ Se garantiza la **integridad y seguridad de los registros**, evitando ediciones o eliminaciones indebidas.  
✅ Existe documentación clara sobre la implementación del registro de auditoría.

**Prioridad:** Media  
**Dependencias:** Implementación de la Modificación y Cancelación de Citas.

----------

### **📌 Ticket 9: Implementación de la Configuración Parametrizable de Reglas del Sistema**

📌 **Épica:** Configuración y Administración

**Título:** Permitir la configuración parametrizable de reglas del sistema desde un panel de administración

**Descripción:**  
Se debe desarrollar una funcionalidad que permita a los administradores configurar parámetros clave del sistema, como **el límite de tiempo para cancelaciones/modificaciones y el horario de atención de los profesionales**, asegurando que estas reglas sean aplicadas en toda la plataforma.

**Tareas:**

-   Crear una **tabla de configuración** en la base de datos para almacenar los parámetros del sistema.
-   Implementar **endpoints en el backend** para actualizar y obtener configuraciones.
-   Diseñar una **interfaz en el frontend** que permita a los administradores modificar los valores de configuración.
-   Asegurar que las reglas parametrizables sean **aplicadas en tiempo real** en el sistema.
-   Documentar la estrategia de configuración en el repositorio.

**Criterios de Aceptación:**  
✅ Los administradores pueden modificar las **reglas del sistema** desde una interfaz.  
✅ Los cambios en la configuración **se reflejan automáticamente** en las reglas de negocio.  
✅ Se asegura la **persistencia de las configuraciones** en la base de datos.  
✅ Existe documentación clara en el repositorio sobre la parametrización de reglas del sistema.

**Prioridad:** Alta  
**Dependencias:** Implementación de Restricciones de Cancelación y Modificación de Citas.

----------

### **📌 Ticket 10: Implementación del Monitoreo y Alertas del Sistema**

📌 **Épica:** Monitoreo y Seguridad

**Título:** Implementar un sistema de monitoreo y alertas para detectar problemas de disponibilidad o rendimiento

**Descripción:**  
Se debe desarrollar un **mecanismo de monitoreo** que permita detectar posibles problemas en el sistema, incluyendo **tiempos de respuesta elevados, errores recurrentes o indisponibilidad del servicio**, notificando a los administradores en caso de anomalías.

**Tareas:**

-   Implementar un **sistema de logs y métricas** en el backend para registrar eventos clave.
-   Configurar un **servicio de monitoreo** para capturar métricas de rendimiento y disponibilidad.
-   Implementar un sistema de **alertas automáticas** en caso de tiempos de respuesta altos o errores críticos.
-   Integrar las alertas con un **canal de notificaciones** (correo, Slack o dashboard interno).
-   Documentar la estrategia de monitoreo y alertas en el repositorio.

**Criterios de Aceptación:**  
✅ El sistema registra **métricas clave** (tiempo de respuesta de la API, tasa de errores, carga del servidor).  
✅ Se generan **alertas automáticas** cuando el sistema detecta problemas críticos.  
✅ Los administradores reciben **notificaciones en tiempo real** cuando ocurre una anomalía.  
✅ Existe una documentación clara en el repositorio sobre el sistema de monitoreo y alertas.

**Prioridad:** Media  
**Dependencias:** Implementación del Registro y Auditoría de Cambios en las Citas.

----------

