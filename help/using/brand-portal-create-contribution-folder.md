---
title: Crear carpeta de contribución
seo-title: Crear carpeta de contribución
description: 'Obtenga información sobre cómo crear una carpeta de contribución en AEM Assets. '
seo-description: Obtenga información sobre cómo crear una carpeta de contribución en AEM Assets.
uuid: null
content-type: reference
contentOwner: Vishabh Gupta
topic-tags: brand-portal
products: SG_EXPERIENCEMANAGER/Brand_Portal
discoiquuid: null
translation-type: tm+mt
source-git-commit: 70d93d37b04d899979e38b454e342ebd78bad3bb
workflow-type: tm+mt
source-wordcount: '258'
ht-degree: 0%

---


# Create contribution folder {#create-contribution-folder}


AEM los administradores y usuarios no administradores que tengan permiso para crear una nueva carpeta, pueden crear una carpeta de contribución en AEM Assets.
Para crear una carpeta de contribución, cree una nueva carpeta de tipo Contribución de recursos, asegurándose de que la nueva carpeta creada esté abierta al envío de recursos por parte de los usuarios de Brand Portal.  Esto desencadena automáticamente un flujo de trabajo que crea dos subcarpetas adicionales, denominadas COMPARTIDO y NUEVO, dentro de la carpeta de contribución.

>[!NOTE]
>
>Puede crear varias carpetas de contribución dentro de una carpeta, pero no debe crear una carpeta de contribución dentro de otra carpeta de contribución.

Para crear una carpeta de contribución:
1. Inicie sesión en la instancia de creación de AEM.

   La dirección URL predeterminada es http:// localhost:4502/aem/start.html.

1. Vaya a **[!UICONTROL Recursos]** > **[!UICONTROL Archivos]**. Lista todas las carpetas existentes en el repositorio de AEM Assets.

1. Click **[!UICONTROL Create]** to create a new folder. **[!UICONTROL Se abre el cuadro de diálogo Crear carpeta]** .

1. Introduzca el **[!UICONTROL título]** y el **[!UICONTROL nombre]** de la carpeta y active la casilla de verificación Contribución **[!UICONTROL de]** recursos.
Se recomienda utilizar letras minúsculas sin ningún espacio para asignar un nombre a la carpeta.

1. Haga clic en **[!UICONTROL Crear]**. Puede ver la carpeta de contribución en el repositorio de AEM Assets.

   >[!NOTE]
   >
   >Un usuario no administrador puede crear y compartir una carpeta de contribución de recursos, pero no puede modificarla ni eliminarla.

   ![](assets/create-contribution-folder.png)

1. Haga clic para abrir la carpeta de contribución. Verá dos subcarpetas:**[!UICONTROL COMPARTIDO]** y **[!UICONTROL NUEVO]** , que se crean automáticamente dentro de la carpeta de contribución.

   ![](assets/contribution-folder.png)

Ahora puede [configurar las propiedades](brand-portal-configure-contribution-folder-properties.md)de la carpeta de contribución.


