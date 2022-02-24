---
title: Cargar recursos y publicar la carpeta Contribution de Brand Portal en Experience Manager Assets
seo-title: Upload assets and publish the Contribution folder from Brand Portal to Experience Manager Assets
description: Obtenga información sobre cómo cargar nuevos recursos y publicar la carpeta de contribución de Brand Portal a Experience Manager Assets.
seo-description: Get an insight into uploading new assets and publishing the contribution folder from Brand Portal to Experience Manager Assets.
uuid: null
content-type: reference
contentOwner: Vishabh Gupta
topic-tags: brand-portal
products: SG_EXPERIENCEMANAGER/Brand_Portal
discoiquuid: null
exl-id: 7dcf445d-97ed-4fa5-959c-c4c48e325766
source-git-commit: 7046f6523a2aa38ef2d4c7edf266953953543ae0
workflow-type: tm+mt
source-wordcount: '1032'
ht-degree: 0%

---

# Publicar carpeta de contribución en Experience Manager Assets {#using-asset-souring-in-bp}

Los usuarios de Brand Portal con los permisos adecuados pueden cargar varios recursos o carpetas que contengan varios recursos en la carpeta de contribución. Sin embargo, los usuarios de Brand Portal solo pueden cargar recursos en la variable **NUEVO** carpeta. La variable **COMPARTIDO** carpeta está diseñada para la distribución de recursos de línea de base (contenido de referencia) que pueden utilizar los usuarios de Brand Portal al crear nuevos recursos para contribución.

El usuario de Brand Portal que tiene permiso para acceder a la carpeta de contribución puede realizar las siguientes actividades:

* [Descargar los requisitos de los recursos](#download-asset-requirements)
* [Cargar nuevos recursos a la carpeta de contribución](#uplad-new-assets-to-contribution-folder)
* [Publicar carpeta de contribución en Experience Manager Assets](#publish-contribution-folder-to-aem)

## Descargar los requisitos de los recursos {#download-asset-requirements}

Los usuarios de Brand Portal reciben automáticamente notificaciones por correo electrónico o por pulso cada vez que el usuario de Experience Manager Assets comparte una carpeta de contribución, lo que les permite descargar el documento breve (requisito de recursos), así como descargar los recursos de línea de base (contenido de referencia) desde el **COMPARTIDO** para garantizar que comprenden los requisitos de los recursos.

El usuario de Brand Portal realiza las siguientes actividades para descargar los requisitos de recursos:

* **Descargar resumen**: Descargue el documento breve (documento de requisitos de recursos) adjunto a la carpeta de contribución que contiene información relacionada con los recursos, como el tipo de recursos, el propósito, los formatos admitidos, el tamaño máximo de los recursos, etc.
* **Descargar recursos de línea de base**: Descargue los recursos de línea de base que se pueden utilizar para comprender los tipos de recursos necesarios. Los usuarios de Brand Portal pueden utilizar estos recursos como referencia para crear nuevos recursos para contribución.

El panel de Brand Portal refleja todas las carpetas existentes permitidas al usuario de Brand Portal junto con la carpeta de contribución recientemente compartida. En este ejemplo, el usuario de Brand Portal solo tiene acceso a la carpeta de contribución recién creada; no se comparte ninguna otra carpeta con el usuario.

**Para descargar los requisitos de recursos:**

1. Inicie sesión en la instancia de Brand Portal.
1. Seleccione la carpeta de contribución en el panel de Brand Portal.
1. Haga clic en **[!UICONTROL Propiedades]**. Se abre la ventana Propiedad que contiene los detalles de la carpeta de contribución.

   ![](assets/properties.png)

   ![](assets/download-asset-requirement2.png)

1. Haga clic en el **[!UICONTROL Descargar resumen]** para descargar el documento de requisitos de recursos en el equipo local.

   ![](assets/download.png)

1. Vuelva al panel de Brand Portal.
1. Haga clic para abrir la carpeta de contribución. Verá dos subcarpetas:**[!UICONTROL COMPARTIDO]** y **[!UICONTROL NUEVO]** en la carpeta de contribución. La carpeta SHARED contiene todos los recursos de línea de base (contenido de referencia) compartidos por los administradores.
1. Puede descargar el **[!UICONTROL COMPARTIDO]** carpeta que contiene todos los recursos de línea de base del equipo local.
O bien, puede abrir el **[!UICONTROL COMPARTIDO]** y haga clic en **Descargar** para descargar archivos/carpetas individuales.

   ![](assets/download.png)

   ![](assets/download-asset-requirement5.png)

Consulte el documento breve (documento de requisitos de recursos) y consulte los recursos de línea de base para comprender los requisitos de los recursos. Ahora, puede crear nuevos recursos para la contribución y cargarlos en la carpeta de contribución.


## Cargar recursos a la carpeta de contribución {#uplad-new-assets-to-contribution-folder}

Después de pasar por los requisitos de recursos, los usuarios de Brand Portal pueden crear nuevos recursos para contribución y cargarlos en la carpeta NEW de la carpeta de contribución.

>[!NOTE]
>
>Los usuarios de Brand Portal pueden cargar recursos (un máximo de **2** GB por tamaño de archivo) a la NUEVA carpeta.
>
>El límite máximo de carga para cualquier inquilino de Brand Portal es **10** GB que se aplica acumulativamente a todas las carpetas de contribución.
>
>Los recursos cargados en Brand Portal no se procesan para representaciones y no contienen vistas previas.

>[!NOTE]
>
>Se recomienda liberar el espacio de carga después de publicar la carpeta de contribución en Experience Manager Assets, de modo que esté disponible para los demás usuarios de Brand Portal para que contribuyan.
>
>Si es necesario ampliar el límite de carga de su inquilino de Brand Portal más allá **10** GB, póngase en contacto con el servicio de atención al cliente para especificar el requisito.


**Para cargar nuevos recursos:**

1. Inicie sesión en la instancia de Brand Portal.
El panel de Brand Portal refleja todas las carpetas existentes permitidas al usuario de Brand Portal junto con la carpeta de contribución recientemente compartida.

1. Seleccione la carpeta de contribución y haga clic en para abrirla. La carpeta de contribución contiene dos subcarpetas: **[!UICONTROL COMPARTIDO]** y **[!UICONTROL NUEVO]**.

1. Haga clic en el **[!UICONTROL NUEVO]** carpeta.

   ![](assets/upload-new-assets4.png)

1. Haga clic en **[!UICONTROL Crear]** > **[!UICONTROL Archivos]** para cargar archivos individuales o carpetas (.zip) que contengan varios recursos.

   ![](assets/upload-new-assets5.png)

1. Examine y cargue recursos (archivos o carpetas) en el **[!UICONTROL NUEVO]** carpeta.

   ![](assets/upload-asset4.png)

Después de cargar todos los recursos o carpetas en la carpeta NEW , publique la carpeta de contribución en Experience Manager Assets.


## Publicar carpeta de contribución en Experience Manager Assets {#publish-contribution-folder-to-aem}

Los usuarios de Brand Portal pueden publicar la carpeta de contribución en Experience Manager Assets sin necesidad de acceder a la instancia de creación de Experience Manager.

Asegúrese de haber pasado por los requisitos de recursos y de cargar los recursos recién creados en **NUEVO** dentro de la carpeta de contribución.

**Para publicar la carpeta de contribución:**

1. Inicie sesión en la instancia de Brand Portal.

1. Seleccione la carpeta de contribución en el panel de Brand Portal.
1. Haga clic en **[!UICONTROL Publicar en AEM]**.

   ![](assets/export.png)

   ![](assets/publish-contribution-folder-to-aem1.png)

Se envía una notificación por correo electrónico o por impulso al usuario y a los administradores de Brand Portal en diferentes etapas del flujo de trabajo de publicación:

1. **En cola** : se envía una notificación al usuario de Brand Portal y a los administradores de Brand Portal cuando déclencheur un flujo de trabajo de publicación en Brand Portal.

1. **Completar** : se envía una notificación al usuario de Brand Portal y a los administradores de Brand Portal cuando la carpeta de contribución se publica correctamente en Experience Manager Assets.

Después de publicar los recursos recién creados en Experience Manager Assets, los usuarios de Brand Portal pueden eliminarlos de la carpeta NEW . En cambio, el administrador de Brand Portal puede eliminar los recursos de las carpetas NUEVO y COMPARTIDO.

Una vez alcanzado el objetivo de crear la carpeta de contribución, el administrador de Brand Portal puede eliminar la carpeta de contribución para liberar el espacio de carga para otros usuarios.

## Estado del trabajo de publicación {#publishing-job-status}

Los administradores pueden utilizar dos informes para ver el estado de las carpetas de contribución de recursos publicadas desde Brand Portal en Experience Manager Assets.

* En Brand Portal, vaya a **[!UICONTROL Herramientas]** > **[!UICONTROL Estado de contribución de recursos]**. Este informe refleja el estado de todos los trabajos de publicación en diferentes etapas del flujo de trabajo de publicación.

   ![](assets/contribution-folder-status.png)

* En Experience Manager Assets (servicio local o administrado), vaya a **[!UICONTROL Recursos]** > **[!UICONTROL Trabajos]**. Este informe refleja el estado final (éxito o error) de todos los trabajos de publicación.

   ![](assets/publishing-status.png)

* En Experience Manager Assets as a Cloud Service, vaya a **[!UICONTROL Recursos]** > **[!UICONTROL Trabajos]**.

   O bien, puede navegar directamente a **[!UICONTROL Trabajos]** desde la navegación global.

   Este informe refleja el estado final (éxito o error) de todos los trabajos de publicación, incluida la importación de recursos de Brand Portal a Experience Manager Assets as a Cloud Service.

   ![](assets/cloud-service-job-status.png)

<!--
>[!NOTE]
>
>Currently, no report is generated in AEM Assets as a Cloud Service for the Asset Sourcing workflow. 
-->
