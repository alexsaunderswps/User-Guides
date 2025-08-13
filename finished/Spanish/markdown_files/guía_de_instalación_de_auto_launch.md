# Guía de Instalación de WildXR Auto Launch

## Propósito y Contexto
Esta guía instala la aplicación WPS Auto Launch que automáticamente inicia WildXR cuando el visor se enciende. Auto Launch elimina la necesidad de controladores manuales en instalaciones públicas, crea una experiencia de usuario fluida y permite el monitoreo remoto del tiempo de actividad del visor. Este proceso transforma un visor VR estándar en un sistema tipo quiosco que requiere mínima interacción del usuario para comenzar la experiencia de conservación.

⚠️ **Meta**: El hardware y software de Meta (incluyendo MQDH) están fuera del control de WPS. Las actualizaciones de Meta pueden causar cambios inesperados en la funcionalidad de los sistemas VR. WPS monitorea los lanzamientos de Meta para informar a los usuarios sobre posibles impactos y cambios.

## Prerrequisitos
- Meta Quest Developer Hub completamente instalado y configurado con al menos un visor conectado y depuración USB autorizada *(ver Guía de Configuración MQDH)*
- Visor VR con modo desarrollador habilitado tanto en la aplicación Oculus como en la configuración del visor
- Aplicación WildXR ya instalada y ejecutada exitosamente al menos una vez en el visor objetivo
- Archivo `autolaunchping_v.1.0.0.apk` *(proporcionado por WPS)*
- Cuenta Meta con privilegios de desarrollador habilitados por WPS
- Cable USB para conectar el visor durante la instalación

## Resumen Rápido (para usuarios experimentados)
1. Conectar visor objetivo a la computadora *(o verificar conexión MQDH existente)*
2. Acceder a la gestión de aplicaciones MQDH e instalar APK `autolaunchping`
3. Lanzar aplicación Auto Launch y configurar integración WildXR
4. Probar funcionalidad de inicio automático

## Pasos Detallados

### Preparando para la Instalación de Auto Launch

1. **Conectar visor para transferencia de archivos**
   - Lanzar **Meta Quest Developer Hub**
   - Encender Quest Headset
   - Conectar Headset a la Computadora con cable USB

2. **Verificar conexión del visor**
   - Asegurar que tu visor objetivo aparezca como **"Active"** en la lista de dispositivos MQDH
   - *Los nuevos visores típicamente requerirán el mismo proceso de autorización de depuración USB completado durante la configuración MQDH (ver Guía de Configuración MQDH)*
   - Confirmar que el visor no muestre indicadores de error o problemas de conectividad
<div style="page-break-after: always;"></div>

3. **Confirmar preparación de WildXR**
   - Verificar que WildXR esté instalado en el visor objetivo
   - Asegurar que WildXR haya sido lanzado exitosamente al menos una vez
   - *Auto Launch no puede registrar aplicaciones que nunca han funcionado en el sistema*
   - Probar inicio de WildXR manualmente si hay incertidumbre sobre su estado operacional

### Instalando la Aplicación Auto Launch

4. **Acceder a gestión de aplicaciones**
   - En MQDH, hacer clic en el **ícono de carpeta** en la barra lateral izquierda
   - *Esto abre la interfaz de gestión de archivos y aplicaciones*
   - Bajo la sección **"On Device"**, hacer clic en el ícono de carpeta **"Apps"**
   - *Esto muestra las aplicaciones actualmente instaladas en tu visor*

5. **Agregar la aplicación Auto Launch**
   - Hacer clic en el botón **"Add Build"** en la esquina superior derecha
   - *Se abre el explorador de archivos para localizar tu archivo APK de instalación*
   - Navegar a la ubicación donde guardaste `autolaunchping_v.1.0.0.apk`
   - Seleccionar el archivo APK y hacer clic en **"Open"**

6. **Monitorear progreso de instalación**
   - MQDH muestra indicadores de progreso de instalación
   - Permitir que el archivo se instale completamente antes de proceder
   - *La instalación típicamente toma 30-60 segundos dependiendo del rendimiento del sistema*
   - Deberías ver `com.wps.autowildxrping` aparecer en tu lista de aplicaciones cuando esté completo

### Configurando la Integración Auto Launch

7. **Lanzar aplicación Auto Launch**
   - Localizar `com.wps.autowildxrping` en tu lista de aplicaciones MQDH
   - Hacer clic en el **ícono de menú de tres puntos** a la derecha del nombre de la aplicación
   - Seleccionar **"Launch App"** del menú desplegable
   - Ponerse el visor VR para completar la configuración

8. **Completar configuración Auto Launch**
   - WildXR puede lanzarse inmediatamente si Auto Launch detecta configuración existente
   - Si WildXR se lanza automáticamente, quitar el visor y reiniciar para probar funcionalidad
   - Si ves una ventana **"WildXRAutoPing"** en su lugar, continúa con configuración manual
   - *Buscar un icono que se parezca a un alienígena o ícono inusual en la barra de menú Quest si la ventana no es inmediatamente visible*
<div style="page-break-after: always;"></div>

9. **Finalizar configuración**
   - En la ventana **WildXRAutoPing**, hacer clic en el botón **"Save URL"**
   - *Esto crea el enlace permanente entre Auto Launch y WildXR*
   - WildXR debería lanzarse inmediatamente después de hacer clic en **Save URL**
   - Quitar visor y reiniciar el dispositivo para verificar funcionalidad de inicio automático

## Entendiendo el Propósito de la Tecnología Auto Launch

Antes de comenzar la instalación, ayuda entender qué logra Auto Launch y por qué requiere este proceso de instalación especializado. Las aplicaciones VR tradicionales requieren que los usuarios naveguen manualmente los menús y seleccionen aplicaciones usando controladores. Esto funciona bien para uso personal pero crea barreras en entornos públicos de conservación donde los visitantes pueden no estar familiarizados con interfaces VR o donde los controladores pueden perderse o dañarse.

La aplicación WPS Auto Launch opera a nivel del sistema Android, registrándose para activarse cuando el visor completa su secuencia de inicio. Piénsalo como configurar un navegador web predeterminado en tu computadora, excepto que en lugar de manejar enlaces web, Auto Launch maneja el evento de inicio del visor. Cuando el sistema arranca, Auto Launch inmediatamente señala a WildXR para comenzar, creando una transición fluida desde el encendido hasta el contenido de conservación.

Esta integración a nivel del sistema es por qué la instalación requiere Meta Quest Developer Hub en lugar de métodos estándar de instalación de aplicaciones. Esencialmente estamos modificando el comportamiento del visor a un nivel más profundo del que las aplicaciones normales acceden.

## Solución de Problemas

**MQDH no muestra dispositivos conectados:**
- Verificar que completaste la configuración completa de MQDH incluyendo autorización de depuración USB
- Verificar que tu visor objetivo sea el mismo configurado durante la configuración MQDH
- Si usas un visor diferente, necesitará el mismo proceso de autorización de depuración USB
- Asegurar que el visor permanezca encendido y conectado durante toda la instalación

**Falla la instalación de Auto Launch:**
- Confirmar que WildXR esté correctamente instalado y haya sido ejecutado exitosamente al menos una vez
- Verificar que el visor tenga suficiente espacio de almacenamiento para aplicaciones adicionales
- Verificar que `com.wps.autowildxrping` aparezca en la lista de aplicaciones MQDH antes de proceder con la configuración
- Asegurar que el archivo APK `autolaunchping` no esté corrupto probando instalación en un visor diferente
<div style="page-break-after: always;"></div>

**La funcionalidad Auto Launch no funciona después de la instalación:**
- Verificar que `com.wps.autowildxrping` aparezca como en ejecución en el menú de tres puntos MQDH
- Confirmar que WildXR se lance manualmente para asegurar integridad de la aplicación
- Probar reinicio completo en lugar de suspender/despertar para verificar comportamiento de inicio
- Verificar que **"Save URL"** fue clickeado durante la configuración y que WildXR se lanzó después

**Ventana WildXRAutoPing no visible:**
- Buscar un ícono inusual o similar a alienígena en la barra de menú Quest
- Intentar quitar y volver a ponerse el visor para refrescar la interfaz
- Asegurar que la aplicación Auto Launch fue realmente lanzada desde MQDH en lugar de solo instalada
- Verificar que WildXR haya sido ejecutado al menos una vez antes de la configuración Auto Launch

## Notas Importantes

⚠️ **Requisitos de Cuenta de Desarrollador**: Tu cuenta Meta debe tener estatus de desarrollador verificado con Wildlife Protection Solutions antes de que cualquier instalación de aplicación personalizada tenga éxito.

⚠️ **Compatibilidad del Sistema**: Auto Launch requiere visores con modo desarrollador correctamente habilitado tanto en la aplicación móvil Oculus como en la configuración interna del visor bajo **Advanced > Developer**.

⚠️ **Coincidencia de Cuenta**: La cuenta Meta usada para MQDH debe coincidir exactamente con la cuenta usada para configurar el visor. Cuentas que no coincidan prevendrán el reconocimiento del dispositivo y la instalación de aplicaciones.

⚠️ **Prerrequisitos WildXR**: WildXR debe estar exitosamente instalado y lanzado al menos una vez antes de la instalación Auto Launch. Auto Launch no puede registrar una aplicación que el sistema no reconoce.

## Verificación y Pruebas

Después de completar la instalación, verificar la funcionalidad Auto Launch a través de pruebas comprensivas. Apagar el visor completamente usando el botón de encendido, esperar 30 segundos, luego encender nuevamente. Auto Launch debería activar el inicio de WildXR sin ninguna intervención manual o uso de controlador. Si aún se requiere navegación manual, el proceso de registro no fue completado exitosamente y debería repetirse desde el paso 5.