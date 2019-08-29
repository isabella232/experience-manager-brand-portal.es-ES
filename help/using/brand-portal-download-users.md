---
title: Descargar recursos
seo-title: Descargar recursos
description: Todos los usuarios pueden descargar simultáneamente varios recursos y carpetas accesibles para ellos. De esta forma, los recursos de marca aprobados pueden distribuirse de forma segura para uso sin conexión.
seo-description: Todos los usuarios pueden descargar simultáneamente varios recursos y carpetas accesibles para ellos. De esta forma, los recursos de marca aprobados pueden distribuirse de forma segura para uso sin conexión.
uuid: 4 b 57118 e-a 76 e -4 d 8 a -992 a-cb 3 c 3097 bc 03
content-type: referencia
products: SG_ EXPERIENCEMANAGER/Brand_ Portal
topic-tags: descarga de descarga
discoiquuid: f 90 c 2214-beea -4695-9102-8 b 952 bc 9 fd 17
translation-type: tm+mt
source-git-commit: 32c3cdb8e3fafd74cfb36e6bcfe0811e7152b2d0

---


# Descargar recursos {#download-assets}

Todos los usuarios pueden descargar simultáneamente varios recursos y carpetas accesibles para [!DNL Brand Portal]ellos. De esta forma, los recursos de marca aprobados pueden distribuirse de forma segura para uso sin conexión. Obtenga información sobre cómo descargar los recursos aprobados y [!DNL Brand Portal]qué esperar del rendimiento [de descarga](../using/brand-portal-download-users.md#main-pars-header).

>[!NOTE]
>
>Solo los administradores pueden descargar recursos caducados. Para obtener más información sobre los recursos caducados, consulte [Administrar derechos digitales de recursos](../using/manage-digital-rights-of-assets.md).

## Pasos para descargar recursos {#steps-to-download-assets}

Para descargar recursos o carpetas que contengan recursos, [!DNL Brand Portal]siga estos pasos:

1. Desde [!DNL Brand Portal] la interfaz, realice una de las siguientes acciones:

   * Seleccione las carpetas o los recursos que desee descargar. En la barra de herramientas de la parte superior, haga clic en el icono **Descargar** .
   ![](assets/downloadassets-1.png)

   * Para descargar una sola carpeta o recurso, coloque el puntero sobre la carpeta o el recurso. En las miniaturas de acción rápida disponibles, haga clic en el icono **Descargar** .
   ![](assets/downloadsingleasset-1.png)

   >[!NOTE]
   >
   >Si los recursos que descarga también incluyen recursos con licencia, se le redirigirá a la página **Administración** de copyright. En esta página, seleccione los recursos, haga clic **en Aceptar** y, a continuación, haga clic **en Descargar**. Si decide rechazar, los recursos con licencia no se descargarán.\
   >Los recursos protegidos por licencia tienen [un acuerdo de licencia asociado](https://helpx.adobe.com/experience-manager/6-5/assets/using/drm.html#DigitalRightsManagementinAssets) a ellos, que se realiza estableciendo la propiedad [de metadatos del recurso](https://helpx.adobe.com/experience-manager/6-5/assets/using/drm.html#DigitalRightsManagementinAssets) en [!DNL AEM] Assets.

   ![](assets/licensed-asset-download-1.png)

   El cuadro **de** diálogo Descargar aparece con la opción **Recurso** seleccionada de forma predeterminada.

   ![](assets/donload-assets-dialog-1.png)

   >[!NOTE]
   >
   >Si los recursos que está descargando son archivos de imagen y selecciona solo la opción **Recurso** en el cuadro de diálogo Descargar, pero no [está autorizado por el administrador para tener acceso a las representaciones originales de archivos](../using/brand-portal-adding-users.md#main-pars-procedure-202029708) de imagen, entonces no se descargan archivos de imagen y aparecerá Aviso, lo que indica que el administrador ha restringido el acceso a las representaciones originales.

   ![](assets/restrictaccess-note.png)

2. Para descargar las representaciones de recursos además de los recursos, seleccione **Representaciones**. Sin embargo, para permitir que las representaciones generadas automáticamente se descarguen junto con representaciones personalizadas, anule la selección **de Excluir representaciones generadas automáticamente**, que se seleccionan de forma predeterminada.

   ![](assets/exclude-auto-renditions.png)

   Para descargar solo las representaciones, anule la selección **de Recursos**.

   >[!NOTE]
   >
   >De forma predeterminada, solo se descargan los recursos. Sin embargo, las representaciones originales de archivos de imagen no se descargan si el administrador no [tiene autorización para acceder a las representaciones originales de archivos de imagen](../using/brand-portal-adding-users.md#main-pars-procedure-202029708).

   * Para acelerar la descarga de archivos de recursos, [!DNL Brand Portal]seleccione **Activar la opción de aceleración** de descarga y [siga el asistente](../using/accelerated-download.md#main-pars-header-405749062). Para obtener más información sobre la descarga más rápida de recursos, consulte [Guía para acelerar las descargas desde [! DNL Brand Portal]](../using/accelerated-download.md).

   * Para aplicar un [ajuste preestablecido de imagen personalizado al recurso y sus representaciones](../using/brand-portal-image-presets.md#applyimagepresetswhendownloadingimages), seleccione **Representación dinámica**. Especifique las propiedades preestablecidas de la imagen (tamaño, formato, espacio de color, resolución y modificador de imagen) para aplicar el ajuste preestablecido de imagen personalizado al descargar el recurso y sus representaciones. Para descargar solo las representaciones dinámicas, haga clic en **Recurso (s)**.
   ![](assets/dynamic-renditions.png)

   >[!NOTE]
   >
   >Para obtener una vista previa (o descargar) representaciones dinámicas de cualquier recurso, asegúrese de que el Dynamic Media está habilitado y de que la representación [!UICONTROL Pyramid Tiff] del recurso exista en la instancia [!DNL AEM] del autor, desde donde se han publicado los recursos. Cuando se publica un recurso, [!DNL Brand Portal]también [!UICONTROL se publica su] representación tiff Pyramid. No hay manera de generar [!UICONTROL la representación tiff] Pyramid desde [!DNL Brand Portal].

   * Para conservar la jerarquía [!DNL Brand Portal] de carpetas al descargar recursos, seleccione **Crear carpeta independiente para cada recurso**. De forma predeterminada, se omite la jerarquía [!DNL Brand Portal] de carpetas y todos los recursos se descargan en una carpeta del sistema local.

   * Para enviar una notificación por correo electrónico a los usuarios con un vínculo para descargar los recursos, seleccione **Correo electrónico**.
   ![](assets/download-link.png)

   >[!NOTE]
   >
   >El vínculo de descarga por correo electrónico caduca después de 45 días.
   >
   >Los administradores pueden personalizar los mensajes de correo electrónico, es decir, el logotipo, la descripción y el pie de página, mediante la función [de marca](../using/brand-portal-branding.md) .

3. Haga clic **en Descargar**.

   Los recursos (y las representaciones si se seleccionan) se descargan como un archivo ZIP en la carpeta local. Sin embargo, no se crea ningún archivo zip si se descarga un único recurso sin ninguna de las representaciones, lo que asegura una descarga rápida.

   Las representaciones originales de los recursos seleccionados no se descargan si el administrador no [tiene autorización para acceder a las representaciones originales](../using/brand-portal-adding-users.md#main-pars-procedure-202029708).

   >[!NOTE]
   >
   >Los recursos seleccionados de forma individual y descargados son visibles en el informe descargado de recursos. Sin embargo, si se descarga una carpeta que contiene recursos, ni la carpeta ni los recursos se muestran en el informe descargado.

   Para obtener información sobre cómo descargar recursos de vínculos compartidos, consulte [Descarga de recursos de vínculos compartidos](../using/brand-portal-link-share.md#main-pars-header-1703469193).

## Rendimiento de descarga esperado {#expected-download-performance}

La experiencia de descarga de archivos puede variar para los usuarios en diferentes ubicaciones de cliente, según los factores como conexión a Internet local y latencia del servidor. El rendimiento de descarga esperado para un archivo de 2 GB observado en diferentes ubicaciones de cliente es el siguiente, con [!DNL Brand Portal] el servidor en Oregón en Estados Unidos:

| Ubicación del cliente | Latencia entre cliente y servidor | Velocidad de descarga esperada | Tiempo empleado para descargar un archivo de 2 GB |
|-------------------------|-----------------------------------|-------------------------|------------------------------------|
| Zona occidental de Estados Unidos (Norte de California) | 18 milisegundos | 7,68 MB/s | 4 minutos |
| Zona occidental de EE. UU. (Oregón) | 42 milisegundos | 3,84 MB/s | 9 minutos |
| Zona oriental de EE. UU. (Norte de Virginia ) | 85 milisegundos | 1,61 MB/s | 21 minutos |
| APAC (Tokio) | 124 milisegundos | 1,13 MB/s | 30 minutos |
| Noida | 275 milisegundos | 0,5 MB/s | 68 minutos |
| Sídney | 175 milisegundos | 0,49 MB/s | 69 minutos |
| Londres | 179 milisegundos | 0,32 MB/s | 106 minutos |
| Singapur | 196 milisegundos | 0,5 MB/s | 68 minutos |

**Nota**: Los datos citados se observan bajo condiciones de prueba, que pueden variar para los usuarios en distintas ubicaciones que ven diversas latencia y ancho de banda.
