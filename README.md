# eleventa puente de conexión POS

<img src="https://res.cloudinary.com/xadani-mexico/image/upload/v1791611418/assets/proyecto-verificador-precios/bridge-libp2p/images/eleventa-banner-top.png" alt="Banner principal de la integración con eleventa®">

Conecte Verificador de Precios con su punto de venta eleventa® desde la red local.

Instale esta aplicación en el equipo donde está instalado eleventa®.

El puente consulta la información del punto de venta sin interrumpir su operación.

<p align="center">
    <img src="https://res.cloudinary.com/xadani-mexico/image/upload/v1791611099/assets/proyecto-verificador-precios/bridge-libp2p/images/eleventa-arquitectura-lan.png?v=4" width="720" alt="Diagrama de conexión local entre eleventa®, el puente y Verificador de Precios">
</p>

## Antes de comenzar

Confirme lo siguiente antes de instalar:

- Usa Windows 10 o Windows 11.
- Tiene instalado eleventa® MonoCaja o el servidor de eleventa® MultiCaja, versión 4.x o 5.x.
- Instalará el puente en el mismo equipo que eleventa®.
- eleventa® ya generó al menos un respaldo.
- El equipo del puente y el dispositivo que usará Verificador de Precios están conectados a la misma red local.

## Instalación rápida

Complete estos pasos para instalar y conectar el puente.

### 1. Descargar e instalar

1. Descargue la [versión más reciente](https://github.com/verificador-precios/puente-de-conexion-pos-eleventa/releases).
2. Abra el instalador y siga sus indicaciones.
3. Al finalizar, abra **eleventa puente de conexión POS**.

**Resultado esperado:** se abre la ventana principal de la aplicación.

> No se requieren permisos de administrador para instalar la aplicación.

<p align="center">
    <img src="https://res.cloudinary.com/xadani-mexico/image/upload/v1780368340/assets/proyecto-verificador-precios/bridge-libp2p/win-11/windows-11-installer-initial.png?v=4" width="450" alt="Instalador de eleventa puente de conexión POS en Windows">
</p>

### 2. Permitir el acceso en Windows

Cuando Windows indique que **eleventa puente de conexión POS** desea comunicarse en la red, seleccione **Permitir acceso**.

Este permiso permite que Verificador de Precios se comunique con el puente desde la red local.

**Resultado esperado:** la aplicación puede mostrar la **URL para conexión del servidor** cuando termine de conectarse con eleventa®.

<p align="center">
    <img src="https://res.cloudinary.com/xadani-mexico/image/upload/v1780104704/assets/proyecto-verificador-precios/bridge-libp2p/win-11/win-11-firewall-permiso-2.png?v=4" width="420" alt="Permiso de firewall de Windows para eleventa puente de conexión POS">
</p>

### 3. Confirmar la conexión con eleventa®

Al abrirse, el puente busca automáticamente la instalación predeterminada de eleventa® y el respaldo más reciente disponible.

1. Espere a que termine la comprobación inicial.
2. Si la aplicación solicita la carpeta de instalación, confirme que corresponde a la ubicación real de eleventa®.
3. Si no hay respaldos disponibles, genere uno desde eleventa® y vuelva a comprobar la conexión.

**Resultado esperado:** aparece el estado **Conectado al punto de venta** y la **URL para conexión del servidor**.

<p align="center">
    <img src="https://res.cloudinary.com/xadani-mexico/image/upload/v1783470696/assets/proyecto-verificador-precios/bridge-libp2p/eleventa/eleventa-home-server-connection-url.png?v=4" width="520" alt="URL para conexión del servidor mostrada en la aplicación">
</p>

### 4. Emparejar con el Verificador de Precios

Antes de continuar, configure la URL de Verificador de Precios en el **Asistente de URL de acceso**. Esta configuración es necesaria para generar los códigos QR de emparejamiento.

Después, use el **QR de apertura automática** para un emparejamiento rápido o el **QR de emparejamiento manual** cuando necesite completar el proceso manualmente.

**Resultado esperado:** Verificador de Precios se abre y queda emparejado con el punto de venta.

## Emparejar Verificador de Precios

### Configurar la URL de Verificador de Precios

1. En el puente, seleccione **Asistente de URL de acceso**.
2. Escriba únicamente la URL base de su Verificador de Precios. Por ejemplo: `https://ejemplo.verificador-precios.com.mx/`.
3. Revise la vista previa y seleccione **Guardar y usar**.

<p align="center">
  <img src="https://res.cloudinary.com/xadani-mexico/image/upload/v1783470696/assets/proyecto-verificador-precios/bridge-libp2p/eleventa/eleventa-home-access-assistant.png?v=4" width="520" alt="Ejemplo de los botones Copiar y Abrir después de registrar la URL del Verificador de Precios">
</p>

**Resultado esperado:** el puente muestra los códigos QR que puede usar para emparejar Verificador de Precios.

### QR de apertura automática

Use esta opción para abrir Verificador de Precios y completar el emparejamiento automáticamente en el dispositivo donde se utilizará.

1. En el puente, ubique el **QR de apertura automática**.
2. Escanee el código desde el dispositivo donde usará Verificador de Precios.
3. Al escanearlo, el navegador abrirá Verificador de Precios ya emparejado con el punto de venta.

#### Escanear el QR desde cada dispositivo

- En **iPhone** o **iPad**, use **Cámara** o **Escanear código** desde el Centro de control.
- En **Android**, use la cámara del teléfono o Google Lens.
- En **Windows**, use la aplicación **Cámara** con una webcam para escanear el código QR.

### QR de emparejamiento manual

Use esta opción cuando necesite emparejar Verificador de Precios manualmente.

1. En el puente, ubique el **QR de emparejamiento manual** y escanéelo o expórtelo como imagen.
2. En Verificador de Precios, abra **Conexión rápida**.
3. Seleccione el método de lectura que corresponda a su dispositivo y complete el emparejamiento.

En el Verificador de Precios, puede usar cualquiera de estos métodos de emparejamiento:

- **Usar cámara:** escanea el código QR con la cámara del dispositivo.
- **Adjuntar archivo:** permite seleccionar una imagen del código QR.
- **Usar escáner 2D:** permite leer el código con un escáner compatible.

<p align="center">
    <img src="https://res.cloudinary.com/xadani-mexico/image/upload/v1783574765/assets/proyecto-verificador-precios/screenshots/direct-pos-database/eleventa-dc-verificador-precios-prueba-com-mx-config-data-source-5ad70b33bf.jpg?v=4" width="720" alt="Opciones de conexión rápida en Verificador de Precios">
</p>


Si Google Chrome solicita permiso para acceder a la red local, selecciónelo como permitido. Este permiso permite que el sitio web se comunique con el puente instalado en el equipo.

<p align="center">
    <img src="https://res.cloudinary.com/xadani-mexico/image/upload/v1783543092/assets/proyecto-verificador-precios/bridge-libp2p/images/chrome-local-network-access-permission.png?v=4" width="540" alt="Permiso de acceso a la red local solicitado por Google Chrome">
</p>

## Solución de problemas

| Situación | Qué hacer |
| --- | --- |
| Windows bloquea el instalador | En la advertencia, seleccione **Más información** y luego **Ejecutar de todas formas**. También puede hacer clic derecho en el archivo, abrir **Propiedades**, seleccionar **Desbloquear** y aplicar los cambios.<br><br><img src="https://res.cloudinary.com/xadani-mexico/image/upload/v1780033662/assets/proyecto-verificador-precios/bridge-libp2p/win-10/win-10-smartscreen-1.png?v=4" width="320" alt="Advertencia de Windows SmartScreen al abrir el instalador"> |
| No hay conectividad con el punto de venta | Verifique los siguientes puntos:<ol><li>La <strong>Carpeta de instalación</strong> corresponde a eleventa®.</li><li>Existe un respaldo disponible.</li><li>Las credenciales de acceso son correctas.</li><li>Genere un respaldo desde eleventa® y vuelva a comprobar la conexión.</li></ol> |
| El código QR no empareja Verificador de Precios con el punto de venta | Verifique los siguientes puntos:<ol><li>La URL ingresada en el <strong>Asistente de URL de acceso</strong> es correcta.</li><li>El puente está conectado correctamente con el punto de venta.</li><li>Ambos equipos están en la misma red local.</li><li>El navegador tiene permiso para acceder a la red local.</li></ol> |


### Permitir la aplicación después de rechazar el aviso de Windows

1. Abra **Seguridad de Windows**.
2. Entre a **Firewall y protección de red**.
3. Seleccione **Permitir una aplicación a través del firewall**.
4. Busque **eleventa puente de conexión POS** y permita el acceso.
5. Guarde los cambios y vuelva a abrir la aplicación.

<p align="center">
    <img src="https://res.cloudinary.com/xadani-mexico/image/upload/v1780104704/assets/proyecto-verificador-precios/bridge-libp2p/win-11/win-11-firewall-permiso-1.png?v=4" width="520" alt="Configuración del firewall de Windows para permitir eleventa puente de conexión POS">
</p>

## Configuración avanzada

Abra **Configuración de la app** para modificar las opciones siguientes.

### Conexión con eleventa®

La aplicación usa de forma predeterminada estos datos:

| Opción | Valor predeterminado |
| --- | --- |
| Usuario | `SYSDBA` |
| Contraseña | `masterkey` |
| Carpeta de instalación: MonoCaja | `C:\Program Files (x86)\AbarrotesPDV` |
| Carpeta de instalación: MultiCaja | `C:\Program Files (x86)\AbarrotesMultiCaja` |

Cambie la **Carpeta de instalación** si eleventa® está instalado en una ubicación distinta, si la aplicación no encuentra sus archivos o si no identifica la carpeta de respaldos.

> La aplicación obtiene automáticamente las credenciales de acceso de eleventa®.

### Respaldos

Para no interrumpir el funcionamiento del POS eleventa®, el puente consulta una copia restaurada del respaldo más reciente de eleventa®.

- Cuando exista un respaldo nuevo, la aplicación lo restaurará automáticamente al abrirse o al comprobar la conexión.
- Use **Restaurar último respaldo** para ejecutar este proceso manualmente.
- La sección **Información del respaldo en uso** muestra el archivo, la fecha de creación y la última restauración.

<p align="center">
    <img src="https://res.cloudinary.com/xadani-mexico/image/upload/v1783470694/assets/proyecto-verificador-precios/bridge-libp2p/eleventa/eleventa-db-config-form.png?v=5" width="520" alt="Configuración de conexión y respaldo de eleventa puente de conexión POS">
</p>

Si no existen respaldos, genere al menos uno desde eleventa® antes de volver a comprobar la conexión.

### Comportamiento de la aplicación

- **Lanzar aplicación al iniciar:** abre el puente al iniciar sesión en Windows.
- **Confirmar salida de la aplicación:** solicita confirmación antes de cerrar por completo el puente.
- **Recuperar conexión:** intenta recuperar la conexión a la base de datos cuando la aplicación inicia sin que esté disponible o cuando se pierde inesperadamente durante el uso.
- **Tema visual:** cambia la apariencia de la aplicación.
- **Reducir movimiento:** disminuye animaciones y transiciones.
- **Habilitar regeneración de QR:** permite mostrar y regenerar el código QR cuando cambia la URL para conexión del servidor.

Se recomienda mantener habilitada la confirmación de salida para evitar cerrar accidentalmente el puente mientras Verificador de Precios está en uso.

## Actualizaciones

En las versiones instaladas desde los canales oficiales, la aplicación busca actualizaciones automáticamente al iniciarse.

1. Abra la aplicación.
2. Espere aproximadamente 15 segundos.
3. Si existe una actualización, se descargará en segundo plano.
4. Cuando aparezca el aviso **Actualización lista**, seleccione **Actualizar ahora** o cierre la aplicación para iniciar la instalación.

> También puede descargar e instalar manualmente la [versión más reciente](https://github.com/verificador-precios/puente-de-conexion-pos-eleventa/releases).

## Desinstalación

1. Abra **Configuración** de Windows.
2. Entre a **Aplicaciones**.
3. Busque **eleventa puente de conexión POS**.
4. Seleccione **Desinstalar** y siga el asistente.

## Aviso de marcas registradas

eleventa® y sus logotipos son marcas registradas de eleventa.com.
