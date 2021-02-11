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
source-git-commit: 2f6ec4ac56390b2243e1d1a2c2adb34eb9aad7b2
workflow-type: tm+mt
source-wordcount: '258'
ht-degree: 0%

---


# Crear carpeta de contribución {#create-contribution-folder}


AEM los administradores y usuarios no administradores que tengan permiso para crear una nueva carpeta, pueden crear una carpeta de contribución en AEM Assets.
Para crear una carpeta de contribución, cree una nueva carpeta de tipo Contribución de recursos, asegurándose de que la nueva carpeta creada esté abierta al envío de recursos por parte de los usuarios de Brand Portal.  Esto déclencheur automáticamente un flujo de trabajo que crea dos subcarpetas adicionales, denominadas COMPARTIDO y NUEVO, dentro de la carpeta de contribución.

>[!NOTE]
>
>Puede crear varias carpetas de contribución dentro de una carpeta, pero no debe crear una carpeta de contribución dentro de otra carpeta de contribución.

Para crear una carpeta de contribución:
1. Inicie sesión en la instancia de creación de AEM.

   La dirección URL predeterminada es http:// localhost:4502/aem/start.html.

1. Vaya a **[!UICONTROL Recursos]** > **[!UICONTROL Archivos]**. Lista todas las carpetas existentes en el repositorio de AEM Assets.

1. Haga clic en **[!UICONTROL Crear]** para crear una nueva carpeta. **[!UICONTROL Se abre]** el cuadro de diálogo Crear carpeta.

1. Introduzca **[!UICONTROL Título]** y **[!UICONTROL Nombre]** de la carpeta y active la casilla de verificación **[!UICONTROL Contribución de recursos]**.
Se recomienda utilizar letras minúsculas sin ningún espacio para asignar un nombre a la carpeta.

1. Haga clic en **[!UICONTROL Crear]**. Puede ver la carpeta de contribución en el repositorio de AEM Assets.

   >[!NOTE]
   >
   >Un usuario no administrador puede crear y compartir una carpeta de contribución de recursos, pero no puede modificarla ni eliminarla.


   ![](assets/create-contribution-folder.png)

1. Haga clic para abrir la carpeta de contribución y verá dos subcarpetas:**[!UICONTROL SHARED]** y **[!UICONTROL NEW]** se crean automáticamente dentro de la carpeta de contribución.

   ![](assets/contribution-folder.png)

Ahora puede [configurar las propiedades de la carpeta de contribución](brand-portal-configure-contribution-folder-properties.md).


