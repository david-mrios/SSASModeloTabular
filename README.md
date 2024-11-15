# Implementación de un Modelo Tabular en SSAS Tabular
## Prerrequisitos

- Tener instalada una instancia de **SSAS Tabular** en modo de compatibilidad tabular. En este caso, se utilizará la dirección de instancia: `localhost/SSASTABULAR`.
- Tener acceso al archivo de respaldo de la base de datos (`.bak`) que se restaurará en SSAS Tabular.

## Configuración y Pasos de Implementación

### 1. Conexión al Workspace en el Modelo Tabular

1. En el entorno de desarrollo, configurar el **Workspace** en el modelo tabular.
   - Configurar la propiedad **Integrated Workspace Mode** como `True`.
   - Establecer el **Workspace Server** en `localhost:50616` (u otro puerto disponible en la máquina local).
   
   Esta configuración permite que el entorno de trabajo esté integrado y sea administrado en el servidor local de desarrollo.

### 2. Procesar las Tablas

1. Luego de restaurar la base de datos, es necesario procesar las tablas para actualizar la información y prepararlas para el despliegue desde el proyecto en visual studio.

### 3. Desplegar el Modelo Tabular

1. Una vez procesadas las tablas, proceder a desplegar el modelo.
2. Configurar el **Deployment Server** a `localhost/SSASTABULAR`.
3. Realizar el despliegue desde el entorno de desarrollo, asegurándose de que el modelo sea accesible desde la instancia configurada.
4. Verificar que el modelo esté desplegado y accesible, y que los datos se puedan consultar correctamente.
