> Detalla en esta sección los prompts principales utilizados durante la creación del proyecto, que justifiquen el uso de asistentes de código en todas las fases del ciclo de vida del desarrollo. Esperamos un máximo de 3 por sección, principalmente los de creación inicial o  los de corrección o adición de funcionalidades que consideres más relevantes.
Puedes añadir adicionalmente la conversación completa como link o archivo adjunto si así lo consideras


## Índice

1. [Descripción general del producto](#1-descripción-general-del-producto)
2. [Arquitectura del sistema](#2-arquitectura-del-sistema)
3. [Modelo de datos](#3-modelo-de-datos)
4. [Especificación de la API](#4-especificación-de-la-api)
5. [Historias de usuario](#5-historias-de-usuario)
6. [Tickets de trabajo](#6-tickets-de-trabajo)
7. [Pull requests](#7-pull-requests)

---



## 1. Descripción general del producto

**Prompt 1:**

---
El objetivo final del proyecto es desarrollar un sistema de **gestión y control de agendamiento de citas** para distintos servicios, operando como una **"marca blanca"**, lo que permitirá su personalización para diferentes negocios.  

Para el **MVP**, nos enfocaremos inicialmente en el **agendamiento de citas para servicios de psicología y áreas relacionadas**. Antes de comenzar la documentación oficial, necesitamos recopilar información relevante para comprender mejor este sector y su funcionamiento.  

### **Instrucciones:**  
A continuación, abordemos cada uno de los siguientes puntos de manera detallada y ordenada:  

#### **1. Características y Requisitos para Servicios de Psicología**  
   - ¿Qué particularidades tiene el agendamiento en este ámbito?  
   - ¿Existen normativas o regulaciones específicas que debamos considerar? (Ejemplo: confidencialidad, protección de datos de los pacientes, etc.)  
   - ¿Cómo debería funcionar un sistema de citas para psicólogos? (Ejemplo: sesiones individuales, grupales, teleconsultas, manejo de disponibilidad)  
   - ¿Qué herramientas adicionales podrían ser útiles para profesionales de esta área? (Ejemplo: historial del paciente, recordatorios personalizados, pagos en línea)  

#### **2. Análisis del Mercado y Plataformas Existentes**  
   - ¿Qué sistemas o plataformas actuales ofrecen agendamiento de citas para psicólogos?  
   - ¿Cuáles son sus principales características, ventajas y desventajas?  
   - ¿Cómo se diferencian entre sí y qué tendencias están marcando el mercado?  
   - ¿Qué aspectos podríamos tomar como referencia y cuáles podríamos mejorar o innovar en nuestro sistema?  

#### **3. Identificación de Oportunidades y Diferenciación**  
   - ¿Qué problemas comunes enfrentan los psicólogos y sus pacientes con los sistemas actuales?  
   - ¿Existen nichos desatendidos o necesidades específicas que podríamos abordar con nuestra solución?  
   - ¿Cómo podríamos hacer que nuestro sistema se destaque y ofrezca un **valor diferencial** respecto a la competencia?  

#### **4. Factores Claves para la Escalabilidad y Adaptabilidad**  
   - Aunque iniciemos con el sector de psicología, ¿qué elementos del sistema deben diseñarse desde el inicio para facilitar su adaptación a otros sectores en el futuro?  
   - ¿Cómo podríamos estructurar el sistema para que sea flexible y configurable para distintos tipos de servicios profesionales?  


---

**Prompt 2:**

---
Eres un **Product Manager (PM) experto** en **sistemas de agendamiento y gestión de citas**. Tu tarea es construir un **Product Requirements Document (PRD)** basándote en un **documento preliminar** elaborado por un **Business Analyst (BA) experto en el área**.  

### **Instrucciones:**  
1. **Análisis Previo:**  
   - Lee y analiza el documento preliminar proporcionado.  
   - Genera un **resumen detallado** con los puntos clave, asegurando que refleje con precisión la información del documento original.  
   - Identifica y destaca cualquier **posible ambigüedad o falta de información** en el documento.  

2. **Definición del Alcance del PRD:**  
   - Enumera los **temas y secciones clave** que se incluirán en el PRD.  
   - Justifica la inclusión de cada punto en función de su relevancia para el sistema de agendamiento y gestión de citas.  
   - Si consideras que algún aspecto adicional debe ser incluido, menciónalo y explica su importancia.  

### **Formato de la Respuesta:**  
- **Resumen detallado del documento preliminar**.  
- **Lista de secciones clave del PRD**, con una breve explicación de cada una.  
- **Observaciones y recomendaciones** sobre posibles mejoras o aclaraciones necesarias antes de iniciar la construcción del PRD.  
---


**Prompt 3:**

---
Este MVP no incluye integración con calendarios externos, personalización avanzada ni modelo híbrido de pago. El pago se realizará en efectivo al momento de la cita. La gestión de disponibilidad será manual por los profesionales, con un sistema simple. Las reglas de cancelación serán básicas, y los roles de usuarios que se implementarán son los de **Paciente** y **Profesional**. El MVP no incluirá generación de reportes ni KPIs específicos por ahora.  

### **Responde las siguientes preguntas basándote en este contexto:**

#### **1. Requerimientos y Alcance**

- **¿Hay alguna funcionalidad mencionada en el documento preliminar que NO se incluirá en el MVP?**  
  *No se incluirán las funcionalidades de integración con calendarios externos, personalización avanzada, ni el modelo híbrido de pago. Solo se habilitará el pago en efectivo.*

- **¿La pasarela de pago estará disponible desde el MVP o solo se habilitará el pago en efectivo?**  
  *Solo se habilitará el pago en efectivo.*

- **¿Cómo se gestionará la disponibilidad en el MVP?**  
  *La disponibilidad será gestionada manualmente por los profesionales. No se implementará una integración con calendarios externos en esta versión.*

- **¿Existen reglas específicas para cancelaciones y reembolsos en esta primera versión?**  
  *Las reglas de cancelación serán básicas. Por ejemplo, el usuario deberá cancelar con X tiempo de antelación para poder recibir un reembolso o evitar cargos adicionales.*

#### **2. Usuarios y Roles**

- **¿Todos los roles (Paciente, Profesional, Administrador) estarán implementados desde el MVP o habrá alguna limitación inicial?**  
  *Solo estarán implementados los roles de Paciente y Profesional. El Administrador no será parte del MVP en esta fase.*

- **¿El Administrador tendrá acceso a reportes desde el MVP o esto será parte de una fase posterior?**  
  *La generación de reportes se implementará en una fase posterior.*

#### **3. Aspectos Técnicos y UX**

- **¿Hay alguna preferencia sobre tecnologías a usar para el desarrollo del MVP?**  
  *Se utilizarán las siguientes tecnologías:  
    - Backend: **NestJs**  
    - Frontend: **NextJs**  
    - Base de datos: **PostgreSQL***

- **¿Se definirá algún estándar de accesibilidad en esta versión o será considerado más adelante?**  
  *Se adoptará el estándar internacional de accesibilidad web **WCAG (Web Content Accessibility Guidelines)** desde el inicio para asegurar que el MVP cumpla con los criterios básicos de accesibilidad.*

- **¿El MVP incluirá recordatorios por WhatsApp y correo o solo uno de estos métodos?**  
  *Solo se implementará el envío de recordatorios por correo electrónico. WhatsApp se considerará en una fase posterior.*

#### **4. Validación y Métricas**

- **¿Cuáles son los indicadores clave de éxito (KPIs) para medir el desempeño del MVP?**  
  *No se establecerán KPIs específicos en esta fase del MVP. El enfoque está en lanzar la versión funcional lo más rápido posible.*

- **¿Cuál es el objetivo de tiempo estimado para lanzar el MVP?**  
  *El objetivo es lanzar el MVP en el **menor tiempo posible**, sin comprometer las funcionalidades esenciales.*
---

---

## 2. Arquitectura del Sistema

### **2.1. Diagrama de arquitectura:**

**Prompt 1:**

---
### **Rol y Objetivo**  
Eres un **Arquitecto de Software** con experiencia en el diseño y definición de arquitecturas para **sistemas de agendamiento y gestión de citas**. Tu tarea es construir un **Architecture Requirements Document (ARD)** basándote en un **Product Requirements Document (PRD)** elaborado por un **Product Manager (PM) experto**.  

### **Instrucciones:**  

1. **Análisis del PRD:**  
   - Revisa y analiza el **PRD** proporcionado, asegurando una comprensión completa de los requerimientos del sistema.  
   - Genera un **resumen técnico** con los puntos clave, enfocándote en las necesidades funcionales y no funcionales que impactan la arquitectura.  
   - Identifica **posibles ambigüedades, inconsistencias o vacíos técnicos** que requieran aclaración antes de proceder con la arquitectura.  

2. **Definición del Alcance del ARD:**  
   - Enumera las **secciones clave del ARD**, alineadas con buenas prácticas de documentación arquitectónica.  
   - Define los **principales componentes y decisiones arquitectónicas** que deben considerarse.  
   - Justifica la inclusión de cada punto en función de su impacto en el sistema y alineación con los requerimientos del PRD.  
   - Si consideras que algún aspecto técnico adicional debe ser tratado, menciónalo y explica su importancia.  

3. **Generación del Índice del ARD:**  
   - Construye un **índice estructurado** del ARD, siguiendo buenas prácticas de documentación arquitectónica.  
   - Asegúrate de incluir aspectos esenciales como:  
     - **Visión general de la arquitectura**  
     - **Decisiones clave y trade-offs**  
     - **Modelo de datos y almacenamiento**  
     - **Integraciones y dependencias externas**  
     - **Consideraciones de escalabilidad y seguridad**  

### **Formato de la Respuesta:**  
- **Resumen técnico del PRD**, con un enfoque en requerimientos clave.  
- **Lista de secciones del ARD**, con una breve descripción de cada una.  
- **Observaciones y recomendaciones** sobre aspectos técnicos que requieran mayor definición antes de continuar con la arquitectura.  
---


**Prompt 2:**

---
Al construir el **Architecture Requirements Document (ARD)**, se debe incluir una variedad de diagramas esenciales para garantizar una comprensión clara del sistema.  

#### **Diagramas Requeridos:**  
✅ **Casos de uso**  
✅ **Diagramas C4** (Niveles según necesidad)  
✅ **Modelado de base de datos**  
✅ **Diagrama de secuencia**  
✅ **Diagrama de flujo**  
✅ **Diseño del sistema y arquitectura de alto nivel**  

### **Tarea:**  
- Evalúa estos elementos y determina **qué mejoras pueden incorporarse al documento en esta fase**.  
- Identifica **qué aspectos deben trabajarse en fases posteriores**, justificando la postergación de ciertos diagramas si es necesario.  

Entrega un análisis estructurado que ayude a definir un enfoque iterativo para el desarrollo del ARD. 
---

**Prompt 3:**

---
Se deberán aplicar las siguientes modificaciones en este apartado:  

### **Reglas Generales:**  
✅ **Lenguaje:** Los nombres de los módulos, entidades de la base de datos y cualquier aspecto relacionado con el desarrollo deben estar en **inglés**.  

### **Modificaciones Específicas:**  

#### **3.1 Backend**  
Este debe cumplir con los siguientes principios y arquitecturas:  

- **Domain-Driven Design (DDD):**  
  - [Explicar cómo se aplicará en la organización del código y las entidades del dominio]  
- **Hexagonal Architecture:**  
  - [Definir cómo se estructurarán los adaptadores y puertos]  
- **Vertical Slicing:**  
  - [Indicar la segmentación del código para mejorar mantenibilidad y escalabilidad]  
- **Screaming Architecture:**  
  - [Describir cómo los nombres de los paquetes reflejarán el dominio del negocio]  
- **Clean Architecture:**  
  - [Explicar cómo se separarán las capas de la aplicación]  
- **SOLID & DRY Principles:**  
  - [Definir cómo se garantizarán buenas prácticas de desarrollo]  

📌 **Adicionalmente:**  
- Se utilizará **Prisma** para la gestión de la base de datos desde el backend.  
- Especificar los **patrones de diseño** que se implementarán bajo esta arquitectura.  

#### **3.2 Frontend**  
- Este apartado debe ser **mucho más detallado**, incluyendo descripciones **claras y completas** sobre el **funcionamiento global y detallado de cada flujo de usuario**.  
- Asegurar que cada componente y su interacción dentro del sistema estén bien documentados.  

#### **3.3 Base de Datos**  
- **Las entidades deben estar en inglés.**  
- No debe limitarse a solo tres tablas (**Users, Appointments, Availability**).  
- La estructura de la base de datos debe **cumplir con la normalización completa**, asegurando eficiencia y consistencia en los datos.  
---

### **2.2. Descripción de componentes principales:**

**Prompt 1:**

---
Ajusta el documento **ARD (Architecture Requirements Document)** en base a la nueva definición de la base de datos.  

### **Proceso de Actualización:**  
- La revisión se realizará **de forma iterativa**, ajustando **un punto a la vez**.  
- **Cada actualización debe ser aprobada** antes de continuar con el siguiente punto.  
- **Se debe mantener la estructura original** del documento ARD.  

### **Formato de Respuesta Esperado:**  
📌 **Sección a actualizar:** (Indicar la parte del documento)  
🔍 **Justificación del cambio:** (Explicar por qué es necesaria la modificación)  
✍ **Versión actualizada:** (Mostrar solo el contenido modificado)  
✅ **Esperando aprobación antes de continuar.**  

---


**Prompt 2:**

---
Carga los siguientes archivos en el contexto de este chat y utiliza su contenido para estructurar la información de la **página principal** de la plataforma.  

### 🎯 **Objetivo:**  
Transformar la información en un formato listo para ser implementado en la web, asegurando que:  
- Siga los **estándares de diseño y usabilidad web**.  
- Esté **claramente estructurada** para facilitar su integración.  
- **Capte la atención del usuario desde el primer momento**.  

### 📑 **Requisitos:**  
- **Organización efectiva** del contenido con jerarquía visual clara.  
- **Texto atractivo y persuasivo** para enganchar a los usuarios.  
- Adaptación a un diseño **moderno y responsive**, priorizando UX/UI.  
- **Uso de elementos clave** (títulos llamativos, subtítulos, bullet points, llamadas a la acción).  

### 🚀 **Formato de Entrega:**  
- Secciones organizadas con su respectivo contenido.  
- Propuesta de **titulares y subtítulos** impactantes.  
- Sugerencias de llamadas a la acción (CTA) efectivas.  

---

**Prompt 3:**

---
Carga los siguientes archivos en el contexto de este chat y utiliza su contenido para estructurar la información de la **página principal** de la plataforma.  

### 🎯 **Objetivo:**  
Transformar la información en un formato listo para ser implementado en la web, asegurando que:  
- Siga los **estándares de diseño y usabilidad web**.  
- Esté **claramente estructurada** para facilitar su integración.  
- **Capte la atención del usuario desde el primer momento**.  

### 📑 **Requisitos:**  
- **Organización efectiva** del contenido con jerarquía visual clara.  
- **Texto atractivo y persuasivo** para enganchar a los usuarios.  
- Adaptación a un diseño **moderno y responsive**, priorizando UX/UI.  
- **Uso de elementos clave** (títulos llamativos, subtítulos, bullet points, llamadas a la acción).  

### 🚀 **Formato de Entrega:**  
- Secciones organizadas con su respectivo contenido.  
- Propuesta de **titulares y subtítulos** impactantes.  
- Sugerencias de llamadas a la acción (CTA) efectivas.  
---

### **2.3. Descripción de alto nivel del proyecto y estructura de ficheros**

**Prompt 1:**

---
El desarrollo del proyecto seguirá un **flujo incremental**, en el que cada fase construye sobre la anterior.  

### **📌 Fase 1: Base Técnica Sólida**  
Esta primera fase es **crucial**, ya que establece los fundamentos de la infraestructura y arquitectura del proyecto. Para garantizar una arquitectura escalable, mantenible y alineada con buenas prácticas, el desarrollo debe cumplir con:  

#### **🛠 Cumplimiento de Arquitecturas y Principios:**  
- **Diseño Dirigido por el Dominio (DDD)**  
- **Arquitectura Hexagonal**  
- **Vertical Slicing**  
- **Screaming Architecture**  
- **Clean Architecture**  
- **SOLID y DRY**  

#### **📌 Patrones de Diseño Aplicables (En casos específicos):**  
- **Singleton** → Asegura una única instancia de una clase con un punto de acceso global.  
- **Factory** → Permite la creación de objetos sin especificar su clase exacta.  
- **Observer** → Facilita la comunicación entre objetos cuando hay cambios en su estado.  
- **Strategy** → Permite definir y cambiar algoritmos de forma intercambiable.  

Además, se debe garantizar una **separación modular**, dividiendo el sistema en módulos independientes que permitan la escalabilidad y el mantenimiento eficiente del proyecto.  

---

### **📌 Tarea a realizar:**  
Con base en estos lineamientos, **propón una primera versión de la estructura del proyecto**, asegurando que:  
1. **Defina una estructura de carpetas y módulos** siguiendo las arquitecturas y principios mencionados.  
2. **Incluya una descripción detallada** justificando la organización propuesta y su impacto en la escalabilidad y mantenibilidad del sistema.  
3. **Proporcione diagramas visuales** para facilitar la comprensión:  
   - 📍 **Diagrama de flujo** → Representación del flujo de ejecución y procesos clave.  
   - 📍 **Diagrama de secuencia** → Descripción de la interacción entre módulos y componentes en tiempo de ejecución.  


---

**Prompt 2:**

---
Debemos aplicar mejoras a la **primera entrega** del proyecto, optimizando la organización del código y la estructura del proyecto en **NestJS**.  

### **📌 Mejoras a Implementar:**  

#### **1️⃣ Organización del código compartido**  
- La lógica **compartida** y las **configuraciones globales** deberán ubicarse en la carpeta **` @libs  `**.  
- La aplicación principal (` @apps  `) solo contendrá la lógica específica del proyecto, manteniendo un código más limpio y modular.  

#### **2️⃣ Uso de Guards en lugar de Middlewares**  
- En lugar de **middlewares**, se utilizarán **guards**, ya que NestJS ofrece esta opción de manera nativa.  
- Si los guards son reutilizables en varias partes del sistema, deberán organizarse dentro de **`libs`**, siguiendo una estructura modular.  

#### **3️⃣ Configuración centralizada en `  @config.yaml  `**  
- El proyecto ya cuenta con una configuración base en **`config.yaml`**, donde se manejan parámetros clave como el **puerto de la aplicación**.  
- En la nueva estructura de directorios, se debe respetar la existencia de las carpetas y archivos actuales encargados de gestionar esta configuración.  
- Se debe proporcionar una **explicación clara del uso de estos archivos** dentro del proyecto.  

#### **4️⃣ Estructura modular en `libs`**  
- Todo lo que se ubique dentro de `libs` deberá estar **estructurado de manera modular**, similar a la carpeta existente **`config-manager`**.  
- Este enfoque garantizará que el proyecto sea más escalable y organizado.  

---

### **📌 Tarea a realizar:**  
1. **Proponer una nueva estructura de directorios** que incorpore estas mejoras, asegurando que:  
   - La configuración global y lógica compartida se ubiquen en `libs`.  
   - Guards reemplacen middlewares y se organicen adecuadamente.  
   - Se mantenga la carpeta y archivos actuales para `config.yaml`.  
2. **Explicar detalladamente** cada cambio realizado y su propósito.  
3. **Justificar cómo esta nueva estructura contribuye a la modularidad y escalabilidad del proyecto.**  

---

**Prompt 3:**

---

La nueva estructura del proyecto es **más ordenada y modular**, lo que facilita su construcción progresiva hasta la entrega final.  

Sin embargo, avanzaremos de forma **iterativa**, dividiendo el proceso en **fases y subfases**. Antes de comenzar a crear carpetas y archivos, es necesario **definir claramente las subfases de esta primera etapa**, basándonos en la nueva estructura establecida.  

### **📌 Tareas a realizar:**  
1. **Definir las subfases de la primera etapa**  
   - Desglosa las tareas en pasos más pequeños y organizados.  
   - Justifica la necesidad de cada subfase en función de la arquitectura propuesta.  

2. **Explicar cada subfase en detalle**  
   - Describe **qué se hará** en cada una y **por qué es importante**.  
   - Asegura que cada paso contribuya a una construcción iterativa e incremental del proyecto.  

3. **Primer cambio a realizar:**  
   - La nueva estructura de carpetas ha modificado la forma en que actualmente está organizada **`  @config-manager  `**.  
   - Este será **el primer cambio a realizar**, asegurando que se adapte correctamente a la nueva arquitectura del sistema.  

Una vez establecidas y aprobadas las subfases, procederemos con la creación de los directorios y archivos necesarios.  

---

### **2.4. Infraestructura y despliegue**

**Prompt 1:**

---
### 🧠 **Contexto:**

Cuento con dos proyectos:

-   ` → Backend de la aplicación @calenconnect-api 
-   ` → Frontend de la aplicación @calenconnect-ui 

Deseo desplegar ambos en **Amazon Web Services (AWS)** utilizando **instancias EC2**, pero **no tengo mucha experiencia previa** con el proceso de despliegue en la nube.

----------

### 🎯 **Objetivo:**

Obtener una **explicación clara, paso a paso**, de cómo realizar el despliegue de estos dos proyectos en **AWS EC2**, desde cero, incluyendo:

-   Configuración del entorno.
-   Instalación de dependencias.
-   Servidores recomendados.
-   Seguridad básica.
-   Ejecución de los proyectos en producción.

----------

### 📌 Requisitos específicos:

1.  **Explicación del flujo general:**
    
    -   ¿Qué es una instancia EC2 y cómo se utiliza?
    -   ¿Qué tipo de instancia se recomienda para comenzar?
2.  **Configuración inicial de EC2:**
    
    -   Creación de instancia desde AWS Console.
    -   Sistema operativo sugerido (ej: Ubuntu).
    -   Acceso vía SSH y configuración de puertos (22, 80, 443, 3000, etc.).
3.  **Despliegue del Backend (`):**
    
    -   Instalación de Node.js, yarn/npm, PM2.
    -   Clonado del repositorio, instalación de dependencias y variables de entorno.
    -   Levantar la API y mantenerla viva (ej: con PM2).
4.  **Despliegue del Frontend (`):**
    
    -   Construcción del proyecto (`npm run build`).
    -   Uso de `serve`, `nginx`, o similar para servir los archivos.
    -   Configuración de dominio si aplica.
5.  **Seguridad y mantenimiento básico:**
    
    -   Configurar `ufw` (firewall).
    -   Acceso solo por clave o certificado.
    -   (Opcional) HTTPS con Let's Encrypt.
6.  **Recomendaciones extra:**
    
    -   Buenas prácticas para mantener los servicios activos.
    -   Automatización sugerida (deploy scripts o GitHub Actions).
    -   Alternativas como Elastic Beanstalk o ECS (si se desea escalar a futuro).

----------

### 🛠️ Instrucciones:

1.  Explica todo el proceso como si fuera para alguien que lo hace por primera vez.
2.  Divide las instrucciones por etapas (EC2 setup, backend, frontend, seguridad).
3.  Usa ejemplos concretos (comandos de terminal, configuraciones, puertos).
4.  Asegúrate de explicar _por qué_ se hace cada paso, no solo cómo.
5.  Si aplica, incluye advertencias o errores comunes a evitar.

----------

### ✅ Resultado esperado:

-   Guía completa para desplegar ambos proyectos en AWS EC2.
-   Explicaciones claras y fáciles de seguir, incluso sin experiencia previa.
-   Configuración básica segura y funcional para producción.

---

**Prompt 2:**

---
### 🧠 **Contexto General:**

Como **DevSecOps Senior**, se te ha encomendado diseñar y desplegar la infraestructura necesaria para los proyectos:

-   ` (@calenconnect-api )
-   ` (@calenconnect-ui )

----------

### 🎯 **Objetivo del Prompt:**

Implementar la infraestructura usando **Terraform** dentro de la carpeta `, cumpliendo con los siguientes requisitos técnicos y operativos.

----------

### 📌 Requisitos de Infraestructura:

1.  **Instancias EC2:**
    
    -   Crear **dos instancias EC2** de tipo `t2.micro`, una para el backend y otra para el frontend.
    -   Sistema operativo sugerido: Amazon Linux 2 o Ubuntu 22.04.
2.  **Acceso a archivos desde S3:**
    
    -   Se provee un bucket S3 con los siguientes archivos en su raíz:
        -   `frontend.zip`
        -   `backend.zip`
    -   Cada instancia EC2 deberá:
        -   Tener **permisos adecuados (IAM Role + IAM Policy)** para acceder y descargar los archivos desde el bucket.
        -   Descargar el archivo correspondiente y descomprimirlo en el sistema.
3.  **Configuración de red y puertos:**
    
    -   El **backend** (`calenconnect-api`) debe ser accesible desde Internet en el **puerto 8080**.
    -   El **frontend** (`calenconnect-ui`) debe ser accesible desde Internet en el **puerto 3000**.
    -   Asegúrate de configurar correctamente los **grupos de seguridad (Security Groups)** para habilitar solo los puertos necesarios.
4.  **Credenciales de AWS:**
    
    -   No es necesario definir claves de acceso en Terraform, ya que ya están configuradas vía `aws configure`.
5.  **Automatización con Terraform:**
    
    -   Toda la infraestructura debe ser declarada utilizando Terraform.
    -   El código debe residir en la carpeta ` del proyecto.
    -   Incluye módulos y separa la configuración en `main.tf`, `variables.tf`, `outputs.tf`, y `provider.tf` según buenas prácticas.

----------

### 🛠️ Instrucciones:

1.  Genera una estructura base de Terraform con todos los archivos necesarios.
2.  Declara recursos para:
    -   VPC (si es necesaria), subredes, instancias EC2, security groups, roles e IAM policies.
3.  Proporciona los `user_data` scripts necesarios para que las EC2:
    -   Instalen dependencias (Node.js, unzip, etc.).
    -   Descarguen y descompriman el archivo `.zip` desde S3.
    -   Inicien el backend (puerto 8080) o el frontend (puerto 3000).
4.  Asegúrate de que la solución siga buenas prácticas DevSecOps:
    -   Principio de mínimo privilegio en IAM.
    -   Separación de responsabilidades en archivos Terraform.
    -   Comentarios que documenten lo necesario.

----------

### ✅ Resultado esperado:

-   Infraestructura desplegable con `terraform init` + `terraform apply`.
-   Dos instancias EC2 accesibles públicamente en los puertos indicados.
-   Código fuente de los proyectos descargado automáticamente desde S3.
-   Aplicaciones backend y frontend en funcionamiento tras el despliegue.

---

**Prompt 3:**

---
## 🔧 Contexto de Infraestructura y Despliegue

Se cuenta con una implementación actual de infraestructura como código utilizando Terraform: @terraform `.

Además, se tienen dos proyectos que deben ser desplegados:
- API: @calenconnect-api `
- Interfaz web (frontend): @calenconnect-ui `

El entorno debe cumplir con el siguiente requerimiento técnico:
- Utilizar Node.js versión 20 o superior

---

## ✅ Objetivo

Analiza la implementación actual de Terraform y los proyectos mencionados para lograr un despliegue exitoso de ambas aplicaciones. La validación debe contemplar todo el flujo, desde la creación de las instancias hasta la ejecución de los servicios.

---

## 📌 Instrucciones

1. **Valida la infraestructura definida en `:**
   - ¿Se están creando correctamente las instancias necesarias?
   - ¿Se están configurando de forma óptima para alojar las aplicaciones Node.js?
   - ¿Se asegura compatibilidad con Node.js 20+?

2. **Evalúa la preparación de los proyectos para su despliegue:**
   - `: ¿Está correctamente configurado para ejecutarse en producción? ¿Faltan variables de entorno, scripts de inicio, etc.?
   - `: ¿Puede construirse y desplegarse correctamente? ¿Está definido el build y el entorno de ejecución?

3. **Identifica los ajustes necesarios para garantizar un despliegue exitoso de ambos proyectos:**
   - Cambios en archivos Terraform (por ejemplo, en configuración de instancias, grupos de seguridad, variables, etc.)
   - Cambios en los proyectos (por ejemplo, estructura de carpetas, configuración de entorno, Dockerfiles si aplica, scripts de despliegue)

---

## 📝 Formato de respuesta esperado

- Explicación organizada por secciones: `Terraform`, `API`, `UI`
- Para cada sección, incluye:
  - Diagnóstico actual (qué está bien, qué falta)
  - Recomendaciones concretas de mejora
  - Justificación técnica de cada cambio sugerido
---

### **2.5. Seguridad**

**Prompt 1:**

---
Explica de manera detallada y clara las principales **regulaciones de seguridad y privacidad de datos**, incluyendo **GDPR y HIPAA**, así como otras normativas relevantes a nivel global.  

### **Requisitos de la respuesta:**  
1. **Definición de cada regulación:**  
   - Explica qué es cada regulación, su propósito y a qué sectores aplica.  
2. **Principales requisitos y obligaciones:**  
   - Describe los aspectos clave que deben cumplir las empresas y organizaciones.  
3. **Ejemplos de aplicación:**  
   - Proporciona casos de uso o ejemplos prácticos para facilitar la comprensión.  
4. **Comparación y diferencias:**  
   - Si es relevante, destaca diferencias entre regulaciones similares.  

La explicación debe ser **estructurada, clara y fácil de entender**, evitando tecnicismos innecesarios. 
---

**Prompt 2:**

---
Se necesita definir qué **regulaciones de seguridad y normativas específicas** aplican a una **aplicación en Colombia** que gestiona el **agendamiento de citas con profesionales de psicología**. Dado que la aplicación manejará **datos sensibles de salud y datos personales**, es fundamental garantizar el cumplimiento de las normativas vigentes para la protección de la información y la privacidad de los usuarios.

### **Instrucción:**

Investiga y explica en detalle las **regulaciones de seguridad y protección de datos** que aplican a este tipo de aplicación en **Colombia**. Asegúrate de incluir:

1.  **Normativas nacionales e internacionales aplicables:**
    
    -   Explica qué regulaciones deben cumplirse en Colombia, incluyendo la **Ley 1581 de 2012** (protección de datos personales) y otras normativas relevantes.
    -   Considera regulaciones internacionales como **GDPR (Europa)** e **HIPAA (EE.UU.)** si pueden influir en la aplicación, por ejemplo, en caso de manejo de usuarios extranjeros.
2.  **Requisitos clave de cumplimiento:**
    
    -   ¿Qué medidas de seguridad deben implementarse para proteger los datos personales y de salud?
    -   ¿Cuáles son las obligaciones legales de la empresa respecto a la recolección, almacenamiento y tratamiento de datos?
    -   ¿Qué derechos tienen los usuarios sobre su información?
3.  **Ejemplos de aplicación:**
    
    -   Casos prácticos de cómo estas regulaciones afectan el diseño y funcionamiento de la aplicación.
    -   Buenas prácticas que deben implementarse en términos de **seguridad, consentimiento del usuario, acceso a datos y almacenamiento seguro**.
4.  **Posibles sanciones por incumplimiento:**
    
    -   Explica qué riesgos legales enfrenta la empresa si no cumple con estas regulaciones.

La explicación debe ser **clara, estructurada y fácil de entender**, con ejemplos concretos que faciliten la comprensión.
---


**Prompt 3:**

---

Aquí tienes las respuestas detalladas:  

---

## **1. Reglas específicas de cancelación/modificación de citas**  

- **¿Cuánto tiempo antes de la cita puede un paciente modificarla o cancelarla?**  
  - Actualmente, la cancelación puede realizarse **con al menos 24 horas de antelación**.  
  - Este tiempo debe ser **parametrizable** dentro del sistema mediante un archivo de configuración.  
  - Al momento de agendar la cita y en la notificación por correo, se debe informar al usuario sobre este límite de cancelación.  

- **¿Hay restricciones específicas para evitar cancelaciones de última hora?**  
  - Sí, dado que la cancelación con menos de 24 horas de anticipación no está permitida.  
  - El sistema no debe permitir cancelaciones fuera del tiempo definido en la configuración.  
  - Se puede considerar una penalización para usuarios que cancelen frecuentemente en el límite permitido.  

---

## **2. Envío de notificaciones**  

- **¿Cuándo exactamente se enviarán los correos de confirmación y recordatorio?**  
  - **Confirmación:** Se enviará **de forma automática** en el momento en que se agenda la cita.  
  - **Recordatorios:** Aunque no se menciona en el contexto, sería recomendable definir una política de recordatorios (ejemplo: 24 horas y 1 hora antes de la cita).  

- **¿Los profesionales también recibirán recordatorios?**  
  - Sí, tanto el usuario que agendó la cita como el profesional recibirán la notificación de la cita asignada.  
  - Esto es clave para la gestión de la disponibilidad del profesional.  

---

## **3. Escalabilidad y optimización**  

- **¿Cómo se manejará la cantidad de citas diarias sin degradación del sistema?**  
  - No debe existir un **límite arbitrario de 500 citas diarias**.  
  - El sistema debe permitir **agendar citas sin restricciones** hasta que los profesionales ya no tengan espacios disponibles en el mes.  
  - Si un usuario intenta agendar y no hay disponibilidad, se debe **informar en tiempo real** con un mensaje claro.  
  - Se recomienda implementar una **lista de espera** o la opción de recibir una notificación si se libera un espacio.  

- **¿Cómo se garantizará la estabilidad del sistema bajo alta demanda?**  
  - Se debe implementar un **plan de pruebas de carga y estrés** que incluya:  
    1. **Pruebas de carga** para medir el rendimiento del sistema en condiciones normales y de alta demanda.  
    2. **Pruebas de estrés** para identificar el punto en el que la aplicación comienza a degradarse.  
    3. **Pruebas de escalabilidad** para evaluar el comportamiento del sistema al aumentar progresivamente la cantidad de citas y usuarios.  
    4. **Simulación de concurrencia**, probando el impacto de múltiples usuarios agendando citas simultáneamente.  

- **¿Qué medidas de optimización se deben considerar?**  
  - Implementar una **infraestructura escalable** que permita aumentar la capacidad del sistema según la demanda.  
  - Uso de **caching** para reducir la carga en la base de datos.  
  - Optimización de consultas y mejoras en la arquitectura del backend para soportar un alto volumen de transacciones.  
  - Implementación de **monitoreo en tiempo real** para detectar cuellos de botella y mejorar la estabilidad del sistema.  

---

## **4. Reglas de disponibilidad de los profesionales**  

- **¿Existen restricciones sobre cómo los profesionales pueden establecer su disponibilidad?**  
  - **Horarios de oficina:** De **7:00 a.m. a 5:00 p.m.**, aunque este horario debe ser **parametrizable** mediante un archivo de configuración.  
  - **Bloqueo de agenda:**  
    - Los profesionales pueden bloquear su agenda **por horas específicas o por el día completo**.  
    - Esto debe reflejarse en el sistema en tiempo real para evitar citas en horarios no disponibles.  
  - **Disponibilidad dinámica:** Si todos los cupos están ocupados, el sistema debe notificar al usuario que no hay disponibilidad en ese momento.  

---

## **5. Seguridad de datos**  

- **¿Qué regulaciones específicas (GDPR, HIPAA, etc.) se seguirán?**  

Dado que la aplicación operará en Colombia y manejará **datos sensibles de salud**, las regulaciones más relevantes son:  

🔹 **Prioridad Alta:** (Obligatorias y críticas para la seguridad de datos)  
1. **Ley 1581 de 2012** – Protección de Datos Personales (Ley principal de Habeas Data en Colombia).  
2. **Decreto 1377 de 2013** – Reglamentación de la Ley 1581 de 2012.  
3. **Resolución 1995 de 1999** – Normas para el manejo de historias clínicas.  
4. **Ley 2015 de 2020** – Historia Clínica Electrónica Interoperable.  
5. **Resolución 2654 de 2019** – Reglamentación de la Telesalud y Telemedicina.  
6. **Constitución Política de Colombia, Artículo 15** – Protección de datos personales y derecho a la intimidad.  

🔹 **Prioridad Media:** (Importantes, pero dependen de la interoperabilidad del sistema)  
7. **Ley 1419 de 2010** – Lineamientos para la Telesalud en Colombia.  
8. **Decreto 1074 de 2015** – Protección de datos personales en el sector Comercio, Industria y Turismo.  

🔹 **Prioridad Baja:** (Relevantes solo si la aplicación maneja aspectos financieros o se expande a otros mercados)  
9. **Ley 1266 de 2008** – Protección de datos personales en el ámbito financiero y crediticio.  
10. **Estándares Internacionales:** **GDPR (Europa)** y **HIPAA (EE.UU.)**, aplicables si la aplicación gestiona usuarios extranjeros o integra sistemas internacionales.  

---

## **Conclusión y Recomendaciones Finales**  

1. **Parámetros configurables:**  
   - Definir una interfaz de administración para gestionar reglas de cancelación, disponibilidad y notificaciones.  

2. **Estrategia de notificaciones:**  
   - Incluir **recordatorios automáticos** para mejorar la asistencia a las citas.  

3. **Pruebas de rendimiento:**  
   - Implementar **pruebas de carga y estrés** para garantizar la estabilidad del sistema sin un límite fijo de citas diarias.  

4. **Cumplimiento normativo:**  
   - Asegurar la implementación de la **Ley 1581 de 2012, la Resolución 1995 de 1999 y la Ley 2015 de 2020**, ya que son las más relevantes en Colombia.  

---


Importante: No generes aun ninguna de las fases 

---

### **2.6. Tests**

**Prompt 1:**

---
### 🧠 **Contexto:**

El proyecto actual desarrollado con **NestJS** utiliza **Prisma** como ORM, cuenta con una base de datos modelada y un archivo `seed.ts` que permite cargar datos iniciales para pruebas o desarrollo.

La base del código se encuentra bajo `@Codebase`, con estructura modular (`) ya definida.

----------

### 🎯 **Objetivo:**

Diseñar e implementar una estrategia completa de **pruebas funcionales e integrales** que abarque todos los flujos críticos de la aplicación, asegurando:

-   Alta cobertura.
-   Aislamiento de dependencias.
-   Datos de prueba controlados.
-   Cumplimiento de buenas prácticas y patrones de testing en NestJS.

----------

### 📌 Requisitos:

1.  **Auditoría inicial:**
    
    -   Revisar cada módulo (`) de forma independiente.
    -   Identificar sus casos de uso principales, controladores, servicios y dependencias externas.
2.  **Diseño de pruebas:**
    
    -   Implementar **pruebas funcionales** que validen cada endpoint expuesto.
    -   Crear **pruebas integrales** que validen la interacción entre servicios, controladores y base de datos (mockeada o en entorno de test).
3.  **Uso de mocks y datos simulados:**
    
    -   Evitar dependencias de la base de datos en pruebas unitarias.
    -   Para pruebas integrales o e2e:
        -   Utilizar datos del `seed.ts` como base de pruebas.
        -   O bien, usar `prisma-test-utils` o herramientas similares para manejar entornos transaccionales con datos temporales.
4.  **Buenas prácticas a seguir:**
    
    -   Estructura de pruebas: `__tests__` o `*.spec.ts`.
    -   Usar `@nestjs/testing` para configurar módulos de prueba.
    -   Mockear servicios externos (Ej: mail, notificaciones, auth).
    -   Separar claramente pruebas **unitarias**, **funcionales** e **integrales**.
5.  **Tecnologías sugeridas:**
    
    -   `Jest` (ya integrado en NestJS).
    -   `supertest` para pruebas funcionales HTTP.
    -   `faker` o `test-data-bot` para datos aleatorios.
    -   `ts-mockito`, `jest.mock`, o `vi.mock` (si usas Vitest).

----------

### 🛠️ Instrucciones:

1.  Analiza la estructura actual del proyecto.
2.  Proporciona un plan claro y escalonado para implementar pruebas en los distintos módulos.
3.  Sugiere la mejor estrategia para trabajar con datos mock usando Prisma.
4.  Proporciona una estructura base para test de ejemplo.
5.  (Opcional) Sugiere una posible estructura de carpetas para separar unit, functional e2e tests.

----------

### ✅ Resultado esperado:

-   Plan detallado para comenzar la implementación de pruebas.
-   Recomendaciones para estructurar test por módulo.
-   Prácticas de testing alineadas con NestJS y Prisma.
-   Fragmento de ejemplo de un `*.spec.ts` con datos simulados o mockeados.

---

**Prompt 2:**

---
### 🧠 **Contexto:**

En base a la información previamente compartida, se requiere llevar a cabo un proceso estructurado para alcanzar un objetivo específico (ej. implementación de pruebas, rediseño de componente, refactorización, etc.).

----------

### 🎯 **Objetivo:**

Definir un plan de trabajo dividido en **fases secuenciales**, donde cada una debe ser **desarrollada, validada y aprobada antes de avanzar** a la siguiente.  
Este enfoque garantiza calidad, control y claridad en cada paso del proceso.

----------

### 📌 Instrucciones:

1.  **Desglosa el objetivo general en fases claras y ordenadas.**
    
    -   Cada fase debe incluir:
        -   Descripción breve.
        -   Alcance de lo que debe lograrse.
        -   Entregables esperados.
        -   Dependencias si las hay (qué debe estar listo antes de avanzar).
2.  **Al completar cada fase:**
    
    -   Se presentará para su validación.
    -   Una vez **aprobada explícitamente**, se podrá continuar con la siguiente fase.
3.  **Consideraciones:**
    
    -   Las fases deben ser lo suficientemente específicas para medir el progreso.
    -   El avance debe ser progresivo, sin saltarse fases.
    -   Si hay necesidad de retroceder por cambios, se deberá indicar qué fase se ve afectada.

----------

### 🛠️ Instrucciones:

1.  Analiza el objetivo general del proceso.
2.  Divide el trabajo en **fases numeradas y progresivas**.
3.  Para cada fase, incluye:
    -   Nombre de la fase.
    -   Objetivo.
    -   Acciones clave.
    -   Resultado esperado (qué se valida).
4.  Espera validación antes de continuar con la siguiente fase.

----------

### ✅ Resultado esperado:

-   Lista estructurada de fases a seguir.
-   Claridad sobre el orden, entregables y puntos de validación.
-   Flujo de trabajo controlado y validado paso a paso.
---

**Prompt 3:**

---
### 🎯 **Objetivo:**

Iniciar la **implementación fase por fase**, asegurando que **cada etapa sea revisada, validada y aprobada** antes de avanzar a la siguiente. Este enfoque garantiza control, calidad y alineación continua con los objetivos del proyecto.

----------

### 📌 Instrucciones de trabajo:

-   Procederemos con la **implementación secuencial** de las fases previamente definidas.
-   **Cada fase será entregada y documentada** para su revisión.
-   No se continuará a la siguiente fase hasta que la actual haya sido **validada y aprobada explícitamente**.
-   En caso de que surjan observaciones, se ajustará lo necesario antes de continuar.

----------

### ✅ Resultado esperado:

-   Flujo de trabajo progresivo, validado paso a paso.
-   Registro claro del avance por fase.
-   Aseguramiento de calidad y cumplimiento de requisitos en cada etapa.


---
 

### 3. Modelo de Datos

**Prompt 1:**

---
### **Instrucciones para la Modificación de la Sección 7**  

Se deberán aplicar las siguientes modificaciones en la **Sección 7** para mejorar la claridad y el nivel de detalle:  

#### **7.3 Modelo de Base de Datos**  
- El modelo debe ser **mucho más completo**, incluyendo:  
  ✅ **Nombre de las columnas** de cada tabla.  
  ✅ **Tipos de datos** de cada atributo.  
  ✅ **Llaves primarias y foráneas** correctamente definidas.  
  ✅ **Relaciones entre tablas** con detalles de cardinalidad.  
  ✅ **Cualquier otra información relevante** para un mejor contexto.  
- La base de datos debe estar **totalmente normalizada** para garantizar eficiencia y consistencia.  
- **Genera un diagrama entidad-relación (ER)** en **sintaxis Mermaid**, utilizando la versión actualizada, sin omitir ningún detalle.  

#### **7.6 Diseño del Sistema y Arquitectura de Alto Nivel**  
- Incluir un **diagrama visual en sintaxis Mermaid** para representar la arquitectura de alto nivel del sistema.  
- Asegurar que el diagrama refleje de manera clara **componentes clave, módulos y sus interacciones**.  

### **Tarea:**  
🔹 **Entrega nuevamente toda la Sección 7** aplicando estos cambios.  

---

**Prompt 2:**

---
La base de datos del proyecto utilizará **PostgreSQL**, almacenada en **Supabase**. Supabase ya incluye un esquema predeterminado llamado **`auth`**, el cual será clave para la definición del modelo de base de datos del proyecto.  

Antes de proceder con el diseño del modelo, proporciona un **detalle completo** sobre la estructura del esquema **`auth`** en Supabase, incluyendo:  
- 📌 **Tablas y relaciones** dentro del esquema.  
- 🔍 **Campos clave y sus tipos de datos**.  
- 🔑 **Restricciones y reglas de autenticación** integradas.  
- ⚙️ **Funciones o triggers relevantes**.  

Esta información servirá como base para definir el modelo de datos del proyecto de manera coherente.  


---

**Prompt 3:**

---
Genera un **modelo ER** utilizando la sintaxis de **Mermaid** (asegurándote de que no contenga errores de sintaxis) que incluya:

1. Las **tablas existentes** en el esquema **`auth`** (utilizadas en el MVP) proporcionado por Supabase para autenticación y registro de usuarios.
2. Las **nuevas tablas** que se deberán crear para cubrir los requerimientos del MVP.

### **Requisitos del Modelo:**  
- **Normalización completa:** Asegúrate de que las nuevas tablas cumplan con las reglas de normalización para evitar redundancias.
- **Detalles y justificaciones:**  
  - Describe y justifica cada tabla y sus atributos.
  - Explica las relaciones entre las tablas, detallando claves primarias, foráneas y cualquier restricción relevante.
- **Enfoque MVP y escalabilidad:**  
  - El modelo debe reflejar las funcionalidades previstas para el MVP.
  - Debe ser lo suficientemente escalable para incorporar futuras funcionalidades o mejoras en fases posteriores.
- **Contexto de autenticación:**  
  - Considera que la autenticación y el registro de usuarios se gestionarán a través de Supabase, utilizando el esquema `auth`.

### **Formato de Respuesta Esperado:**  
- Código en sintaxis **Mermaid** para el diagrama ER.
- Sección descriptiva que incluya:
  - **Listado de tablas:** existentes y nuevas.
  - **Descripción de atributos y justificación:** de cada tabla.
  - **Explicación de relaciones:** entre tablas.

---

---

### 4. Especificación de la API

**Prompt 1:**

**Prompt 2:**

**Prompt 3:**

---

### 5. Historias de Usuario

**Prompt 1:**

---

### **Rol y Objetivo** 

Eres un **Product Owner (PO)**, con experiencia avanzada en la gestión de productos digitales y generación de historias de usuario, será responsable de transformar los requerimientos del **PRD** (Product Requirements Document) y el **ARD** (Architecture Requirements Document) en artefactos de trabajo claros y bien estructurados para el equipo de desarrollo.  

Todas las tareas se abordarán en **fases secuenciales**, asegurando una revisión detallada antes de avanzar a la siguiente. Cada fase deberá ser **analizada, corregida y aprobada** antes de continuar con la siguiente. Esto aplica tanto a la comprensión de los documentos base (PRD y ARD) como a la generación y validación de historias de usuario y tickets de trabajo.  

---

## **Fases de Trabajo y Validación**  

### **Fase 1: Análisis y Comprensión del PRD y ARD**  
✅ **Objetivo:** Comprender a fondo los requerimientos del sistema antes de definir historias de usuario o tareas técnicas.  
📌 **Proceso:**  
1. **Revisión del PRD:**  
   - Analizar el **PRD generado por el Product Manager (PM) experto**, asegurando que los requerimientos funcionales y no funcionales estén bien definidos.  
   - Extraer los **objetivos clave del producto** y validar su alineación con la visión estratégica.  
   - Identificar **brechas o ambigüedades** en la definición de los requisitos y documentarlas para revisión.  

2. **Revisión del ARD:**  
   - Evaluar el **ARD proporcionado por el Arquitecto de Software experto**, comprendiendo la arquitectura propuesta.  
   - Identificar **componentes clave, patrones de diseño, integraciones y dependencias técnicas** que influencian la planificación del producto.  
   - Documentar cualquier restricción técnica o decisión arquitectónica relevante para la planificación del desarrollo.  

🎯 **Criterios de aprobación:**  
- Todos los requisitos deben estar **claros y alineados** entre PRD y ARD.  
- Cualquier inconsistencia debe ser **reportada y ajustada** antes de avanzar.  

---

### **Fase 2: Generación de Historias de Usuario y Tickets de Trabajo**  
✅ **Objetivo:** Crear y validar historias de usuario y tickets de trabajo de manera iterativa.  
📌 **Proceso:**  
1. Generar historias de usuario siguiendo el formato estándar:  
   - **Título:** Nombre claro y conciso.  
   - **Descripción:** Explicación del valor que aporta la historia al usuario.  
   - **Criterios de aceptación:** Condiciones específicas que deben cumplirse para considerar la historia completa.  
   - **Prioridad:** Nivel de importancia dentro del backlog.  
   - **Dependencias:** Relación con otros tickets o requerimientos técnicos.  

2. Validar y aprobar cada historia de usuario antes de continuar con la siguiente.  

3. Clasificar y generar los tickets de trabajo en **épicas, historias de usuario y tareas técnicas**, asegurando una correcta granularidad.  

🎯 **Criterios de aprobación:**  
- Cada historia de usuario debe ser **revisada y corregida** si es necesario antes de seguir con la siguiente.  
- Los tickets deben ser **claros, viables y alineados** con los requerimientos técnicos definidos en el ARD.  

---

### **Fase 3: Documentación Complementaria**  
✅ **Objetivo:** Asegurar que el equipo tenga información clara sobre la estructura del sistema y sus principales componentes.  
📌 **Proceso:**  
1. Elaborar la **Descripción de Componentes Principales**, detallando su propósito y funcionalidad dentro del sistema.  
2. Documentar los **flujos de trabajo** relevantes, asegurando alineación entre requisitos de negocio y decisiones técnicas.  
3. Agregar un **diccionario de términos** con definiciones clave extraídas del PRD y ARD para mejorar la comunicación entre equipos.  

🎯 **Criterios de aprobación:**  
- Cada sección debe ser validada y corregida antes de finalizar el proceso.  
- La documentación debe estar completa y alineada con las necesidades del equipo de desarrollo.  

---

## **Formato de la Respuesta:**  
1. **Resumen del PRD y ARD** (foco en objetivos clave, componentes técnicos y restricciones).  
2. **Lista de Historias de Usuario y Tickets** (con descripción, criterios de aceptación y prioridad).  
3. **Documentación de Componentes Principales** (explicación de módulos clave y su función dentro del sistema).  
4. **Observaciones y Recomendaciones** (sobre posibles mejoras o puntos críticos a considerar antes del desarrollo).  



---

**Prompt 2:**

---

Con base en este nuevo contexto, el trabajo se realizará de forma **iterativa y secuencial**, asegurando que cada fase pase por un **proceso de revisión y aprobación** antes de avanzar a la siguiente.

### **Reglas del proceso:**

1.  **Fases de desarrollo:** Cada fase será **analizada, revisada y aprobada individualmente** antes de continuar con la siguiente. No se podrá avanzar sin una validación previa.
2.  **Historias de usuario y tickets:**
    -   Se generarán **uno por uno**, garantizando que cada historia y ticket sean revisados y aprobados antes de proceder con el siguiente.
    -   Se deben cumplir los **criterios de aceptación** y alinearse con los requerimientos establecidos en el contexto.
3.  **Correcciones y ajustes:**
    -   Si una fase o historia de usuario requiere ajustes, deberá ser corregida antes de ser aprobada.
    -   Solo cuando una fase o historia esté completamente validada, se podrá continuar con la siguiente.

Este enfoque asegura un **control preciso, alta calidad y alineación con los objetivos del proyecto**.

---

**Prompt 3:**

---

Para el desarrollo tanto del **frontend** como del **backend**, se debe garantizar el cumplimiento de los siguientes principios y arquitecturas:  

### **Cumplimiento de Arquitecturas y Principios**  
- **Diseño Dirigido por el Dominio (DDD)**: Garantizar que el modelo de negocio sea el centro del diseño.  
- **Arquitectura Hexagonal**: Asegurar una separación clara entre lógica de negocio, infraestructura y adaptadores.  
- **Vertical Slicing**: Organizar las funcionalidades en módulos independientes y manejables.  
- **Screaming Architecture**: La estructura del código debe reflejar claramente la funcionalidad principal del sistema.  
- **Clean Architecture**: Implementar capas bien definidas, separando detalles de implementación.  
- **Principios SOLID y DRY**: Mantener código modular, reutilizable y fácil de mantener.  

---

## **Tareas a Realizar:**  

1. **Validación y Ajuste de Historias de Usuario**  
   - Revisar si la historia de usuario actual cumple con los principios arquitectónicos mencionados.  
   - Si es necesario, **modificar o reestructurar la historia** para garantizar alineación con estos principios.  
   - Asegurar que las historias de usuario sean claras, implementables y alineadas con la arquitectura definida.  

2. **Iteración y Continuidad**  
   - Si la historia revisada está correctamente estructurada y alineada con los principios arquitectónicos, proceder con la siguiente historia de usuario.  
   - En caso de modificaciones, asegurarse de que sean validadas antes de continuar.  

---

## **Formato de la Respuesta Esperada:**  
- **Historia de usuario revisada o ajustada**, con criterios de aceptación claros.  
- **Justificación de cambios** en caso de que se hayan realizado modificaciones.  
- **Confirmación de cumplimiento** de los principios arquitectónicos o detalles sobre qué aspectos aún requieren ajuste.  
- **Siguiente historia de usuario** si la anterior ya ha sido aprobada.

---


---

### 6. Tickets de Trabajo

**Prompt 1:**

---

Realicemos una **revisión rápida y estructurada del backlog** para asegurarnos de que todo esté correctamente definido y alineado con los objetivos del proyecto.  

### **Puntos a Evaluar en la Revisión del Backlog:**  
- **Coherencia y completitud**: ¿Todas las historias de usuario están bien definidas y alineadas con sus respectivas épicas?  
- **Priorización**: ¿El backlog refleja correctamente el orden en que deben desarrollarse las funcionalidades?  
- **Criterios de aceptación**: ¿Cada historia tiene criterios claros y medibles para su validación?  
- **Dependencias**: ¿Existen historias o tickets que dependan de otros antes de ser implementados?  

### **Fases a Seguir para la Generación de Tickets:**  
1. **Análisis del backlog**: Identificar qué historias requieren tickets específicos y validar su alineación con las épicas definidas.  
2. **Desglose en tareas**: Convertir cada historia de usuario en **tickets detallados**, asegurando que cada uno represente una acción clara para los desarrolladores.  
3. **Asignación a épicas**: Cada ticket debe estar correctamente vinculado a su respectiva épica para mantener la organización del backlog.  
4. **Priorización y validación**: Ordenar los tickets según su importancia y validar que no haya dependencias bloqueantes.  
5. **Revisión final**: Asegurar que los tickets cumplen con los estándares definidos antes de ser asignados al equipo.  

### **Formato de la Respuesta Esperada:**  
- **Estado del backlog** tras la revisión (correcto o con ajustes necesarios).  
- **Fases detalladas para la generación de tickets**, indicando cualquier aspecto clave a considerar.  
- **Observaciones adicionales o mejoras recomendadas**.  


---

**Prompt 2:**

---

Antes de continuar con la siguiente fase, actualizaremos el contexto para asegurarnos de que **toda la información relevante esté presente** y alineada con lo que se ha creado hasta el momento.  

### **Actualización del Contexto:**  
- Se compartirá un documento que contendrá **todas las épicas e historias de usuario creadas hasta ahora**.  
- Este documento servirá como referencia para garantizar que la generación de tickets esté bien estructurada y alineada con el backlog existente.  

### **Fase de Generación de Tickets:**  
- La creación de tickets se trabajará **de manera iterativa**.  
- Cada ticket deberá ser **revisado y aprobado** antes de continuar con el siguiente.  
- Se debe asegurar que cada ticket esté correctamente vinculado a su **épica e historia de usuario correspondiente**.  

### **Formato de la Respuesta Esperada:**  
- **Confirmación de la actualización del contexto** tras revisar el documento compartido.  
- **Inicio de la fase de generación de tickets**, asegurando que cada uno siga el proceso de revisión y aprobación antes de avanzar.  
- **Observaciones o ajustes recomendados** si se identifica algún aspecto a mejorar antes de continuar.  

---

**Prompt 3:**

---

Dado que la **creación de los tickets de trabajo** para cada historia de usuario ha finalizado, antes de proceder a definir la siguiente fase o fases, realiza lo siguiente:  

### **1. Resumen de las Fases Completadas**  
- Enumera **todas las fases que se han completado** hasta el momento.  
- Destaca los **puntos clave y logros** de cada fase.  

### **2. Puntos Importantes de Cada Fase**  
- ¿Cuáles fueron los aspectos más relevantes o desafíos superados en cada fase?  
- ¿Qué decisiones críticas se tomaron y cómo impactaron el desarrollo del proyecto?  

### **3. Conclusión General**  
- ¿Cómo se encuentra el estado actual del proyecto después de estas fases?  
- ¿Está todo alineado con los objetivos iniciales y las expectativas del MVP?  
- ¿Existen observaciones o ajustes finales antes de avanzar?  

### **4. Definición de la Siguiente Fase**  
- Con base en el resumen y la conclusión, indica **cuál es la siguiente fase** o si ya se considera finalizado el proceso actual.  

---

## **Formato de la Respuesta Esperada:**  
- **Resumen de fases completadas** con puntos clave.  
- **Conclusión general** del estado actual del proyecto.  
- **Propuesta de la siguiente fase** o confirmación de finalización.  



---

---

### 7. Pull Requests

**Prompt 1:**

**Prompt 2:**

**Prompt 3:**
