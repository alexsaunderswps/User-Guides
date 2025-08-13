# Guía de Configuración del Visor Quest VR

## Propósito y Contexto
Esta guía proporciona los pasos requeridos para configurar un visor Quest VR por primera vez. 
WPS puede haber creado algunas cuentas necesarias como parte de su programa interno de socios VR. Consultar con personal de WPS si no estás seguro de qué cuentas necesita tu organización.
La creación de cuentas por WPS se hace para facilitar operación fluida de VR y aumenta nuestra capacidad de proporcionar soporte técnico. 
Las cuentas creadas sin la ayuda del personal de WPS no pueden ser accedidas por el personal de WPS durante sesiones de soporte técnico.

⚠️ **Meta**: El hardware y software de Meta (incluyendo MQDH) están fuera del control de WPS. Las actualizaciones de Meta pueden causar cambios inesperados en la funcionalidad de los sistemas VR. WPS monitorea los lanzamientos de Meta para informar a los usuarios sobre posibles impactos y cambios.

## Prerrequisitos
- Una conexión a internet WiFi
- Credenciales de cuenta de email asociadas con tu configuración VR *(pueden ser proporcionadas por WPS)*
- Smartphone con capacidad de aplicación 2FA
- Smartphone con aplicación Meta Horizon instalada
- Coordinación inicial con personal de WPS para primer inicio de sesión
- Visores VR

## Resumen Rápido (para usuarios experimentados)
1. Se crea cuenta Meta para Organización *(puede ser proporcionada por WPS)*
2. El usuario inicia sesión en aplicación Meta Horizon del teléfono
3. Se habilita modo desarrollador para visor
4. Se aplican configuraciones recomendadas al visor
5. Se instalan WildXR y Auto Launch *(si se desea)* en visor
6. El visor se registra con el Sitio Web WildXR para aprovisionamiento remoto
7. Los videos se descargan o cargan lateralmente para mejorar rendimiento WildXR 

## Pasos Detallados

### Creación de Cuenta Meta

- *Si el personal de WPS creó la Cuenta Meta usada para registrar visores, este paso puede estar completo*

1. **Navegar a Meta**
   - Abrir navegador web e ir a `meta.com`
<div style="page-break-after: always;"></div>

2. **Acceder al inicio de sesión**
   - Hacer clic en el **ícono de Cuenta** *(silueta de persona)* en la parte superior derecha
   - Seleccionar **"Sign up or log into a Meta account"**
   - Elegir **"Continue with email"**

3. **Ingresar credenciales**
   - Hacer clic en **Continue with Email**
   - Ingresar dirección de Email asociada con tu configuración VR
   - Hacer clic en **"Next"**
   - Elegir **"Create new account"**
   - Ingresar los detalles solicitados según sea necesario para creación de cuenta
   - *Al agregar fecha de nacimiento - WildXR se recomienda para edades 13+ - ingresar una fecha que satisfaga este requisito*
   - Elegir una contraseña para tu cuenta *(el personal de WPS no tendrá acceso a tu contraseña)*
   - Asegurar los detalles de tu cuenta (email y contraseña) para uso futuro
   - Hacer clic en **"Next"**

4. **Gestionar persistencia de inicio de sesión (opcional)**
   - Elegir si guardar credenciales de inicio de sesión en esta computadora
   - *Guardar credenciales solo almacena información de email y contraseña*
   - *Considerar implicaciones de seguridad de credenciales guardadas en computadoras compartidas*

5. **Verificar detalles de cuenta** 
   - Revisar los detalles de cuenta según se ingresaron
   - *Desmarcar la casilla de recibir emails de marketing*
   - Hacer clic en **"Create account"**

6. **Confirmar creación de cuenta**
   - Abrir la cuenta de email asociada con tu cuenta Meta
   - Copiar el código de confirmación del email reciente de Meta
   - Ingresar el código de confirmación en la casilla apropiada.
   - Hacer clic en **"Next"**

7. **Acceder al panel de cuenta**
   - Regresarás a la página principal de `meta.com`
   - Hacer clic en el **ícono de Cuenta** nuevamente para acceder a características de cuenta *(El ícono ahora es un círculo con una letra o Logo)*
   - Seleccionar **"Accounts Center"** para el panel principal
<div style="page-break-after: always;"></div>

### Autenticación de Dos Factores

- *Ahora es un buen momento para configurar autorización de dos factores ya que será necesaria más tarde*
- *Si tu cuenta fue aprovisionada por personal de WPS, este paso puede haber sido completado*

8. **Navegar a configuraciones de seguridad**
   - En **Accounts Center**, hacer clic en **"Password and security"**
   - Seleccionar **"Two-factor authentication"**
   - Elegir tu perfil
   - Seleccionar **"Authentication app"** y continuar al paso 9 *(recomendado)*
   - Seleccionar **"SMS or WhatsApp"** y continuar al paso 13

### 2FA vía Aplicación de Autenticación

9. **Instalar aplicación autenticadora (Recomendado)**
   - Una aplicación autenticadora permite gestión por múltiples personas
   - Descargar Google Authenticator (recomendado) o Authy
   - Disponible tanto en iOS como Android
   - Múltiples miembros del personal pueden usar el mismo autenticador para cuenta compartida
   - La autenticación SMS o WhatsApp está disponible solo para un número de teléfono

10. **Agregar nuevo dispositivo**
    - Hacer clic en el botón **"Add"**
    - *Aparecerán código QR y clave de configuración*
    - *Cambiar a tu teléfono para los siguientes pasos*

11. **Configurar aplicación autenticadora**
    - Abrir aplicación autenticadora en teléfono
    - Agregar nueva cuenta *(ícono +)*
    - Elegir **"Scan QR code"** o **"Enter setup key"**
    - Escanear código QR del sitio web Meta

12. **Completar configuración**
    - Ingresar nombre descriptivo para este dispositivo *(ej WPSVR GAuth o GAuth de Alex)*
    - Ingresar código de 6 dígitos de la aplicación autenticadora
    - Hacer clic en **"Done"**
    - *El dispositivo ahora aparece en la lista de dispositivos 2FA*
<div style="page-break-after: always;"></div>

### 2FA vía SMS o WhatsApp

- *Solo se permite un número de teléfono para 2FA vía SMS o WhatsApp*
- *Esto restringirá la capacidad de solucionar ciertos problemas si surgen*

13. **Agregar Número de Teléfono**
    - Cambiar código de País si es necesario *(por defecto Estados Unidos)*
    - Ingresar Número de Teléfono
    - Hacer clic en **"Next"**
    - Ingresar el código de 6 dígitos enviado al dispositivo
    - Hacer clic en **"Done"**

### Aprovisionamiento de aplicación Meta Horizon

14. **Abrir la aplicación Meta Horizon del teléfono**
    - Elegir **Continue with email**
    - Ingresar el email usado para crear la cuenta Meta de la Organización *(Puede ser proporcionado por WPS)*
    - Hacer clic en **"Next"**
    - Elegir **"Enter password instead"** *(más fácil que código de email)*
    - Ingresar tu contraseña de cuenta Meta *(puede ser proporcionada por WPS)*

15. **Verificar cuenta vía 2FA *(puede ser requerido)***
    - Seleccionar método 2FA del menú desplegable
    - Hacer clic en **"Next"**
    - Abrir aplicación autenticadora o buscar mensaje SMS/WhatsApp
    - Ingresar código de 6 dígitos
    - Hacer clic en **"Next"**

16. **Gestionar persistencia de inicio de sesión (opcional)**
    - Elegir si guardar credenciales de inicio de sesión en esta computadora
    - *Guardar credenciales solo almacena información de email y contraseña*
    - *Considerar implicaciones de seguridad de credenciales guardadas en computadoras compartidas*
  
### Configurar cuenta Meta Horizon

- *La cuenta Meta Horizon se usa exclusivamente para el espacio VR de Meta*
- *Algunas opciones serán visibles para otros usuarios Meta Horizon*

17. **Elegir un nombre de usuario Meta Horizon**
    - *Este nombre de usuario será visible para otros usuarios Meta Horizon*
    - Ingresar un nombre de usuario aceptado *(una marca verde indicará que el nombre de usuario es válido)*
    - Hacer clic en **"Continue"**
    - Serás llevado al panel Meta Horizon
<div style="page-break-after: always;"></div>

### Configuración del visor

18. **Encender visor**
    - Remover el material de empaque del visor
    - Remover ahorradores de batería de los controladores de mano
    - **Quest 2**: Presionar **botón de encendido** en el lado derecho
    - **Quest 3 & Quest 3s**: Presionar **botón de encendido** en el lado izquierdo
    - Ponerse el visor VR

19. **Introducción inicial y conectar a WiFi**
    - Seguir las indicaciones en pantalla en el Visor VR
    - *Ocasionalmente los controladores de mano instalarán una actualización que los vuelve inoperables por un período breve*
    - Conectar tu visor a tu conexión de internet WiFi
    - *WPS recomienda ingresar los detalles WiFi en tu visor*
    - *Si tu red WiFi está oculta ir al Paso #20*
    - Tu visor puede aplicar actualizaciones de firmware
    - Deja tu visor conectado mientras se descargan actualizaciones
    - *Tu visor puede indicar que puedes continuar configuración en la aplicación Meta Horizon del teléfono*
    - ⚠️ **WPS no recomienda que lo hagas y sugiere esperar hasta que el visor muestre tu código de emparejamiento**

### Agregar una red WiFi oculta

20. **Agregar una red oculta a WiFi**
    - *Puedes necesitar asistencia de tu departamento de TI de la empresa si tienes un programa robusto de seguridad WiFi*
    - En la ventana WiFi desplazarse hacia abajo a **"+ New Network >"**
    - Hacer clic para agregar una nueva red
    - Hacer clic en **"Advanced"**
    - Bajo **"Hidden Network"** cambiar valor mostrado a **"Yes"**
    - Generalmente los valores predeterminados para el resto del menú Advanced serán suficientes
    - *Si continúas teniendo problemas conectándote a una red WiFi oculta puedes necesitar contactar tu departamento de TI de la empresa*
    - Hacer clic en **"Confirm"**
    - Si tu red WiFi tiene contraseña, muy probablemente usa **WPA/WPA2-Personal** como configuración de **"Security"**
    - Ingresar los detalles restantes de tu red WiFi
    - Hacer clic en **"Connect"** para terminar configuración WiFi y conectarse a la red
<div style="page-break-after: always;"></div>

### Emparejar visor con aplicación Meta Horizon del teléfono

21. **Navegar a Devices en aplicación Horizon**
    - Abrir tu aplicación Meta Horizon del teléfono
    - La aplicación Meta Horizon mostrará el avatar de la cuenta y un menú hamburguesa *(tres barras horizontales)* en el lado derecho.
    - Abrir el menú hamburguesa
    - Bajo **Device Management** hacer clic en **Devices**

22. **Emparejar visor con aplicación Meta Horizon**
    - Encontrar la opción **Pair New Headset** y hacer clic en ella
    - Seleccionar el modelo correcto de visor Meta
    - *Puedes ser solicitado a crear un avatar - este paso ahora es requerido por Meta*
    - *Este avatar es visible para otros usuarios Meta Horizon*
    - Crear un avatar y hacer clic en **"Continue"**
    - Tu visor debería estar mostrando un código de cinco dígitos
    - Ingresar el código de cinco dígitos cuando se solicite
    - Hacer clic en **"Continue"** cuando se muestre la pantalla de emparejamiento exitoso

### **Aceptar condiciones de Meta**

23. **Aceptar descargos de responsabilidad en aplicación Meta Horizon**
    - Hacer clic en **"Continue"** en las pautas de seguridad
    - Hacer clic en **"Don't Share"** o **"Share"** en la solicitud de compartir datos adicionales
    - Hacer clic en **"Not now"** en la solicitud Enable hand and body tracking
    - Hacer clic en **"Skip"** en la oferta Start 3-month trial *(Esta pantalla puede o no estar presente)*
    - Hacer clic en **"Skip"** en Add a payment method
    - Hacer clic en **"Close"** en la pantalla **You're all set!**

### **Terminar configuración del visor**

24. **Terminar introducción del Visor**
    - Ponerse el visor VR para una breve introducción a tu visor de Meta
    - Seguir indicaciones en pantalla
    - Participar en tutoriales según se desee *(Saltar tutoriales no afecta configuración del visor)*
    - *Debes mantener el visor puesto durante la introducción*
    - Después de la introducción se te mostrará el panel Horizon

## Siguientes Pasos

**Habilitar Modo Desarrollador**
- Seguir la guía **Developer Mode Setup**
- El modo desarrollador es necesario para aplicar algunas configuraciones recomendadas
- El modo desarrollador es necesario para remover el límite de seguridad requerido
<div style="page-break-after: always;"></div>

**Aplicar Configuraciones Recomendadas del Visor**
- Seguir la guía **Recommended Headset Settings**

**Remover Software Innecesario**
- Seguir la guía **Library Management**

## Solución de Problemas

**No se puede acceder a cuenta Meta:**
- Verificar que la dirección de Email sea correcta para tu configuración VR *(Si es proporcionada por WPS)*
- Contactar WPS para asistencia con contraseña

**Código de confirmación de Meta ausente:**
- Los códigos de confirmación pueden retrasarse por conexiones de internet lentas o intermitentes
- Revisar la carpeta **Spam** en tu navegador de email
- Asegurar que estés buscando en la cuenta de email correcta *(la cuenta puede haber sido proporcionada por WPS)*

**Ya existen dispositivos 2FA para cuenta Meta**
- Si tu cuenta Meta fue creada por personal de WPS estará prepoblada con 2 - 3 dispositivos 2FA
- Uno de estos dispositivos debería corresponder a la cuenta de email aprovisionada por WPS
- Otros dispositivos 2FA serán usados por Personal de WPS para asistir en solución de problemas si surgen problemas

**Botón "Add" deshabilitado para 2FA:**
- La cuenta puede tener el máximo de dispositivos vinculados
- Contactar WPS para remover dispositivos no utilizados
- Algunos tipos de cuenta tienen límites de dispositivos

**No se puede encontrar aplicación Meta Horizon:**
- La aplicación Meta Horizon está disponible para descarga en Apple App store o Google Play store
- Si estás usando un teléfono suministrado por WPS la aplicación debería estar presente - buscar Horizon
- La aplicación Meta Horizon puede no estar colocada en la primera página de tu teléfono
- Usar la función de búsqueda del teléfono para encontrar Meta Horizon y moverla a una ubicación obvia

**No se puede iniciar sesión en la aplicación Meta Horizon**
- Asegurar que estés usando la misma cuenta que fue usada en los pasos de Creación de Cuenta Meta
- Asegurar que hayas seleccionado "Enter Password instead" si estás intentando ingresar una contraseña
- Verificar tu contraseña, será la contraseña de Cuenta Meta, no la contraseña de cuenta de email para inicio de sesión Horizon
<div style="page-break-after: always;"></div>

**2FA falla para la aplicación Meta Horizon**
- Asegurar que estés usando la cuenta 2FA correcta para autorización
- Si estás usando SMS/WhatsApp para autorización solo un número de teléfono está asociado con la cuenta
- Los códigos 2FA son válidos por 30 segundos en promedio, esperar hasta que se genere un nuevo código e intentar iniciar sesión

**Meta no permite mi nombre de usuario deseado**
- Meta restringe el formato de nombres de usuario para forzar unicidad.
- Editar el nombre de usuario para incluir guiones bajos o números
- Recordar que este nombre de usuario puede volverse visible para otros usuarios Meta Horizon

**El visor no reconoce controladores de mano**
- En el arranque inicial de un visor pueden aplicarse actualizaciones de firmware a controladores de mano que los vuelven temporalmente no funcionales
- Esperar 2 - 3 minutos antes de intentar usar controladores de mano nuevamente
- Insertar baterías frescas en los controladores de mano
- Muy raramente puede haber otros problemas con controladores de mano - Programar una sesión de ayuda con Personal de WPS para orientación adicional

**Visor no puede conectarse a WiFi**
- Asegurar que tu departamento de TI permita que dispositivos no reconocidos se conecten al canal WiFi de tu empresa
- Registrar el dispositivo VR con tu departamento de TI si es necesario
- Asegurar que tengas la red WiFi y contraseña correctas ingresadas en los campos apropiados
- Si tu red WiFi está oculta, ir al Paso #20 - *Puedes necesitar asistencia de tu departamento de TI con redes ocultas*

**No se puede encontrar menú Devices en la Aplicación Horizon**
- Asegurar que estés en la página principal de la aplicación Meta Horizon - *Deberías ver tu avatar de usuario y nombre*
- Cerrar la Aplicación Horizon y reabrir la aplicación para cargar la página principal
- Identificar el menú hamburguesa en el lado derecho de la aplicación - el ícono son tres barras horizontales apiladas
- Abrir el menú hamburguesa y desplazarse hacia abajo para ver la sección **"Device management"**
- Verificar si hay actualizaciones pendientes para la aplicación Meta Horizon o el sistema operativo de tu teléfono
<div style="page-break-after: always;"></div>

**Forzado a crear un Avatar**
- Meta ahora fuerza a los usuarios a crear un Avatar para su usuario
- Si has deshabilitado o bloqueado la mayoría de redes sociales este avatar será mínimamente visible para otros usuarios
- Si quieres verificar tu configuración de privacidad, abrir el menú hamburguesa y desplazarse hacia abajo a **"Privacy and security"** para abrir la sección **"Privacy settings"**

**Código de emparejamiento de 5 dígitos no aceptado**
- Puede tomar un tiempo para que el emparejamiento del visor se complete dependiendo de la conectividad a internet
- Asegurar que tu teléfono y visor estén en la misma red WiFi
- Verificar el código mostrado en el visor y según se ingresó en la aplicación Meta Horizon

## Notas Importantes

⚠️ **Aplicación Meta Horizon**: Meta requiere el uso de la aplicación de teléfono **Meta Horizon** para configurar visores Quest.

⚠️ **Creación de Avatar**: Meta requiere la creación de un avatar virtual. Este avatar es visible en algunas ubicaciones a través del "metaverso" VR dependiendo de configuraciones de privacidad.

⚠️ **Dificultad con 2FA**: Cuando Meta pide un método 2FA puede haber múltiples opciones presentadas. Solo un número de teléfono puede ser usado para alertas SMS/WhatsApp para autenticación. Asegurar que estés seleccionando la cuenta correcta para 2FA. Los códigos 2FA generalmente duran 30 segundos, si un código está por expirar, esperar a que se genere uno nuevo.

⚠️ **Redes de internet**: Si tu visor y teléfono no están conectados a la misma red WiFi puede no ser posible emparejar tu visor con la aplicación.