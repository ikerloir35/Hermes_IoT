# Hermes IoT - Sensorización del Jardín Botánico de Barcelona

## Resumen del Proyecto

### Propósito

Este proyecto implementa una infraestructura IoT para la monitorización del área del estanque del Jardín Botánico de Barcelona. Proporciona visualización y seguimiento en tiempo real de datos de sensores a través de una aplicación móvil.

### Stack Tecnológico

- **Lenguaje**: Kotlin
- **Plataforma**: Android
- **Arquitectura**: MVVM con Clean Architecture
- **Tecnologías Principales**:
  - Jetpack Compose para UI
  - Dagger Hilt para inyección de dependencias
  - Retrofit para comunicación API
  - MQTT para datos de sensores en tiempo real
  - Docker para containerización
  - Kotlin Coroutines para operaciones asíncronas

### Características

- ## **Autenticación**:

  - Sistema de autenticación de usuarios
  - Gestión segura de sesiones
  - Control de acceso basado en roles

- ## **Características del Sistema**:

  - Monitorización de datos de sensores en tiempo real
  - Visualización de datos históricos
  - Alertas y notificaciones personalizables
  - Panel de control interactivo

- ## **Interfaz de Usuario**:

  - Diseño Material Design 3 moderno
  - Diseño responsivo
  - Soporte para tema claro/oscuro
  - Navegación intuitiva

- ## **Características Técnicas**:
  - Almacenamiento en caché offline
  - Sincronización de datos en segundo plano
  - Actualizaciones en tiempo real vía MQTT
  - Integración con API RESTful

### Seguridad

- ## **Seguridad de Autenticación**:

  - Autenticación basada en tokens seguros
  - Transmisión de datos encriptada
  - Gestión de sesiones

- ## **Seguridad de Datos**:

  - Encriptación de extremo a extremo
  - Almacenamiento seguro de datos
  - Actualizaciones regulares de seguridad

- ## **Mejores Prácticas**:
  - Ofuscación de código
  - Gestión segura de claves API
  - Auditorías regulares de seguridad

### Co-Desarrolladores

- **Desarrollador Principal**:
  - Iker López Iribas
  - Damià Belles Sampera
  - Daniel Boj

## Configuración del Entorno

### Prerrequisitos

- Android Studio Hedgehog o más reciente
- Docker Desktop
- Git
- JDK 17 o más reciente
- Android SDK 34

### Claves API Requeridas

1. **Google API Key**
   - Requerida para integración con Maps
   - Colocar en archivo local.properties

### Instrucciones de Configuración

1. **Clonar el Repositorio**

   ```bash
   git clone https://github.com/ikerloir35/Hermes_IoT.git
   cd Hermes_IoT
   ```

2. **Configuración del Entorno**

   - Copiar `local.properties.example` a `local.properties`
   - Añadir tus claves API y configuración

3. **Configuración de Compilación**

   - Abrir proyecto en Android Studio
   - Sincronizar archivos Gradle
   - Compilar proyecto

4. **Ejecutar la Aplicación**
   - Iniciar contenedores Docker:
     ```bash
     cd docker-iot-api-server && docker compose up
     cd ../docker-iot-broker && docker compose up
     ```
   - Ejecutar app en emulador Android o dispositivo físico

### Mejores Prácticas de Seguridad

1. **Gestión de Claves API**

   - Almacenar claves en local.properties
   - Nunca subir claves al control de versiones
   - Usar variables de entorno en producción

2. **Seguridad del Código**

   - Actualizaciones regulares de dependencias
   - Firma de código
   - Configuración de ProGuard

3. **Flujo de Desarrollo**
   - Flujo de ramas feature
   - Proceso de revisión de código
   - Pruebas automatizadas

### Solución de Problemas

1. **Problemas de Compilación**

   - Limpiar y recompilar proyecto
   - Actualizar dependencias Gradle
   - Verificar versiones SDK

2. **Problemas en Tiempo de Ejecución**

   - Verificar estado de contenedores Docker
   - Comprobar endpoints API
   - Monitorear logcat para errores

3. **Problemas de Autenticación**
   - Verificar claves API
   - Comprobar conectividad de red
   - Validar credenciales

### Despliegue en Producción

1. **Lista de Verificación Pre-despliegue**

   - Actualizar números de versión
   - Ejecutar escaneo de seguridad
   - Probar en múltiples dispositivos

2. **Proceso de Lanzamiento**

   - Generar APK firmado
   - Actualizar documentación
   - Desplegar en Play Store

3. **Post-despliegue**
   - Monitorear reportes de errores
   - Recopilar feedback de usuarios
   - Planificar actualizaciones

## Licencia

Este proyecto está licenciado bajo la Licencia Creative Commons - ver el archivo LICENSE para más detalles.
