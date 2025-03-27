# CalenConnect - Sistema de Agendamiento de Citas

## ⚠️ Importante
Antes de comenzar, asegúrate de:
1. Clonar o actualizar los tres repositorios del proyecto para obtener la versión más reciente de la documentación y el código:
   ```bash
   # Clonar repositorios
   git clone https://github.com/Jeferson96/AI4Devs-Final-Project-JDCH.git
   git clone https://github.com/Jeferson96/calenconnect-api.git
   git clone https://github.com/Jeferson96/calenconnect-ui.git

   # O actualizar si ya los tienes
   git pull origin main
   ```

2. Revisar los videos demostrativos del proyecto:
   📹 **Recursos Audiovisuales:**
   - **Ubicación:** [Carpeta de Videos en Google Drive](https://drive.google.com/drive/folders/1pL2zKpTF9GjnztG1J_vUYJ3pWwoTNizd?usp=sharing)
   - **Contenido disponible:**
     - Demo funcional del sistema
     - Tutorial de instalación y configuración
     - Guía de desarrollo

## 📁 Estructura del Proyecto

El proyecto está distribuido en tres repositorios independientes para un mejor control de versiones:

### 1. Repositorio Global (Documentación)
**URL:** https://github.com/Jeferson96/AI4Devs-Final-Project-JDCH.git

Contiene:
- 📝 Documentación completa del proyecto
- 📊 Diagramas de arquitectura
- 🔍 Especificaciones técnicas
- 📋 Guías de instalación
- 🔄 Scripts de integración
- 🚀 Configuración de despliegue

### 2. Repositorio Backend (API)
**URL:** https://github.com/Jeferson96/calenconnect-api.git

Contiene:
- 🖥️ Código fuente del backend (NestJS)
- 🗄️ Modelos de datos
- 🔐 Configuración de seguridad
- 🧪 Tests unitarios y de integración
- 📡 Endpoints de la API

#### Variables de Entorno Backend
> **⚠️ Nota**: Credenciales temporales para demostración

Crea un archivo `.env` en la raíz del proyecto:
```bash
NODE_ENV=production

# Conexión a base de datos de prueba
DATABASE_URL="postgresql://postgres.dvbqvvgltduwpmkwhlcf:T6U9htv9tfcdHvT8@aws-0-us-west-1.pooler.supabase.com:5432/postgres?schema=public"
DIRECT_URL="postgresql://postgres.dvbqvvgltduwpmkwhlcf:T6U9htv9tfcdHvT8@aws-0-us-west-1.pooler.supabase.com:5432/postgres"
SUPABASE_URL=https://dvbqvvgltduwpmkwhlcf.supabase.co
SUPABASE_KEY=eyJhbGciOiJIUzI1NiIsInR5cCI6IkpXVCJ9.eyJpc3MiOiJzdXBhYmFzZSIsInJlZiI6ImR2YnF2dmdsdGR1d3Bta3dobGNmIiwicm9sZSI6ImFub24iLCJpYXQiOjE3NDA5MzcyMTMsImV4cCI6MjA1NjUxMzIxM30.v3aGxMCUXIaVpXC_9TzTPE_jnnLPNfInhE8UDYFhX14
PORT=8080

# Configuraciones específicas para pruebas
TEST_TIMEOUT=30000 
```

### 3. Repositorio Frontend (UI)
**URL:** https://github.com/Jeferson96/calenconnect-ui.git

Contiene:
- 🎨 Código fuente del frontend (React)
- 🖌️ Componentes de UI
- 🔄 Gestión de estado
- 📱 Interfaces responsivas
- 🧪 Tests de componentes
- 🌐 Configuración de rutas

#### Variables de Entorno Frontend
> **⚠️ Nota**: Credenciales temporales para demostración

Crea un archivo `.env` en la raíz del proyecto:
```bash
VITE_SUPABASE_URL=https://dvbqvvgltduwpmkwhlcf.supabase.co
VITE_SUPABASE_ANON_KEY=eyJhbGciOiJIUzI1NiIsInR5cCI6IkpXVCJ9.eyJpc3MiOiJzdXBhYmFzZSIsInJlZiI6ImR2YnF2dmdsdGR1d3Bta3dobGNmIiwicm9sZSI6ImFub24iLCJpYXQiOjE3NDA5MzcyMTMsImV4cCI6MjA1NjUxMzIxM30.v3aGxMCUXIaVpXC_9TzTPE_jnnLPNfInhE8UDYFhX14
VITE_API_URL=http://localhost:3000
```

> **📅 Importante**: Estas credenciales serán revocadas después de la presentación.

## 🚀 Comenzando

1. Clona los tres repositorios
2. Sigue las guías de instalación en cada repositorio
3. Consulta la documentación completa en el repositorio global

## 📝 Convención de Commits

Seguimos la especificación de Conventional Commits. Ejemplos:
```bash
feat(auth): implementar autenticación JWT
fix(api): corregir validación de fechas
docs(readme): actualizar instrucciones de instalación
```

## 🤝 Contribución

1. Crea un fork del repositorio correspondiente
2. Crea una rama para tu feature (`git checkout -b feature/AmazingFeature`)
3. Realiza tus cambios siguiendo las convenciones de commits
4. Envía un Pull Request

## 📫 Contacto

Jeferson David Camargo Herrera - [GitHub](https://github.com/Jeferson96)
