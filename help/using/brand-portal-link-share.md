---
title: Compartir recursos como un vínculo
seo-title: Share assets as a link
description: Adobe Experience Manager Assets los administradores de Brand portal pueden compartir vínculos de varios activos con usuarios internos y entidades externas autorizados, incluidos socios y proveedores. Los editores pueden vista y compartir solo los activos compartidos con ellos.
seo-description: Adobe Experience Manager Assets Brand Portal Administrators can share links of multiple assets with authorized internal users and external entities, including partners and vendors. Editors can view and share only the assets shared with them.
uuid: 8889ac24-c56d-4a47-b792-80c34ffb5c3f
contentOwner: bdhar
content-type: reference
topic-tags: sharing
products: SG_EXPERIENCEMANAGER/Brand_Portal
discoiquuid: f3573219-3c58-47ba-90db-62b003d8b9aa
exl-id: 9d254e95-a4fc-468d-ae1f-9690ddd3b4a1
source-git-commit: e3e35ad4be5c082ad7bac7bed8ea20a186d245ad
workflow-type: tm+mt
source-wordcount: '969'
ht-degree: 5%

---

# Compartir recursos como un vínculo {#share-assets-as-a-link}

Adobe Experience Manager Assets los administradores de Brand portal pueden compartir vínculos de varios activos con usuarios internos y entidades externas autorizados, incluidos socios y proveedores. Los editores solo pueden ver y compartir los recursos que han compartido con ellos.

El uso compartido de activos a través de un vincular es una forma cómoda de hacer que estén disponibles para terceros externos, ya que los receptores no tienen que iniciar sesión en Brand portal para acceder a la activos.

<!-- Link sharing access is restricted to editors and administrators. 
-->

Para obtener más información, consulte [ Administración de usuarios, grupos y funciones ](../using/brand-portal-adding-users.md#manage-user-roles) de usuario.


A continuación se detallan los pasos para compartir activos como vincular:

1. Inicie sesión en su inquilino de Brand portal. De forma predeterminada, se abre la **[!UICONTROL Archivos]** vista que contiene todos los activos y carpetas publicados.

1. Seleccione las activos o carpetas que desee compartir, o vaya a la **[!UICONTROL vista colecciones]** para compartir las recopilaciones que ha creado.

   ![select-multiple-assets](assets/select-assets-new.png)

1. En la barra de herramientas de la parte superior, haga clic en **[!UICONTROL Compartir vínculo]** icono.

   El **[!UICONTROL Vínculos compartidos]** aparece el cuadro de diálogo.

   ![](assets/link-sharing.png)

   * En el cuadro Dirección de correo electrónico, escriba el ID de correo electrónico del usuario con el que desea compartir el vínculo. Puede compartir el vínculo con varios usuarios. Si el usuario es miembro de su organización, seleccione su ID de correo electrónico de entre las sugerencias que aparecen en la lista desplegable. Si el usuario es externo, escriba el ID de correo electrónico completo y pulse **[!UICONTROL Entrar]**; el ID de correo electrónico se añade a la lista de usuarios.

      ![](assets/link-sharing-text.png)

   * En el **[!UICONTROL Asunto]** , escriba un asunto para el recurso que desea compartir.
   * En el **[!UICONTROL Mensaje]** , escriba un mensaje si es necesario.
   * En el **[!UICONTROL Caducidad]** , utilice el selector de fechas para especificar una fecha y hora de caducidad para el vínculo. De forma predeterminada, la fecha de caducidad se establece en 7 días a partir de la fecha en que comparta el vínculo.
   * Habilite la **[!UICONTROL Permitir la descarga del archivo original]** casilla de verificación para permitir que los destinatarios descarguen la representación original.

   Los activos compartidos a través del vínculo caducan después de cruzar la fecha y la hora especificadas en la **[!UICONTROL Caducidad]** field. Para obtener información sobre el comportamiento de los recursos caducados y los cambios en las actividades permitidas en función de las funciones de usuario en Brand Portal, consulte [Administración de los derechos digitales de recursos](../using/manage-digital-rights-of-assets.md#asset-expiration).

   >[!NOTE]
   >
   >El tiempo de caducidad predeterminado para el vínculo es de 7 días. El vínculo debe enviarse por correo electrónico a los usuarios que utilizan la variable **[!UICONTROL Vínculos compartidos]** , no copie y comparta el vínculo por separado.

1. Clic **[!UICONTROL Compartir]**. Un mensaje confirma que la vincular se comparte con los usuarios. Los usuarios reciben un correo electrónico que contiene los vincular compartidos.

   ![](assets/link-share-email.png)

   >[!NOTE]
   >
   >Los administradores pueden personalizar el correo electrónico mensajería, lo que incluye personalizar el logotipo, la descripción y el pie de página con la función de personalización de [ marca ](../using/brand-portal-branding.md) .

## Descarga de recursos desde vínculos compartidos {#download-assets-from-shared-links}

Haga clic en el vínculo del correo electrónico para acceder al recurso compartido. AEM Se abre la página Uso compartido de vínculos.

Para descargar los recursos compartidos:

1. Haga clic en los recursos o carpetas y, a continuación, haga clic en **[!UICONTROL Descargar]** de la barra de herramientas.

   ![](assets/download-share-link.png)

   >[!NOTE]
   >
   >Actualmente, solo se puede generar una vista previa y una miniatura para determinados recursos, según el formato de archivo. Para obtener más información sobre los formatos de archivo compatibles, consulte [Compatibilidad con vista previa y miniaturas para formatos de recursos](#preview-thumbnail-support).

1. Se abre el cuadro de **[!UICONTROL diálogo descargar]** .

   ![cuadro de diálogo de descargar](assets/download-dialog-box-new.png)

1. De forma predeterminada, la **[!UICONTROL configuración de descarga]** rápida está habilitada en la **[!UICONTROL configuración]** de descarga. Por lo tanto, aparece un cuadro de confirmación para continuar la descarga con IBM aspera Connect.

   Para continuar con **[!UICONTROL la descarga]** rápida, haga clic en **[!UICONTROL permitir]** .

   Todas las representaciones seleccionadas se descargan en una carpeta ZIP que contiene una carpeta independiente para cada recurso.

   >[!NOTE]
   >
   >Se crea una carpeta independiente para cada recurso al descargar la activos desde una vincular compartida.
   >
   >Si se selecciona una carpeta, colección o más de 20 activos para descargar, el **[!UICONTROL cuadro de diálogo de descarga]** se omite y todas las representaciones de recurso accesibles para el usuario de exclusión de las representaciones dinámicas se descargan en una carpeta ZIP que contiene una carpeta independiente para cada recurso.

   >[!NOTE]
   >
   >Las representaciones originales no se descargan mediante el vincular compartido si la usuario que compartía la activos como vincular no [ está autorizada por el administrador para acceder a las representaciones ](../using/brand-portal-adding-users.md#manage-group-roles-and-privileges) originales.


>[!NOTE]
>
>Brand portal restringe descargar de carpetas o activos, cuyo tamaño es superior a 5 GB, utilizando vincular compartir.

<!--
1. The **[!UICONTROL Download]** dialog box appears.

   ![](assets/download-linkshare.png)

    * To speed up the download of asset files shared as the link, select **[!UICONTROL Enable download acceleration]** option and [follow the wizard](../using/accelerated-download.md#download-workflow-using-file-accelerator). To know more about the fast download of assets on Brand Portal refer [Guide to accelerate downloads from Brand Portal](../using/accelerated-download.md).
    
1. To download the renditions of assets in addition to the assets from the shared link, select **[!UICONTROL Rendition(s)]** option. When you do so, **[!UICONTROL Exclude System Renditions]** option appears that is selected by default. This prevents the download of out-of-the-box renditions along with approved assets or their custom renditions.

   However, to allow auto-generated renditions to download along with custom renditions, deselect the **[!UICONTROL Exclude System Renditions]** option.

   >[!NOTE]
   >
   >Original renditions are not downloaded using the shared link if the user who shared the assets as a link is not [authorized by the administrator to have access to the original renditions](../using/brand-portal-adding-users.md#manage-group-roles-and-privileges).

   ![](assets/download-linkshare-autoren.png)

1. Click **[!UICONTROL Download]**. The assets (and renditions if selected) are downloaded as a ZIP file to your local folder. However, no zip file is created if a single asset is downloaded without any of the renditions, thereby ensuring speedy download.

-->

## Compatibilidad con Vista previa y vistas en miniatura para formatos recurso {#preview-thumbnail-support}

La siguiente matriz enumera los formatos de recurso para los que Brand portal admite miniaturas y previsualización:

| formato de recursos | Compatibilidad con miniaturas | Compatibilidad con Vista previa |
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
| IA | ✓ | ✕ |
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
| TARRO | ✓ | ✕ |
| RAR | ND | ✕ |
| TAR | ND | ✕ |
| ZIP | ✓ | ✕ |

La siguiente leyenda explica los símbolos utilizados en la matriz:

| Símbolo | Significado |
|---|---|
| ✓ | Este formato de archivo admite esta función |
| ✕ | El formato de archivo no admite esta función |
| ND | Esta característica no es aplicable a este archivo formato |
| &#42; | Esta función requiere compatibilidad con complementos para este archivo formato en AEM autor instancia pero no en Brand portal después de que activos se publique en Brand portal |

## Dejar de compartir recursos compartidos como vínculo {#unshare-assets-shared-as-a-link}

Para dejar de compartir recursos compartidos anteriormente como vínculo, haga lo siguiente:

1. Cuando inicia sesión en Brand Portal, la variable **[!UICONTROL Archivo]** La vista se abre de forma predeterminada. Para ver los recursos que ha compartido como vínculos, vaya a **[!UICONTROL Vínculos compartidos]** vista.

1. Revise los vínculos que ha compartido desde la lista mostrada.

   ![](assets/shared-links.png)

1. Para dejar de compartir un vínculo de la lista, selecciónelo y haga clic en **[!UICONTROL Dejar de compartir]** en la barra de herramientas de la parte superior.

   ![](assets/unshare-asset.png)

   >[!NOTE]
   >
   >La visualización de vínculos compartidos es específica de usuario. Esta característica no muestra todos los vínculos compartidos por todos los usuarios de un inquilino.

1. En el cuadro mensaje de advertencia, haga clic en **[!UICONTROL continuar]** para confirmar anular uso compartido. La entrada del vincular se elimina del lista de los vínculos compartidos.
