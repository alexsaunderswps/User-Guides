# Guía de Revinculación de Cuenta Meta del Visor VR

## Propósito y Contexto
Esta guía aborda el proceso de reconectar un visor VR a su cuenta Meta asociada cuando el enlace se ha roto o perdido. La revinculación de cuenta se vuelve necesaria cuando los visores pierden su conexión a los servidores de autenticación de Meta, lo cual puede ocurrir después de períodos prolongados sin conexión, actualizaciones del sistema o cambios de seguridad de la cuenta.

⚠️ **Meta**: El hardware y software de Meta (incluyendo MQDH) están fuera del control de WPS. Las actualizaciones de Meta pueden causar cambios inesperados en la funcionalidad de los sistemas VR. WPS monitorea los lanzamientos de Meta para informar a los usuarios sobre posibles impactos y cambios.

## Prerrequisitos
- Conexión estable a internet para computadora y visor VR
- Credenciales de cuenta de email asociadas con tu configuración VR *(pueden ser proporcionadas por WPS)*
- Contraseña de cuenta Meta *(puede ser proporcionada por WPS)*
- **Si has completado "Guía de Configuración de Acceso y Seguridad de Cuenta Meta":**
  - Smartphone con aplicación autenticadora 2FA configurada
  - Acceso a tu dispositivo de autenticación previamente configurado
- **Si NO has completado "Guía de Configuración de Acceso y Seguridad de Cuenta Meta":**
  - Coordinación inmediata con personal de WPS para provisión de código 2FA en tiempo real
  - Tiempo programado con soporte WPS para proceso de autenticación guiado

## Resumen Rápido (para usuarios experimentados)
1. Navegar a `meta.com/device` y autenticarse con credenciales de cuenta Meta
2. Completar verificación 2FA usando tu dispositivo configurado o código proporcionado por WPS
3. Ingresar el código de verificación de ocho caracteres mostrado en la interfaz del visor VR
4. Confirmar revinculación exitosa y probar características dependientes de la cuenta

## Pasos Detallados

### Accediendo a la Interfaz de Gestión de Dispositivos de Meta

1. **Navegar al portal de gestión de dispositivos**
   - Abrir navegador web e ir directamente a `meta.com/device`
   - *Esta URL especializada te lleva directamente a la interfaz de gestión de dispositivos de Meta*
   - *Evitar usar el sitio general meta.com ya que requiere pasos de navegación adicionales*

2. **Iniciar autenticación de cuenta**
   - Seleccionar **"Continue with email"** de las opciones de inicio de sesión disponibles
   - *Este método proporciona la ruta de autenticación más confiable para tareas de gestión de cuenta*
<div style="page-break-after: always;"></div>

3. **Completar autenticación primaria**
   - Ingresar la dirección de Email asociada con tu configuración VR
   - Hacer clic en **"Next"** para proceder a la verificación de contraseña
   - Elegir **"Enter password instead"** *(más fácil que código de email)*
   - Ingresar tu contraseña de cuenta Meta *(puede ser proporcionada por WPS)*
   - Hacer clic en **"Log in"** para proceder a la autenticación de dos factores

### Completando Autenticación de Dos Factores

4. **Manejar verificación 2FA**
   - El sistema presenta menú desplegable para métodos 2FA disponibles
   - Seleccionar el método que has configurado previamente o según indicación del personal de WPS
   - Hacer clic en **"Next"** para proceder a la entrada de código
   - Ingresar el código de autenticación de seis dígitos de tu aplicación autenticadora
   - *Si no has configurado 2FA personal, usar el código proporcionado por el personal de WPS durante tu sesión de soporte programada*
   - Hacer clic en **"Next"** para completar autenticación

5. **Gestionar persistencia de inicio de sesión (opcional)**
   - Elegir si guardar credenciales de inicio de sesión en esta computadora
   - *Guardar credenciales solo almacena información de email y contraseña*
   - *La verificación 2FA aún será requerida para futuras sesiones de inicio de sesión*
   - *Considerar implicaciones de seguridad de credenciales guardadas en computadoras compartidas*

6. **Localizar código de verificación del visor**
   - Ponerse el visor VR o revisar su pantalla
   - *Si se necesita un código de revinculación, generalmente no se mostrará nada más en el visor*
   - *Este código es único para esta sesión y expira después de un período de tiempo razonable*
   - *Anotar el código cuidadosamente ya que es sensible a mayúsculas y debe ingresarse exactamente*

7. **Ingresar código de verificación**
   - Regresar a la interfaz de gestión de dispositivos Meta en tu computadora
   - Confirmar que se muestre la información correcta de cuenta Meta
   - Ingresar el código de ocho caracteres de tu visor en el campo designado
   - *Verificar cada carácter antes de proceder ya que entrada incorrecta requiere empezar de nuevo*
   - Hacer clic en **"Continue"** para iniciar el proceso de revinculación

8. **Verificar conexión exitosa**
   - El sistema debería mostrar confirmación de que tu dispositivo ha sido reconectado
   - El visor debería mostrar información actualizada del estado de la cuenta
   - Las características de cuenta Meta deberían estar disponibles inmediatamente en la interfaz del visor
<div style="page-break-after: always;"></div>

## Solución de Problemas

**La autenticación falla repetidamente:**
- Verificar que la dirección Gmail coincida con la cuenta de configuración VR
- Confirmar precisión de contraseña con personal de WPS
- Verificar que la cuenta tenga privilegios de desarrollador habilitados
- Asegurar que los códigos 2FA sean actuales (expiración de 30 segundos)

**Código de ocho caracteres no aceptado por interfaz Meta:**
- Verificar que las cuentas Meta de web y visor coincidan
- Confirmar que el código de ocho dígitos fue ingresado correctamente
- Reiniciar visor para refrescar código

**La revinculación parece exitosa pero las características de cuenta permanecen no disponibles:**
- Permitir tiempo para que la cuenta se revincule
- Reiniciar el visor

## Notas Importantes

⚠️ **Coordinación de Contraseña**: Nunca intentar cambiar contraseñas de cuenta Meta independientemente. Siempre coordinar modificaciones de contraseña con personal de WPS para prevenir bloqueos de soporte técnico y asegurar que todos los sistemas relacionados reciban las actualizaciones necesarias.

⚠️ **Consistencia de Cuenta**: La cuenta Meta usada para revinculación debe coincidir exactamente con la cuenta originalmente configurada en el visor. Usar cuentas diferentes, incluso si pertenecen a la misma organización, creará problemas de acceso persistentes.

⚠️ **Tiempo de Seguridad**: Los códigos 2FA son sensibles al tiempo. Los códigos 2FA expiran cada 30 segundos.