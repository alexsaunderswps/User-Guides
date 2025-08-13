# Guía de Configuración de Meta Quest Developer Hub

## Propósito y Contexto
Esta guía establece el Meta Quest Developer Hub (MQDH) en tu computadora, que sirve como la base para gestión avanzada de visores VR. MQDH te permite instalar aplicaciones personalizadas como WPS Auto Launch, gestionar configuraciones de desarrollador y realizar solución avanzada de problemas. Este es un proceso de configuración única que crea el entorno de desarrollo necesario para implementaciones WildXR.

⚠️ **Meta**: El hardware y software de Meta (incluyendo MQDH) están fuera del control de WPS. Las actualizaciones de Meta pueden causar cambios inesperados en la funcionalidad de los sistemas VR. WPS monitorea los lanzamientos de Meta para informar a los usuarios sobre posibles impactos y cambios.

## Prerrequisitos
- Computadora Windows o Mac con acceso a internet
- Credenciales de cuenta Meta para tu configuración VR (incluyendo acceso 2FA)
- Derechos administrativos para instalar software en tu computadora
- Visor Meta Quest con modo desarrollador habilitado
- Cable USB compatible con tu visor Quest
- Visor y computadora conectados a la misma red WiFi

## Resumen Rápido (para usuarios experimentados)
1. Descargar MQDH del sitio de desarrolladores Meta e instalar
2. Lanzar MQDH y autenticarse con cuenta Meta
3. Completar configuración inicial y aceptar términos de desarrollador
4. Conectar visor y establecer autorización de depuración USB
5. Verificar funcionalidad completa con gestión de visor conectado

## Pasos Detallados
*Solo se cubrirán los pasos para el sistema operativo Windows a continuación.*
*Una versión Apple iOS de MQDH está disponible siguiendo el enlace inferior*

### Descargando e Instalando MQDH

1. **Navegar a Descargas de Desarrolladores Meta**
   - Abrir navegador web e ir al sitio de desarrolladores Meta
   - **Windows**: Visitar https://developers.meta.com/horizon/downloads/package/oculus-developer-hub-win/
   - **Mac**: Visitar https://developers.meta.com/horizon/downloads/package/oculus-developer-hub-mac/
<div style="page-break-after: always;"></div>

2. **Descargar paquete MQDH**
   - Hacer clic en el botón "Download" en la esquina superior derecha
   - Aceptar términos de licencia cuando se solicite
   - Elegir ubicación de descarga y hacer clic en "Save"
   - El archivo se descarga como "Meta-Quest-Developer-Hub.zip"

3. **Extraer e instalar MQDH**
   - Navegar a la ubicación del archivo zip descargado
   - Hacer clic derecho en "Meta-Quest-Developer-Hub.zip"
   - Seleccionar "Extract All" y elegir destino (la ubicación predeterminada funciona bien)
   - Hacer clic en "Extract" para desempaquetar archivos
   - Abrir carpeta extraída y localizar "Meta-Quest-Developer-Hub.exe"
   - Hacer doble clic en el ejecutable para comenzar instalación

4. **Completar proceso de instalación**
   - Seguir indicaciones del asistente de instalación
   - Aceptar ubicación de instalación predeterminada a menos que existan requisitos específicos
   - Cuando termine la instalación, marcar casilla "Run MQDH"
   - Hacer clic en "Finish" para completar instalación y lanzar aplicación

### Autenticación Inicial MQDH

5. **Comenzar configuración MQDH**
   - La aplicación se abre a pantalla de bienvenida
   - Hacer clic en "Continue" en la esquina inferior derecha
   - Seleccionar opción "Log in with a Meta account"
   - El sistema abre ventana de navegador para autenticación

6. **Autenticarse con cuenta Meta**
   - El navegador redirige a página de inicio de sesión Meta
   - Elegir opción "Continue with email"
   - Ingresar dirección de Email asociada con tu configuración VR *(puede ser proporcionada por WPS)*
   - Hacer clic en "Next" para proceder

7. **Completar autenticación de contraseña**
   - Seleccionar "Enter password instead" *(más fácil que código de email)*
   - Ingresar tu contraseña de cuenta Meta *(puede ser proporcionada por WPS)*
   - Hacer clic en "Log in" para autenticar
<div style="page-break-after: always;"></div>

8. **Manejar verificación 2FA**
   - El sistema presenta menú desplegable de métodos 2FA
   - Seleccionar método especificado por personal de WPS
   - Hacer clic en "Next" para proceder
   - Ingresar código de autenticación de 6 dígitos cuando se solicite
   - Hacer clic en "Next" para completar verificación 2FA

9. **Gestionar persistencia de inicio de sesión (opcional)**
   - Elegir si guardar credenciales de inicio de sesión en esta computadora
   - *Guardar credenciales solo almacena información de email y contraseña*
   - *La verificación 2FA aún será requerida para futuras sesiones de inicio de sesión*
   - *Considerar implicaciones de seguridad de credenciales guardadas en computadoras compartidas*

### Completando Configuración MQDH

10. **Aceptar términos de desarrollador**
    - MQDH muestra pantalla Terms and Documents
    - Revisar términos del acuerdo de desarrollador
    - Hacer clic en "Continue" para aceptar y proceder

11. **Manejar advertencia de ruta ADB (si aparece)**
    - El sistema puede mostrar advertencia sobre múltiples rutas ADB
    - Esta advertencia típicamente es segura de descartar
    - Hacer clic en "Cancel" o cerrar advertencia sin modificar configuraciones ADB
    - MQDH usará valores predeterminados apropiados para tu sistema

12. **Verificar instalación exitosa**
    - La interfaz principal de MQDH ahora debería ser visible
    - La barra lateral izquierda muestra íconos de gestión de dispositivos
    - La barra de herramientas superior muestra información de cuenta
    - La aplicación está lista para conexiones de visor y gestión de aplicaciones

### Conectando Tu Visor y Estableciendo Depuración USB

13. **Establecer conexión física**
    - Encender tu visor VR completamente
    - Conectar cable USB entre visor y computadora ejecutando MQDH
    - Asegurar que la conexión del cable sea segura en ambos extremos
    - El visor debería permanecer encendido durante todo el proceso de conexión
<div style="page-break-after: always;"></div>

14. **Verificar reconocimiento automático del dispositivo**
    - En MQDH, hacer clic en el ícono del visor en la barra lateral izquierda
    - Buscar tu dispositivo listado como "Active" en la sección Devices
    - Si el dispositivo aparece como Active, proceder directamente al paso 18 para depuración USB
    - Si el dispositivo no se muestra o aparece como inactivo, continuar con configuración del dispositivo

15. **Iniciar configuración de nuevo dispositivo (si es necesario)**
    - Hacer clic en menú desplegable en la esquina superior derecha de MQDH
    - Seleccionar "Set Up New Device" de las opciones del menú
    - Puede que necesites desplazarte hacia abajo para localizar esta opción
    - Hacer clic en "Next" para comenzar asistente de configuración del dispositivo

16. **Configurar conexión del dispositivo**
    - Seleccionar tu modelo específico de visor de las opciones disponibles
    - MQDH escaneará dispositivos compatibles en tu red
    - Elegir tu visor de la lista "Choose Device" cuando aparezca
    - Hacer clic en "Next" para proceder con verificación de cuenta

17. **Completar configuración del dispositivo**
    - Confirmar que se muestre la cuenta Meta correcta en la página Account
    - Hacer clic en "Next" para proceder a configuración de red
    - Seleccionar red WiFi apropiada para tu entorno de implementación
    - Hacer clic en "Next" para continuar con verificación de modo desarrollador
    - Activar interruptor "Enable Developer Mode" si no está ya activo
    - Hacer clic en "Next" para completar configuración inicial del dispositivo

18. **Autorizar acceso de depuración USB**
    - Ponerse el visor VR para ver indicaciones del sistema
    - Buscar cuadro de diálogo "Allow USB debugging?"
    - Este diálogo autoriza a tu computadora a instalar aplicaciones y acceder funciones del sistema
    - Puede que necesites mirar alrededor del entorno virtual para localizar el diálogo

19. **Otorgar permisos permanentes de depuración**
    - Hacer clic en el botón "Always allow from this computer" en el diálogo
    - Este botón puede estar parcialmente oculto en la parte inferior de la ventana del diálogo
    - La opción "Always allow" previene solicitudes repetidas de autorización
    - Quitar visor después de confirmar la autorización
<div style="page-break-after: always;"></div>

20. **Completar verificación de configuración**
    - Regresar a MQDH en tu computadora
    - Hacer clic en "Finish" si el asistente de configuración del dispositivo aún está abierto
    - Tu visor ahora debería aparecer como "Active" en la lista de dispositivos
    - La depuración USB ahora está permanentemente autorizada para este par computadora-visor

## Entendiendo los Componentes del Developer Hub

**Por qué MQDH es Esencial:**
Meta Quest Developer Hub sirve como el puente entre tu computadora y visores VR para tareas avanzadas de gestión. Mientras que la operación básica del visor funciona a través de la aplicación Meta estándar, MQDH desbloquea capacidades de desarrollador que son esenciales para implementación de aplicaciones personalizadas como WPS Auto Launch. Piénsalo como la diferencia entre usar un smartphone como consumidor versus tener acceso de desarrollador para instalar aplicaciones personalizadas y modificar comportamiento del sistema.

**Integración ADB:**
MQDH se integra con Android Debug Bridge (ADB), que es el protocolo de comunicación subyacente para gestionar dispositivos basados en Android. Los visores Meta Quest funcionan en un sistema Android modificado, así que ADB proporciona la base técnica para instalar aplicaciones personalizadas, acceder configuraciones del sistema y realizar solución avanzada de problemas. La advertencia ADB que podrías ver durante la configuración se relaciona con asegurar que MQDH use las rutas de comunicación correctas.

**Requisitos de Cuenta:**
Tu cuenta Meta debe tener privilegios de desarrollador habilitados por WPS antes de que MQDH funcione correctamente. Esto no es algo que puedas habilitar tú mismo - requiere coordinación con personal de WPS que gestiona la configuración de la organización de desarrolladores. Esta medida de seguridad asegura que solo personal autorizado pueda instalar aplicaciones personalizadas en visores de implementación WildXR.

## Solución de Problemas

**La descarga falla o está corrupta:**
- Verificar conexión estable a internet durante toda la descarga
- Intentar descargar desde navegador diferente o modo incógnito
- Verificar espacio disponible en disco antes de descargar
- Contactar WPS si la descarga falla consistentemente

**El proceso de instalación se detiene o falla:**
- Asegurar privilegios administrativos en computadora
- Desactivar temporalmente antivirus durante instalación
- Verificar que el sistema cumpla requisitos mínimos
- Reiniciar computadora y reintentar instalación
<div style="page-break-after: always;"></div>

**La autenticación falla repetidamente:**
- Verificar que la dirección Gmail coincida con la cuenta de configuración VR
- Confirmar precisión de contraseña con personal de WPS
- Verificar que la cuenta tenga privilegios de desarrollador habilitados
- Asegurar que los códigos 2FA sean actuales (expiración de 30 segundos)

**MQDH no se lanza después de la instalación:**
- Verificar cuarentena de Windows Defender o antivirus
- Verificar que la instalación se completó exitosamente
- Intentar ejecutar como administrador
- Reiniciar computadora y reintentar lanzamiento

**Visor no reconocido por MQDH:**
- Verificar que tanto computadora como visor estén conectados a la misma red WiFi
- Confirmar que tu cuenta Meta tenga privilegios de desarrollador a través de WPS
- Verificar que el modo desarrollador esté habilitado tanto en la aplicación Oculus del teléfono como en Settings > Advanced > Developer del visor
- Asegurar que no existan actualizaciones pendientes del visor bajo Settings > General > Software Update

**Autorización de depuración USB no aparece:**
- Verificar que las conexiones del cable USB sean seguras en ambos extremos
- Verificar actualizaciones pendientes del visor que puedan prevenir autorización
- Buscar actualizaciones pendientes de MQDH indicadas por banner en la parte superior de la aplicación
- Intentar desconectar y reconectar cable USB después de 30 segundos
- Reiniciar el visor completamente y reintentar conexión

**El dispositivo aparece conectado pero se muestra como inactivo:**
- Confirmar que la depuración USB fue autorizada correctamente con opción "Always allow"
- Verificar consistencia de cuenta Meta entre MQDH y visor
- Verificar que el modo desarrollador permanezca habilitado en configuraciones del visor
- Intentar remover y re-agregar el dispositivo a través del asistente de configuración MQDH

## Notas Importantes

⚠️ **Privilegios de Desarrollador Requeridos**: Tu cuenta Meta debe tener acceso de desarrollador otorgado por WPS antes de que MQDH funcione correctamente para instalación de aplicaciones personalizadas.

⚠️ **Consistencia de Cuenta**: La cuenta Meta usada en MQDH debe coincidir exactamente con la cuenta asociada con tus visores VR. Cuentas mixtas prevendrán reconocimiento apropiado del dispositivo.

⚠️ **Vinculación del Visor**: MQDH requiere que los visores tengan ADB habilitado para alguna funcionalidad. Si falta funcionalidad, este puede ser el problema.

⚠️ **Actualizaciones de Software**: MQDH está en un estado constante de desarrollo y como tal a menudo requerirá una actualización. Si es posible, siempre actualizar MQDH cuando se solicite antes de completar otras tareas en MQDH.

## Pasos de Verificación

Verificar que tu aplicación MQDH sea capaz de reconocer, conectarse y gestionar visores VR sin pasos de configuración adicionales.

**Verificación de funcionalidad completa:**
- MQDH se lanza sin errores y muestra información de cuenta correctamente
- Al menos un visor aparece como "Active" en la lista de dispositivos
- La autorización de depuración USB ha sido otorgada y confirmada
- Los íconos de gestión de dispositivos son accesibles y responsivos en la barra lateral izquierda
- Puedes acceder al sistema de archivos del visor y características de gestión de aplicaciones