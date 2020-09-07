---
title: Descargar recursos
seo-title: Descargar recursos
description: Todos los usuarios pueden descargar simultáneamente varios recursos y carpetas a los que tengan acceso. De este modo, los recursos de marca aprobados se pueden distribuir de forma segura para su uso sin conexión.
seo-description: Todos los usuarios pueden descargar simultáneamente varios recursos y carpetas a los que tengan acceso. De este modo, los recursos de marca aprobados se pueden distribuir de forma segura para su uso sin conexión.
uuid: 4b57118e-a76e-4d8a-992a-cb3c3097bc03
content-type: reference
products: SG_EXPERIENCEMANAGER/Brand_Portal
topic-tags: download-install
discoiquuid: f90c2214-beea-4695-9102-8b952bc9fd17
translation-type: tm+mt
source-git-commit: f4f92724cdd4ba8c79d3d72de5cba9451dceadb1
workflow-type: tm+mt
source-wordcount: '1294'
ht-degree: 2%

---


# Descargar recursos {#download-assets}

<!-- Before update in Download experience - 26th Aug 2020 by Vishabh.
 All users can simultaneously download multiple assets and folders accessible to them from Brand Portal. This way, approved brand assets can be securely distributed for offline use. Read on to know how to download approved assets from Brand Portal, and what to expect from the [download performance](../using/brand-portal-download-assets.md#main-pars-header).
-->

Adobe Experience Manager Assets Brand Portal mejora la experiencia de descarga al permitir a los usuarios descargar simultáneamente varios recursos y carpetas a los que pueden acceder desde Brand Portal. De este modo, los recursos de marca aprobados se pueden distribuir de forma segura para su uso sin conexión. Siga leyendo para saber cómo descargar los recursos aprobados desde Brand Portal y qué esperar del rendimiento [de la](../using/brand-portal-download-assets.md#expected-download-performance)descarga.

>[!NOTE]
>
>Instale IBM Aspera Connect 3.9.9 en la extensión de su navegador antes de descargar los recursos de Brand Portal.


<!--
**Types of renditions in Brand Portal:**

* Original asset rendition

  It is the original binary of the asset uploaded in AEM Assets. 
  
  
* System renditions

  These are the thumbnail renditions which are automatically generated in AEM Assets based on the "DAM update asset" workflow. 
  
* Custom renditions

  These are the additional renditions that an asset might have and its dynamic renditions. Any user can create additional custom renditions, whereas, only the AEM administrator can create dynamic renditions of an image in AEM Assets. To know more, see [how to apply image presets or dynamic renditions](../using/brand-portal-image-presets.md).     
-->

## Configuración de la descarga de recursos {#configure-download}

La configuración de descarga permite a los administradores de Brand Portal definir el conjunto de representaciones disponibles para los usuarios de Brand Portal para descargar los recursos. El administrador puede configurar la configuración de **[!UICONTROL descarga]** de recursos desde la interfaz de Brand Portal.

Las configuraciones disponibles son:

* **[!UICONTROL Descarga rápida]**

   Permite la descarga de los recursos a alta velocidad. Para obtener más información, consulte la [guía para acelerar las descargas desde Brand Portal](../using/accelerated-download.md).

* **[!UICONTROL Representaciones personalizadas]**

   Descargue representaciones personalizadas y dinámicas de los recursos.
Todas las representaciones de recursos que no sean el recurso original y las generadas por el sistema se denominan representaciones personalizadas. Incluye tanto representaciones estáticas como dinámicas disponibles para el recurso. Cualquier usuario puede crear una representación estática personalizada en AEM Assets, mientras que solo el administrador de AEM puede crear representaciones dinámicas personalizadas. Para obtener más información, consulte [cómo aplicar ajustes preestablecidos de imagen o representaciones dinámicas](../using/brand-portal-image-presets.md)

* **[!UICONTROL Representaciones del sistema]**

   Descargue representaciones de los recursos generadas por el sistema. Estas son las miniaturas que se generan automáticamente en AEM Assets en función del flujo de trabajo &quot;Recurso de actualización DAM&quot;.

Inicie sesión como administrador en el inquilino de Brand Portal y vaya a **[!UICONTROL Herramientas]** > **[!UICONTROL Descargar]**. De forma predeterminada, la configuración de Descarga **** rápida está habilitada en Configuración **[!UICONTROL de]** descarga.

Los administradores pueden habilitar cualquier combinación para configurar el proceso de descarga de recursos.

![](assets/download-configuration.png)


En función de la configuración, el flujo de trabajo de descarga permanece constante para los recursos independientes, varios recursos, carpetas que contienen recursos, recursos con licencia o sin licencia, y la descarga de recursos mediante un vínculo compartido.


* Si se desactivan las configuraciones de Representaciones **** personalizadas y de Representaciones **** del sistema, las representaciones originales de los recursos se descargan sin que se presente ningún cuadro de diálogo adicional a los usuarios.

<!--
If all the three download configurations are turned-off, or only the **[!UICONTROL Fast Download]** configuration is enabled, the original assets are directly downloaded on your local system with no additional step required.
Test.. 
-->

* Si está habilitada alguna de las representaciones **** personalizadas o la configuración de representaciones **** del sistema, aparece un cuadro de diálogo de **[!UICONTROL descarga]** adicional en el que puede elegir si desea descargar el recurso original junto con sus representaciones o descargar solo representaciones específicas.

>[!NOTE]
>
>Solo los administradores pueden descargar los recursos caducados. Para obtener más información sobre los recursos caducados, consulte [Gestión de derechos digitales de los recursos](../using/manage-digital-rights-of-assets.md).


## Pasos para descargar recursos {#steps-to-download-assets}

A continuación se indican los pasos para descargar recursos o carpetas que contengan recursos desde Brand Portal:

1. En la interfaz de Brand Portal, realice una de las siguientes acciones:

   * Seleccione las carpetas o los recursos que desee descargar. En la barra de herramientas de la parte superior, haga clic en el icono **[!UICONTROL Descargar]** .

      ![](assets/downloadassets-1.png)

   * Para descargar un recurso o una carpeta específicos, coloque el puntero sobre el recurso o la carpeta y haga clic en el icono **[!UICONTROL Descargar]** disponible en las miniaturas de acción rápida.

      ![](assets/downloadsingleasset-1.png)


      >[!NOTE]
      >
      >Si descarga los recursos por primera vez y no tiene instalado IBM Aspera Connect en su navegador, se le pedirá que instale el acelerador de descargas de Aspera.

      >[!NOTE]
      >
      >Si los recursos que está descargando también incluyen recursos con licencia, se le redirigirá a la página Administración de **[!UICONTROL derechos de autor]** . En esta página, seleccione los recursos, haga clic en **[!UICONTROL Aceptar]** y, a continuación, haga clic en **[!UICONTROL Descargar]**. Si no está de acuerdo, los recursos con licencia no se descargan.
      > 
      >Los recursos protegidos por licencias tienen un contrato de [licencia adjunto](https://helpx.adobe.com/experience-manager/6-5/assets/using/drm.html#DigitalRightsManagementinAssets) , lo que se realiza estableciendo la propiedad [de](https://helpx.adobe.com/experience-manager/6-5/assets/using/drm.html#DigitalRightsManagementinAssets) metadatos del recurso en Recursos Experience Manager.

      ![](assets/licensed-asset-download-1.png)

      Si alguna de las representaciones **** personalizadas o la configuración de representaciones **** del sistema está habilitada en Configuración **[!UICONTROL de]** descarga, aparecerá el cuadro de diálogo **[!UICONTROL Descargar]** con la casilla de verificación **** Recursos activada de forma predeterminada. Si la configuración de Descarga **** rápida está habilitada, la casilla de verificación **[!UICONTROL Activar aceleración]** de descarga está activada de forma predeterminada.

      ![](assets/download-dialog.png)

      >[!NOTE]
      >
      >Si los recursos que se descargan son archivos de imagen y sólo se selecciona la casilla de verificación **[!UICONTROL Recursos en el cuadro de diálogo]** Descargar **[!UICONTROL , pero el administrador no]** autoriza el acceso a las representaciones originales de los archivos [](../using/brand-portal-adding-users.md#main-pars-procedure-202029708) de imagen, no se descarga ningún archivo de imagen y aparece una notificación que indica que el administrador le ha restringido el acceso a las representaciones originales.

      ![](assets/restrictaccess-note.png)

1. Para descargar las representaciones además de los recursos originales, active la casilla de verificación **[!UICONTROL Representaciones]** . Sin embargo, si desea descargar las representaciones generadas por el sistema junto con las representaciones personalizadas, desactive la casilla de verificación **[!UICONTROL Excluir representaciones]** del sistema.

   ![](assets/download-system-rendition.png)

   * Para descargar solo las representaciones, desactive la casilla de verificación **[!UICONTROL Recursos]** .

      >[!NOTE]
      >
      >De forma predeterminada, solo se descargan los recursos. Sin embargo, las representaciones originales de los archivos de imagen no se descargan si el administrador no le [autoriza a acceder a las representaciones originales de los archivos](../using/brand-portal-adding-users.md#main-pars-procedure-202029708)de imagen.

   * Para compartir los recursos seleccionados con otros usuarios a través de un vínculo, active la casilla de verificación **[!UICONTROL Correo electrónico]** . Se envía una notificación por correo electrónico a los usuarios con el vínculo de descarga. Para obtener información sobre cómo descargar recursos de vínculos compartidos, consulte [Descarga de recursos de vínculos](../using/brand-portal-link-share.md#main-pars-header-1703469193)compartidos.

      ![](assets/download-link.png)

      >[!NOTE]
      >
      >El vínculo de descarga de la notificación por correo electrónico caduca pasados 45 días.
      >
      >Los administradores pueden personalizar los mensajes de correo electrónico, es decir, el logotipo, la descripción y el pie de página, mediante la función [Marcas](../using/brand-portal-branding.md) .

   * Puede seleccionar un ajuste preestablecido de imagen predefinido o crear una representación dinámica personalizada desde el cuadro de diálogo **[!UICONTROL Descargar]** .

      Para aplicar un ajuste preestablecido de imagen [personalizado al recurso y sus representaciones](../using/brand-portal-image-presets.md#applyimagepresetswhendownloadingimages), active la casilla de verificación Representaciones **[!UICONTROL dinámicas]** . Especifique las propiedades del ajuste preestablecido de imagen (como el tamaño, el formato, el espacio de color, la resolución y el modificador de imagen) para aplicar el ajuste preestablecido de imagen personalizado al descargar el recurso y sus representaciones. Para descargar solo las representaciones dinámicas, desactive la casilla de verificación **[!UICONTROL Recursos]** .

      ![](assets/dynamic-rendition.png)

      >[!NOTE]
      >
      >Brand Portal admite la configuración de Dynamic Media tanto en modo Hybird como en modo Scene 7.
      >
      >(*Si AEM instancia de autor se está ejecutando en el modo **híbrido de medios***dinámicos)      >Para realizar la previsualización o descarga de representaciones dinámicas de un recurso, asegúrese de que el medio dinámico está activado y que la representación de tiff piramidal del recurso existe en la instancia de creación de AEM Assets desde donde se han publicado los recursos. Cuando se publica un recurso en Brand Portal, también se publica su representación de tiff piramidal.

   * Para conservar la jerarquía de carpetas de Brand Portal al descargar recursos, active la casilla de verificación **[!UICONTROL Crear carpeta independiente para cada recurso]** . De forma predeterminada, se ignora la jerarquía de carpetas de Brand Portal y todos los recursos se descargan en una carpeta del sistema local.

1. Haga clic en **[!UICONTROL Descargar]**.

   Los recursos (y las representaciones, si se seleccionan) se descargan como un archivo zip en la carpeta local. Sin embargo, no se crea ningún archivo zip si se descarga un único recurso sin ninguna de las representaciones.

   Si el administrador no le [autoriza a acceder a las representaciones](../using/brand-portal-adding-users.md#main-pars-procedure-202029708)originales, las representaciones originales de los recursos seleccionados no se descargarán.

   >[!NOTE]
   >
   >Los recursos que se descargan de forma individual están visibles en el informe de descarga de recursos. Sin embargo, si se descarga una carpeta que contiene recursos, la carpeta y los recursos no se muestran en el informe de descarga de recursos.


## Rendimiento de descarga esperado {#expected-download-performance}

La experiencia de descarga de archivos puede variar para los usuarios en diferentes ubicaciones de clientes, según factores como la conectividad local a Internet y la latencia del servidor. El rendimiento de descarga esperado para archivos de 2 GB observado en diferentes ubicaciones de cliente es el siguiente, con el servidor Brand Portal en Oregon, Estados Unidos:

| Ubicación del cliente | Latencia entre cliente y servidor | Velocidad de descarga esperada | Tiempo necesario para descargar un archivo de 2 GB |
|-------------------------|-----------------------------------|-------------------------|------------------------------------|
| Zona occidental de Estados Unidos (Norte de California) | 18 milisegundos | 7,68 MB/s | 4 minutos |
| Zona occidental de EE. UU. (Oregón) | 42 milisegundos | 3,84 MB/s | 9 minutos |
| Zona oriental de EE. UU. (Norte de Virginia ) | 85 milisegundos | 1,61 MB/s | 21 minutos |
| APAC (Tokio) | 124 milisegundos | 1,13 MB/s | 30 minutos |
| Adobe | 275 milisegundos | 0,5 MB/s | 68 minutos |
| Sídney | 175 milisegundos | 0,49 MB/s | 69 minutos |
| Londres | 179 milisegundos | 0,32 MB/s | 106 minutos |
| Singapur | 196 milisegundos | 0,5 MB/s | 68 minutos |

>[!NOTE]
>
>Los datos citados se observan en condiciones de prueba, que pueden variar para los usuarios en distintas ubicaciones que presencian latencia y ancho de banda variados.

