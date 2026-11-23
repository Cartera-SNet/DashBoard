# Dashboard de Radicación

Aplicación de escritorio para Windows que muestra el estado de radicación de facturas mes a mes: facturado, radicado, pendientes, detalle por usuario y exportación a Excel.

> Este repositorio **solo publica las versiones** del programa. No contiene código ni datos.

## Descarga

1. Entra a la sección **[Releases](../../releases)** (también está a la derecha de esta página).
2. Abre la versión más reciente y descarga **`Dashboard_Radicacion.exe`**.

No necesita instalación ni tener Python.

## Requisitos

- Windows 10 u 11 (con Microsoft Edge WebView2, que ya viene incluido en los equipos al día).
- Acceso al archivo Excel de radicación.

## Primer uso

1. Guarda el archivo en una carpeta donde puedas escribir, por ejemplo **Documentos** o el **Escritorio** (no en *Program Files*).
2. Ábrelo. Si Windows muestra el aviso *"Windows protegió su PC"*, pulsa **Más información** y luego **Ejecutar de todas formas**. Aparece porque el programa no está firmado digitalmente.
3. En **Configuración**, pulsa **Examinar…** y elige el archivo Excel de radicación.
4. Espera unos 30 segundos mientras se lee el archivo la primera vez.

## Actualizaciones

El programa busca versiones nuevas al abrirse y muestra un aviso con las novedades. Pulsa **Actualizar ahora** y se instalará y reiniciará solo. También puedes buscarlas en cualquier momento en **Acerca de → Buscar actualizaciones**.

Tu configuración y la clasificación de usuarios se conservan al actualizar.

## Verificar la descarga (opcional)

Cada versión incluye un archivo `Dashboard_Radicacion.exe.sha256` con la huella digital del programa. Para comprobarla, abre PowerShell en la carpeta de la descarga y ejecuta:

```powershell
(Get-FileHash .\Dashboard_Radicacion.exe -Algorithm SHA256).Hash.ToLower()
```

El resultado debe ser idéntico al contenido del archivo `.sha256`. El programa hace esta comprobación automáticamente antes de instalar una actualización.
