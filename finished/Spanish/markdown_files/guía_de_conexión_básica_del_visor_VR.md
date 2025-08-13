# Guía de Conexión Básica del Visor VR

## Propósito y Contexto
Esta guía establece la base para todas las tareas de gestión de archivos del visor VR. Conectarás tu Meta Quest 2, Quest 3 o Quest 3s a una computadora y accederás a los archivos de la aplicación WildXR. Esta conexión es requerida antes de transferir archivos multimedia, confirmar archivos de configuración o localConfiguration, o solucionar problemas de aplicaciones.

⚠️ **Meta**: El hardware y software de Meta (incluyendo MQDH) están fuera del control de WPS. Las actualizaciones de Meta pueden causar cambios inesperados en la funcionalidad de los sistemas VR. WPS monitorea los lanzamientos de Meta para informar a los usuarios sobre posibles impactos y cambios.

## Prerrequisitos
- Visor VR Meta Quest 2, Quest 3 o Quest 3s
- Cable USB-C *(recomendado)* o cable USB-C a USB-A
- Computadora con File Explorer *(Windows)* o Finder *(Mac)*
- Baterías AA para controladores
- Aplicación WildXR instalada en visor
- Configuraciones de desarrollador habilitadas en el visor

## Resumen Rápido (para usuarios experimentados)
1. Encender visor y asegurar que los controladores tengan baterías
2. Conectar cable USB y salir de WildXR si está ejecutándose
3. Habilitar conexión USB a través de notificaciones Quest
4. Navegar a: `Quest` > `Internal shared storage` > `Android` > `data` > `com.wps.wildx` > `files`

## Pasos Detallados

### Configuración Inicial

1. **Instalar baterías del controlador**
   - Tanto Quest 2 como Quest 3 usan **baterías AA**
   - Asegurar que ambos controladores estén encendidos

2. **Encender tu visor**
   - **Quest 2**: Presionar **botón de encendido** en el lado derecho
   - **Quest 3 & Quest 3s**: Presionar **botón de encendido** en el lado izquierdo

3. **Conectar cable USB**
   - **Quest 2**: Puerto USB ubicado en lado izquierdo bajo la sien
   - **Quest 3 & Quest 3s**: Puerto USB ubicado en lado izquierdo en la sien
<div style="page-break-after: always;"></div>

4. **Identificar controlador primario**
   - **Quest 2**: El controlador derecho tiene **botón oval horizontal**
   - **Quest 3 & Quest 3s**: El controlador derecho tiene **botón logo Meta**

### Saliendo de la Aplicación WildXR

*Si WildXR se lanza automáticamente, debes salir de ella para acceder a archivos.*

5. **Intentar abrir menú del sistema**
   - Ponerse el visor
   - Presionar y soltar el **botón oval/Meta** en controlador derecho
   - Si aparece pantalla **Quit/Resume**, saltar al paso 8

6. **Forzar aparición del menú (si es necesario)**
   - Presionar **botón de encendido** para suspender visor *(la pantalla se oscurece)*
   - Presionar **botón de encendido** nuevamente para despertar visor
   - Intentar **botón oval/Meta** nuevamente
   - Repetir hasta que aparezca pantalla **Quit/Resume**

7. **Salir de WildXR**
   - Seleccionar **"Quit"** usando gatillo del controlador
   - *Deberías ver el entorno de inicio Quest*

### Habilitando Acceso de Computadora

8. **Abrir notificaciones**
   - Apuntar punto de targeting al **ícono de campana** en la barra de menú
   - Presionar **gatillo del controlador** *(bajo dedo índice)* para abrir notificaciones

9. **Habilitar conexión USB**
   - *Necesitarás haber habilitado configuraciones de desarrollador en el visor*
   - Encontrar notificación **"USB Detected"**
   - Apuntar a la notificación y presionar **gatillo del controlador**
   - *Esto permite que la computadora reconozca el visor como unidad externa*

### Accediendo Archivos en Computadora

10. **Abrir explorador de archivos**
    - **Windows**: Abrir **File Explorer**, hacer clic en **"This PC"**
    - **Mac**: Abrir **Finder**

11. **Navegar al visor**
    - Hacer doble clic en **"Quest 2"**, **"Quest 3"** o **Quest 3s**
    - Hacer doble clic en **"Internal shared storage"**
<div style="page-break-after: always;"></div>

12. **Navegar a archivos WildXR**
    - Hacer doble clic en **"Android"**
    - Hacer doble clic en **"data"**
    - Hacer doble clic en **"com.wps.wildx"**
    - Hacer doble clic en **"files"**

*Ahora tienes acceso a archivos y carpetas WildXR.*

## Entendiendo archivos y carpetas WildXR

**Carpeta downloads**
- Contiene todos los videos descargados para la aplicación WildXR
- Archivos nombrados usando id de 36 caracteres universalmente único (UUID)
- Todos en formato MP4
- *Esta carpeta es donde se colocarán archivos de video **cargados lateralmente***

**Carpeta textures**
- Contiene todas las imágenes en miniatura descargadas para la aplicación WildXR
- Archivos nombrados con UUID que coincide con UUID del video
- Todos en formato PNG

**Carpeta temp**
- Contiene archivos temporales necesarios por la aplicación WildXR
- A menudo contendrá archivos de video que están siendo descargados por la aplicación WildXR

**Carpeta Unity**
- Archivos Unity de WildXR
- No se necesita acceso por la mayoría de usuarios

**Archivo localConfiguration.json**
- Configuraciones que son específicas del dispositivo (visor)
- Contiene configuraciones de Device ID, Environment y OfflineMode

**Archivo configuration.json**
- Configuraciones que controlan la apariencia de la aplicación WildXR
- Si el visor o computadora (dispositivo) está registrado a través del Portal Web WildXR, estas configuraciones se controlan remotamente
- Si el visor o computadora (dispositivo) no está registrado a través del Portal Web WildXR, estas configuraciones están preconfiguradas por la aplicación WildXR

**metadataDatabase.json**
- Metadatos requeridos por la aplicación WildXR para funcionamiento apropiado
<div style="page-break-after: always;"></div>

**DownloadQueue.json**
- Información para función de descarga de video en la aplicación WildXR
- Puede estar vacío o ausente si no hay videos en cola para descarga

**Player.log y Player-prev.log**
- Archivos de registro que registran el comportamiento más reciente y previo de la aplicación WildXR
- Importantes para diagnosticar problemas y pueden ser solicitados por personal de WPS para diagnóstico

**youtubeData.json**
- Datos usados para ordenar videos en galerías de miniaturas basados en varios factores

## Solución de Problemas

**Visor no aparece en explorador de archivos:**
- Asegurar que el cable USB esté completamente conectado
- Intentar un puerto USB diferente en la computadora
- Verificar que habilitaste la conexión USB en el paso 9
- Verificar que el cable USB soporte transferencia de datos, no solo carga

**No se puede salir de WildXR:**
- Quitar visor brevemente, luego volver a ponérselo
- Reiniciar visor *Presionar botón de encendido para suspender visor y luego presionar nuevamente para despertar*
- Asegurar que los controladores tengan suficiente energía de batería

**Controladores no responden:**
- Verificar dirección de instalación de batería
- Intentar baterías AA frescas
- Asegurar que los controladores estén emparejados *(debería suceder automáticamente cuando el visor inicia)*
- Reiniciar controladores removiendo y reinsertando baterías

**Notificación de conexión USB no aparece:**
- Desconectar y reconectar cable USB
- Intentar puerto USB diferente en computadora
- Asegurar que el visor esté completamente encendido y no en modo de suspensión
- Verificar si el modo desarrollador está habilitado en configuraciones del visor
- *Debes aceptar la notificación de conexión USB cada vez que se conecte el USB*
<div style="page-break-after: always;"></div>

**Archivos/carpetas aparecen vacíos o inaccesibles:**
- Verificar que WildXR haya sido ejecutado al menos una vez en el visor
- Verificar que se esté siguiendo la ruta correcta: `Android` > `data` > `com.wps.wildx` > `files`
- Asegurar que se otorgaron permisos de depuración USB si se solicitaron
- Intentar refrescar la vista del explorador de archivos

## Notas Importantes

⚠️ **Restricción de Edición de Archivos**: Archivos como `configuration.json` no pueden editarse directamente en el visor. Debes:
1. Copiar archivos a tu computadora
2. Editarlos ahí
3. Copiar los archivos modificados de vuelta para sobrescribir originales
4. Los archivos pueden abrirse para verificar que los cambios han sido aplicados *(ver **Verificación de Transferencia de Archivos** abajo)*

⚠️ **Recomendación de Respaldo**: Siempre crear una copia de respaldo de archivos de configuración antes de editar.

⚠️ **Verificación de Edición de Archivos**: Siempre verificar que los archivos editados han sido transferidos exitosamente al visor.

⚠️ **Recomendación de Transferencia de Archivos**: Cuando cargues lateralmente archivos de video, verificar que la carpeta **downloads** contenga el número de videos que intentaste cargar lateralmente.

⚠️ **Requisitos de Cable**: Asegurar que tu cable USB soporte transferencia de datos. Algunos cables son solo para carga y no permitirán acceso a archivos.

⚠️ **Prerrequisitos WildXR**: WildXR debe estar instalado y ejecutado al menos una vez antes de que los archivos sean accesibles en la estructura de directorio esperada.