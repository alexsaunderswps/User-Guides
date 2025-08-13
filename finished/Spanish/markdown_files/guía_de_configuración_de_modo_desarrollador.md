# Guía de Configuración de Modo Desarrollador

## Propósito y Contexto
Esta guía proporciona los pasos requeridos para autorizar una cuenta Meta y visores asociados con esa cuenta con credenciales de desarrollador. 
Las credenciales de desarrollador son requeridas para habilitar ciertas características que son necesarias para resolver problemas de conexión, gestionar configuraciones del dispositivo o solucionar problemas de aplicaciones VR.

⚠️ **Meta**: El hardware y software de Meta (incluyendo MQDH) están fuera del control de WPS. Las actualizaciones de Meta pueden causar cambios inesperados en la funcionalidad de los sistemas VR. WPS monitorea los lanzamientos de Meta para informar a los usuarios sobre posibles impactos y cambios.

## Prerrequisitos
- Una conexión a internet
- Credenciales de cuenta de email asociadas con tu configuración VR *(pueden ser proporcionadas por WPS)*
- Contraseña de cuenta Meta *(puede ser proporcionada por WPS)*
- Smartphone con capacidad de aplicación 2FA
- Smartphone con aplicación Meta Horizon instalada
- Coordinación inicial con personal de WPS para primer inicio de sesión
- Visores VR

## Resumen Rápido (para usuarios experimentados)
1. La Cuenta Meta de la organización es agregada al grupo de Desarrolladores WPS
2. Modo Desarrollador activado para cada dispositivo en la aplicación Meta Horizon
3. Modo Desarrollador activado en cada visor vía Configuración Avanzada

## Pasos Detallados

### Autorización Inicial de Desarrollador

1. **Solicitar al personal de WPS agregar la Cuenta Meta de tu Organización al grupo de Desarrolladores WPS**
   - *Si el personal de WPS creó la Cuenta Meta usada para registrar visores, este paso puede estar completo*
   - *Los siguientes pasos se completan mejor durante una videollamada*
   - Enviar al personal de WPS información de cuenta Meta (**Dirección de Email** o **Nombre de Usuario**) solicitando acceso de Desarrollador
   - El personal de WPS invitará la cuenta a unirse a la organización como Desarrollador
   - Revisar email para invitación a Meta Quest Developer Dashboard de Meta Horizons
<div style="page-break-after: always;"></div>

2. **Aceptar invitación para unirse al grupo de Desarrolladores WPS**
   - Abrir email de invitación
   - Hacer clic en **"View Invitation"** - se abrirá un enlace web - *(Recomendamos usar navegadores Chrome o Firefox para este paso)*

3. **Ingresar credenciales**
   - Hacer clic en **Continue with Email**
   - Ingresar dirección de Email asociada con tu configuración VR
   - Hacer clic en **"Next"**
   - Elegir **"Enter password instead"** *(más fácil que código de email)*
   - Ingresar tu contraseña de cuenta Meta *(puede ser proporcionada por WPS)*
   - Hacer clic en **"Log in"**

4. **Autorización de dos factores (puede ser requerida)**
   - *Si no has habilitado autorización de dos factores (2FA) para tu cuenta Meta necesitarás hacerlo ahora*
   - *Ver la Guía de Configuración de Acceso y Seguridad de Cuenta Meta para detalles sobre habilitar 2FA*
   - *Si tu cuenta fue creada por personal de WPS necesitarás coordinar acceso*

5. **Aceptar invitación y verificar autorización** 
   - Aceptar invitación en el sitio web Meta
   - *Una casilla "accept invitation" debería ser visible en la página web*
   - Confirmar con personal de WPS que la invitación ha sido aceptada y las credenciales de Desarrollador han sido autorizadas

### Conectar Visor a la aplicación Meta Horizon del teléfono

6. **Encender visor VR**
   - *Los siguientes pasos asumen que el visor VR ha sido configurado inicialmente*
   - *Si este no es el caso - ver **Guía de Configuración Inicial del Visor VR** para pasos requeridos*
   - Conectar visor VR a internet
   - *Es mejor tener solo un visor encendido a la vez*

7. **Abrir Opciones del Dispositivo**
   - Abrir la aplicación Meta Horizon del teléfono
   - *La cuenta usada para el visor VR debe ser la misma usada para la cuenta Meta Horizon*
   - La aplicación Meta Horizon mostrará el avatar de la cuenta y un menú hamburguesa *(tres barras horizontales)* en el lado derecho.
   - Abrir el menú hamburguesa
   - Bajo **Device Management** hacer clic en **Devices**
<div style="page-break-after: always;"></div>

8. **Conectar al dispositivo**
   - *Puedes ver múltiples dispositivos listados* 
   - Un dispositivo debería mostrar un círculo verde y estar listado como **"Nearby"**
   - Hacer clic en el dispositivo **Nearby**
   - Una nueva pantalla muestra detalles del dispositivo y cuatro opciones **Manage your device**

9. **Activar Modo Desarrollador**
    - Hacer clic en **Headset Settings** - *(puede estar oculto por notificación Manage profiles)*
    - Deberías ver varias opciones bajo **Headset settings**
    - Hacer clic en **Developer Mode**
    - Activar el interruptor **Developer Mode**

### Habilitar configuraciones de desarrollador en el visor VR

- *Estarás usando el visor VR para los siguientes pasos*
- *Para instrucciones detalladas sobre acceder al menú Settings ver - **Configuraciones Recomendadas del Visor***

10. **Abrir el menú Advanced Settings**
    - Abrir el menú **Quick Settings** haciendo clic en la pantalla de hora/WiFi/batería
    - Hacer clic en **Settings** en la parte superior derecha
    - En la izquierda, desplazarse hacia abajo para encontrar **Advanced Settings**
    - Hacer clic en la opción **Advanced Setting**

11. **Activar Modo Desarrollador**
    - Desplazarse hacia abajo para encontrar la sección **Developer**
    - Activar **Enable Developer Settings**
    - Debería aparecer una lista adicional de opciones
    - Activar **Enable MTP Notifcation**
    - Desactivar **Physical Link Features**
    - Desactivar **Link Auto-Connect**

## Solución de Problemas

**No se recibió Email de Invitación de WPS**
- Coordinar con personal de WPS antes de enviar email de seguimiento
- Verificar la dirección de Email enviada al personal de WPS
- Revisar tu carpeta de spam

**Incapaz de iniciar sesión en cuenta Meta**
- Verificar el Email correcto para la cuenta Meta
- Al iniciar sesión, usar código de email en lugar de contraseña para confirmar coincidencia de cuenta
- Asegurar que la contraseña sea correcta para la cuenta 
- Si la cuenta Meta fue creada por WPS, coordinar más solución de problemas con el personal

**Problemas de autorización de dos factores**
- Si la cuenta fue creada por WPS, coordinar o recibir acceso 2FA *(usualmente Google Authenticator)*
- Asegurar que estés eligiendo el método correcto para 2FA *(si existen múltiples opciones)*
- El personal de WPS no podrá asistir con 2FA vía teléfono o SMS

**Incapaz de aceptar invitación para unirse a la Organización**
- Asegurar que la cuenta Meta coincida con la dirección de Email en la invitación
- Intentar aceptar invitación usando navegadores Chrome o Firefox - *(Safari ha causado problemas en el pasado)*

**Incapaz de encontrar Dispositivo en aplicación Meta Horizon**
- Asegurar que tanto el visor VR como el teléfono estén usando la misma fuente de internet
- Verificar que el visor VR y el teléfono estén conectados con la misma cuenta Meta
- Reiniciar tanto el visor como la aplicación Meta Horizon
- Para reducir posible confusión, asegurar que solo un visor VR esté encendido

**Múltiples Dispositivos se muestran como **Nearby** en aplicación Meta Horizon**
- Apagar otros Dispositivos cercanos para simplificar configuración
- Coincidir números de serie *(número de serie se encuentra en la sien izquierda del visor)*
- *Número de serie está en el interior de la sien izquierda - Quest 3*
- *Número de serie está en el exterior de la sien izquierda, bajo la cubierta de la correa - Quest 2*

**Modo Desarrollador no disponible en aplicación Meta Horizon**
- Asegurar que la cuenta Meta haya sido agregada a la Organización WPS como desarrollador
- Cerrar sesión de la aplicación Meta Horizon y volver a iniciar sesión
- Verificar que se esté usando la cuenta Meta correcta en la aplicación Meta Horizon

**El interruptor de Modo Desarrollador no se mantiene activado en aplicación Meta Horizon**
- Verificar que la cuenta Meta haya sido agregada a la Organización WPS como desarrollador
- Asegurar que se esté usando la cuenta Meta correcta en la aplicación Meta Horizon
- Revisar el visor VR para diálogo de advertencia o mensajes de acción

**Configuraciones de Desarrollador no se ven en Advanced Settings en el visor**
- Verificar que el visor haya tenido el Modo Desarrollador activado en la aplicación Meta Horizon
- Reiniciar visor VR
- Revisar visor para actualizaciones pendientes - *(aplicar cualquier actualización pendiente)*

## Notas Importantes

⚠️ **Invitación de Organización WPS**: Se requiere coordinación de este paso antes de cualquier otra configuración de cuenta de Desarrollador

⚠️ **Consistencia de Cuenta**: Las cuentas Meta deben coincidir entre la aplicación Meta Horizon y el visor VR.