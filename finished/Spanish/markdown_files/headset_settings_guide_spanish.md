# Configuraciones Recomendadas del Visor Quest VR

## Propósito y Contexto
Esta guía detalla configuraciones recomendadas para Quest 2, Quest 3 y Quest 3s, para hacer la experiencia VR WildXR consistente y confiable.

⚠️ **Meta**: El hardware y software de Meta (incluyendo MQDH) están fuera del control de WPS. Las actualizaciones de Meta pueden causar cambios inesperados en la funcionalidad de los sistemas VR. WPS monitorea los lanzamientos de Meta para informar a los usuarios sobre posibles impactos y cambios.

## Prerrequisitos
- Visor Quest y controladores con baterías

## Resumen Rápido (para usuarios experimentados)
1. Ingresar al menú **Settings**
2. Cambiar configuraciones de energía para coincidir con el caso de uso deseado
3. Habilitar:
    - **Do Not Disturb**
    - **Developer Mode**
    - **Enable MTP connection**
4. Deshabilitar:
    - **Cloud Backup**
    - **Automatic Updates**
    - **Interactive Elements**

## Pasos Detallados

### Accediendo al Menú Settings

1. **Salir de la Aplicación WildXR (si está ejecutándose)**
   - Presionar el **botón Meta-logo** (Quest 3 y Quest 3s) o el **botón Oval Horizontal** (Quest 2) en el controlador de mano derecha
   - Seleccionar **"Quit"** en la ventana de gestión de App que aparece
   - Si la ventana de gestión de App no aparece:
     - Presionar el **botón de encendido del visor** para suspender el visor
     - Presionar el **botón de encendido del visor** nuevamente para despertar el visor
     - Presionar el **botón Meta-logo** en el controlador de mano derecha
     - Seleccionar **"Quit"** en la ventana de gestión de App

2. **Abrir el Menú Quick Settings**
   - Hacer clic en el **botón que muestra hora, fuerza WiFi y nivel de batería** en la Barra de Menú izquierda
   - *Debería aparecer una nueva ventana flotante mostrando Quick Menu Settings*
<div style="page-break-after: always;"></div>

3. **Abrir el Menú Settings**
   - Hacer clic en **"Settings"** en la parte superior derecha de la pantalla Quick Settings Menu
   - *Debería aparecer una nueva ventana flotante mostrando Settings del visor*
   - *Algunas opciones no serán visibles hasta que desplaces la lista izquierda de categorías de configuración*
   - *Los joysticks en cualquier controlador te permitirán desplazarte cuando la retícula de apuntado esté sobre la lista*

### Configuraciones Generales

4. **Configuraciones Software Update**
   - Hacer clic en la pestaña **"Software Update"**
   - Desactivar **todas** las opciones:
     - `Software updates`
     - `Security and Critical updates`
     - `Automatically power headset to update`
     - `Update and backup before shutdown`

5. **Configuraciones Cloud Backup**
   - Hacer clic en la pestaña **"Cloud Backup"**
   - Desactivar `Cloud Backups`

6. **Configuraciones Power**
   - Hacer clic en la pestaña **"Power"**
   - Configurar **"Display Off"** a **4 hours**
   - Configurar **"Auto Sleep Headset"** a **4 hours** *(puede no estar presente en todos los visores)*
   - Desactivar **todas** las opciones bajo **"Battery"**:
     - `Battery Saver`
     - `Low battery audio alert`
     - `Low battery voice alert`

### Configuraciones de Notificación

7. **Configuraciones Notification**
   - Activar `Do Not Disturb`
   - Seleccionar **"Until I turn it off"** de las opciones que aparecen
   - Hacer clic en **"Done"**

### Configuraciones Environment Setup

8. **Configuraciones Interactive Objects**
   - Hacer clic en la pestaña **"Interactive objects"**
   - Desactivar **todas** las opciones:
     - `Avatar Mirror`
     - `First Encounters`
     - `Portal to Meta Horizon World`
<div style="page-break-after: always;"></div>

### Configuraciones Avanzadas

9. **Configuraciones Developer**
   - Activar `Enable Developer Settings`
   - Activar `Enable MTP Notification`
   - Desactivar `Physical Space Features`
   - Desactivar `Link Auto-Connect`

### Siguientes Pasos

10. **Crear PIN de App y bloquear aplicaciones**
    - Seguir la guía **Library Management**

## Entendiendo las Configuraciones Recomendadas del Visor

**Por qué Estas Configuraciones:**
Las configuraciones recomendadas han sido probadas en lugares públicos y proporcionan la experiencia de usuario más consistente y duradera hasta la fecha.

**Configuraciones Software Update**
Desactivar todas las configuraciones de actualización automática previene que un visor esté inesperadamente no disponible durante horas públicas. También permite que las actualizaciones de software sean probadas de manera controlada para prevenir conflictos no anticipados entre WildXR, Auto Launch y software del visor. Meta ha instituido actualizaciones forzadas después de 30 - 45 días de retraso, permitiendo a WPS una ventana para verificar actualizaciones por rendimiento y reaccionar, cuando sea posible, a conflictos de software. Recomendamos revisar visores para actualizaciones pendientes cada 21 días como mantenimiento rutinario y contactar WPS para orientación respecto a instalación.

**Configuraciones Cloud Backup:**
No hay beneficio al Cloud Backup en la mayoría de casos de uso del usuario final donde WildXR se usa en un entorno público o educativo.

**Configuraciones Power**
Configurar **"Display Off"** a **4 hours** permite que visores usados en un entorno público o educativo sean inmediatamente responsivos al uso. Tener la pantalla apagándose prolongará la vida de la batería, pero puede causar que el visor sea lento para responder al uso e influir en la orientación de escenas en WildXR de maneras inesperadas.

**Configuraciones Notification**
Las notificaciones pueden causar interrupción de experiencias de usuario mostrando ventanas emergentes dentro de la aplicación WildXR.

**Configuraciones Interactive Objects**
Un usuario puede encontrarse en la pantalla del menú principal Quest si hay un problema inesperado con el programa Auto Launch o la aplicación WildXR. Usuarios familiarizados con visores VR pueden forzar salida de WildXR en ciertas situaciones para acceder al menú principal Quest. Al ocultar objetos interactivos podemos prevenir algún comportamiento malicioso o simplemente curioso de alterar configuraciones del dispositivo.
<div style="page-break-after: always;"></div>

**Configuraciones Developer**
Desactivar características de espacio físico remueve la necesidad de definir un límite en el visor. La configuración de límites puede interferir con la experiencia del usuario interrumpiendo la visualización WildXR si un usuario se mueve fuera del límite. Los límites también son requeridos para configurarse cada vez que un visor se mueve cualquier distancia y puede causar comportamiento inesperado en algunas situaciones.
Las Notificaciones MTP permiten que el visor sea visto como una unidad cuando se conecta a una computadora vía USB. Esto permite transferencia y manipulación de archivos, necesario en algunas situaciones de solución de problemas.

## Solución de Problemas

**Sección Developer no visible bajo Advanced Settings:**
- Revisar la Guía para habilitar Developer Settings en tu visor
- Asegurar que tu cuenta Meta tenga privilegios de desarrollador habilitados por WPS
- Verificar que el modo desarrollador esté habilitado tanto en la aplicación Meta Horizon del teléfono como en configuraciones del visor

**Los cambios de configuración no persisten:**
- Asegurar que completes cada sección completamente antes de moverte a la siguiente
- Verificar que el visor no esté en un modo restringido o controles parentales
- Verificar que tu cuenta tenga privilegios administrativos en el dispositivo

**No se puede acceder a ciertas opciones de configuración:**
- Confirmar que tu cuenta Meta tenga los permisos necesarios
- Verificar si el visor está inscrito en un sistema de gestión organizacional
- Verificar que la versión de software del visor soporte todas las configuraciones listadas

**Configuraciones de energía causando comportamiento inesperado:**
- Probar diferente temporización de **"Display Off"** si 4 horas causa problemas
- Monitorear vida de batería con configuraciones ajustadas
- Asegurar que el visor permanezca responsivo durante horas pico de uso

## Notas Importantes

⚠️ **Advertencia de Valores Predeterminados**: Los valores predeterminados pueden prolongar vida de batería pero pueden introducir comportamiento inesperado en la aplicación WildXR.

⚠️ **Prerrequisitos de Desarrollador**: Si una sección Developer no es visible bajo Advanced Settings, revisar la Guía para habilitar Developer Settings en tu visor.

⚠️ **Gestión de Actualizaciones**: Meta ha instituido actualizaciones forzadas después de 30-45 días de retraso. Revisar visores para actualizaciones pendientes cada 21 días y contactar WPS para orientación.

⚠️ **Privilegios de Desarrollador Requeridos**: Tu cuenta Meta debe tener acceso de desarrollador otorgado por WPS antes de que modificaciones de configuraciones avanzadas estén disponibles.