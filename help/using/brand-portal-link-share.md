---
title: Compartir recursos como un vínculo
seo-title: Compartir recursos como un vínculo
description: Los administradores de AEM Assets Brand Portal pueden compartir vínculos de varios recursos con usuarios internos autorizados y entidades externas, incluidos socios y proveedores. Los editores pueden realizar vistas y compartir solo los recursos que se comparten con ellos.
seo-description: Los administradores de AEM Assets Brand Portal pueden compartir vínculos de varios recursos con usuarios internos autorizados y entidades externas, incluidos socios y proveedores. Los editores pueden realizar vistas y compartir solo los recursos que se comparten con ellos.
uuid: 8889ac24-c56d-4a47-b792-80c34ffb5c3f
contentOwner: bdhar
content-type: reference
topic-tags: sharing
products: SG_EXPERIENCEMANAGER/Brand_Portal
discoiquuid: f3573219-3c58-47ba-90db-62b003d8b9aa
translation-type: tm+mt
source-git-commit: ecd53a7d92dd020e6a3527793ff11efadcb531ee
workflow-type: tm+mt
source-wordcount: '1118'
ht-degree: 4%

---


# Compartir recursos como un vínculo {#share-assets-as-a-link}

Los administradores de AEM Assets Brand Portal pueden compartir vínculos de varios recursos con usuarios internos autorizados y entidades externas, incluidos socios y proveedores. Los editores pueden realizar vistas y compartir solo los recursos que se comparten con ellos.

El uso compartido de recursos a través de un vínculo es una forma práctica de ponerlos a disposición de terceros externos, ya que los receptores no tienen que iniciar sesión en Brand Portal para acceder a los recursos.

El acceso al uso compartido de vínculos está restringido a editores y administradores.

Para obtener más información, consulte [Administración de usuarios, grupos y funciones](../using/brand-portal-adding-users.md#manage-user-roles)de usuario.

>[!NOTE]
>
>Se permiten hasta 5 GB de descarga zip mediante la función de uso compartido de vínculos en Brand Portal.

A continuación se indican los pasos para compartir recursos como vínculo:

1. Haga clic en el icono de superposición de la izquierda y elija **[!UICONTROL Navegación]**.

   ![](assets/siderail.png)

1. Desde el lateral de la izquierda, haga clic en **[!UICONTROL Archivos]** para compartir carpetas o imágenes. Para compartir colecciones, haga clic en **[!UICONTROL Colecciones]**.

   ![](assets/navigationrail.png)

1. Seleccione las carpetas o colecciones que desee compartir como vínculo.

   ![](assets/asset-link-share.png)

1. En la barra de herramientas de la parte superior, haga clic en el icono **[!UICONTROL Compartir vínculo]** .

   Aparece el cuadro de diálogo **[!UICONTROL Vínculo compartido]** .

   ![](assets/link-sharing.png)

   >[!NOTE]
   >
   >El campo **[!UICONTROL Compartir vínculo]** muestra un vínculo de recurso creado automáticamente. La hora de caducidad predeterminada para este vínculo es de 7 días. Puede copiar el vínculo y compartirlo por separado con los usuarios o compartirlo desde el cuadro de diálogo **[!UICONTROL Vínculos compartidos]** .

1. En el cuadro de dirección de correo electrónico, escriba el ID de correo electrónico del usuario con el que desea compartir el vínculo. Puede compartir el vínculo con varios usuarios.

   Si el usuario es miembro de su organización, seleccione su ID de correo electrónico en las sugerencias que aparecen en la lista desplegable. Si el usuario es externo, escriba el ID de correo electrónico completo y pulse **[!UICONTROL Intro]**; el ID de correo electrónico se agrega a la lista de usuarios.

   ![](assets/link-sharing-text.png)

1. En el cuadro **[!UICONTROL Asunto]** , escriba un asunto para el recurso que desee compartir.
1. En el cuadro **[!UICONTROL Mensaje]** , escriba un mensaje si es necesario.
1. En el campo **[!UICONTROL Caducidad]** , utilice el selector de fechas para especificar una fecha y hora de caducidad para el vínculo. De forma predeterminada, la fecha de caducidad se establece en 7 días a partir de la fecha en que se comparte el vínculo.

   Los recursos compartidos a través del vínculo caducan después de superar la fecha y hora especificadas en el campo **[!UICONTROL Caducidad]** . Para obtener información sobre el comportamiento de los recursos caducados y los cambios en las actividades permisibles en función de las funciones de usuario en Brand Portal, consulte [Gestión de los derechos digitales de los recursos](../using/manage-digital-rights-of-assets.md#asset-expiration).

1. Haga clic en **[!UICONTROL Compartir]**. Un mensaje confirma que el vínculo se comparte con los usuarios. Los usuarios reciben un correo electrónico que contiene el vínculo.

   ![](assets/link-sharing-email.png)

   >[!NOTE]
   >
   >Los administradores pueden personalizar los mensajes de correo electrónico, lo que incluye personalizar el logotipo, la descripción y el pie de página con la función [de promoción de marca](../using/brand-portal-branding.md) .

## Descargar recursos de vínculos compartidos {#download-assets-from-shared-links}

Haga clic en el vínculo del correo electrónico para realizar la vista del recurso compartido. Se abre la página Compartir vínculos de AEM.

Para descargar los recursos compartidos:

1. Haga clic en los recursos y, a continuación, en el icono **[!UICONTROL Descargar]** de la barra de herramientas.

   ![](assets/assets-shared-link.png)

   >[!NOTE]
   >
   >Actualmente, puede generar una previsualización y una miniatura solo para determinados recursos, según el formato de archivo. Para obtener más información sobre los formatos de archivo admitidos, consulte Compatibilidad con [Previsualizaciones y miniaturas para los formatos](#preview-thumbnail-support)de recurso.

   >[!NOTE]
   >
   >Si los recursos que está descargando también incluyen recursos con licencia, se le redirigirá a la página Administración de **[!UICONTROL derechos de autor]** . En esta página, seleccione los recursos con licencia, haga clic en **[!UICONTROL Aceptar]** y, a continuación, haga clic en **[!UICONTROL Descargar]**. Si no está de acuerdo, solo se descargan los recursos sin licencia.\
   >Los recursos protegidos por licencias tienen un contrato [de licencia adjunto](https://helpx.adobe.com/experience-manager/6-5/assets/using/drm.html#DigitalRightsManagementinAssets) , lo que se realiza estableciendo la propiedad [de](https://helpx.adobe.com/experience-manager/6-5/assets/using/drm.html#DigitalRightsManagementinAssets) metadatos del recurso en [!DNL AEM Assets].

   ![](assets/licensed-asset-download.png)

   Aparecerá el cuadro de diálogo **[!UICONTROL Descargar]** .

   ![](assets/download-linkshare.png)

   * Para acelerar la descarga de archivos de recursos compartidos como vínculo, seleccione la opción **[!UICONTROL Activar aceleración]** de descarga y [siga las instrucciones del asistente](../using/accelerated-download.md#download-workflow-using-file-accelerator). Para obtener más información sobre la rápida descarga de recursos en Brand Portal, consulte la [Guía para acelerar las descargas desde Brand Portal](../using/accelerated-download.md).

1. Para descargar las representaciones de recursos además de los recursos desde el vínculo compartido, seleccione la opción **[!UICONTROL Representaciones]** . Al hacerlo, aparece la opción **[!UICONTROL Excluir representaciones]** del sistema que está seleccionada de forma predeterminada. Esto evita la descarga de representaciones integradas junto con los recursos aprobados o sus representaciones personalizadas.

   Sin embargo, para permitir la descarga de representaciones generadas automáticamente junto con representaciones personalizadas, anule la selección de la opción **[!UICONTROL Excluir representaciones]** del sistema.

   >[!NOTE]
   >
   >Las representaciones originales no se descargan mediante el vínculo compartido si el usuario que compartió los recursos como vínculo no está [autorizado por el administrador para tener acceso a las representaciones](../using/brand-portal-adding-users.md#manage-group-roles-and-privileges)originales.

   ![](assets/download-linkshare-autoren.png)

1. Toque o haga clic en **[!UICONTROL Descargar]**. Los recursos (y las representaciones si se seleccionan) se descargan como un archivo ZIP en la carpeta local. Sin embargo, no se crea ningún archivo zip si se descarga un único recurso sin ninguna representación, lo que garantiza una descarga rápida.

>[!NOTE]
>
>Brand Portal restringe la descarga de recursos de más de 5 GB por tamaño de archivo.

## Compatibilidad con previsualizaciones y miniaturas para formatos de recursos {#preview-thumbnail-support}

La siguiente matriz lista los formatos de recursos para los que Brand Portal admite miniaturas y previsualizaciones:

| Formato del recurso | Compatibilidad con miniaturas | Compatibilidad con previsualizaciones |
|--------------|-------------------|-----------------|
| PNG | ✓ | ✓ |
| GIF | ✓ | ✓ |
| TIFF | ✓ | ✕ |
| JPEG | ✓ | ✓ |
| BMP | ✓ | ✕ |
| PNM* | ND | ND |
| PGM* | ND | ND |
| PBM* | ND | ND |
| PPM* | ND | ND |
| PSD | ✓ | ✕ |
| EPS | ND | ✕ |
| DNG | ✓ | ✕ |
| PICT | ✓ | ✕ |
| PSB* | ✓ | ✕ |
| JPG | ✓ | ✓ |
| AI | ✓ | ✕ |
| DOC | ✕ | ✕ |
| DOCX | ✕ | ✕ |
| ODT* | ✕ | ✕ |
| PDF | ✓ | ✕ |
| HTML | ✕ | ✕ |
| RTF | ✕ | ✕ |
| TXT | ✓ | ✕ |
| XLS | ✕ | ✕ |
| XLSX | ✕ | ✕ |
| ODS | ✕ | ✕ |
| PPT | ✓ | ✕ |
| PPTX | ✕ | ✕ |
| ODP | ✕ | ✕ |
| INDD | ✓ | ✕ |
| PS | ✕ | ✕ |
| QXP | ✕ | ✕ |
| EPUB | ✓ | ✕ |
| AAC | ✕ | ✕ |
| MIDI | ✕ | ✕ |
| 3GP | ✕ | ✕ |
| MP3 | ✕ | ✕ |
| MP4 | ✕ | ✕ |
| OGA | ✕ | ✕ |
| OGG | ✕ | ✕ |
| RA | ✕ | ✕ |
| WAV | ✕ | ✕ |
| WMA | ✕ | ✕ |
| DVI | ✕ | ✕ |
| FLV | ✕ | ✕ |
| M4V | ✕ | ✕ |
| MPG | ✕ | ✕ |
| OGV | ✕ | ✕ |
| MOV | ✕ | ✕ |
| WMV | ✕ | ✕ |
| SWF | ✕ | ✕ |
| TGZ | ND | ✕ |
| JAR | ✓ | ✕ |
| RAR | ND | ✕ |
| TAR | ND | ✕ |
| ZIP | ✓ | ✕ |

La leyenda siguiente explica los símbolos utilizados en la matriz:

| Símbolo | Significado |
|---|---|
| ✓ | Este formato de archivo admite esta función |
| ✕ | Este formato de archivo no admite esta función |
| ND | Esta función no se aplica a este formato de archivo |
| * | Esta función requiere compatibilidad con complementos para este formato de archivo en AEM instancia de creación, pero no en Brand Portal después de publicar los recursos en Brand Portal |

## No compartir recursos compartidos como vínculo {#unshare-assets-shared-as-a-link}

Para dejar de compartir recursos compartidos anteriormente como vínculo, haga lo siguiente:

1. Para vista de los recursos compartidos como vínculos, haga clic en el icono de superposición de la izquierda y elija **[!UICONTROL Navegación]**.

   ![](assets/siderail.png)

1. Desde el lateral, haga clic en Vínculos **** compartidos.

   ![](assets/navigationrail.png)

1. Revise los vínculos que ha compartido desde la lista mostrada.
1. Para dejar de compartir un vínculo de la lista, selecciónelo y haga clic en el icono de bandeja situado junto a la entrada de vínculo o en el icono **[!UICONTROL Dejar de compartir]** de la barra de herramientas situada en la parte superior.

   ![](assets/unshare-links.jpg)

   >[!NOTE]
   >
   >La visualización de vínculos compartidos es específica del usuario. Esta función no muestra todos los vínculos compartidos por todos los usuarios de un inquilino.

1. En el cuadro de mensaje de advertencia, haga clic en **[!UICONTROL Continuar]** para confirmar que no se comparte. La entrada del vínculo se elimina de la lista de vínculos compartidos.
