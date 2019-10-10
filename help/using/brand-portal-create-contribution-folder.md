---
title: Crear carpeta de contribución
seo-title: Crear carpeta de contribución
description: 'Obtenga información sobre cómo crear una carpeta de contribución en Recursos AEM. '
seo-description: Obtenga información sobre cómo crear una carpeta de contribución en Recursos AEM.
uuid: null
content-type: referencia
topic-tags: portal de marca
products: SG_EXPERIENCEMANAGER/Brand_Portal
discoiquuid: null
translation-type: tm+mt
source-git-commit: 413a6bd17d689d0af0cce20bbd7dedb6ae3cf9b5

---


# Create contribution folder {#create-contribution-folder}

Los usuarios de AEM (administradores/usuarios no administradores) pueden crear nuevas carpetas en Recursos AEM con una propiedad de contribución **de** recursos adicional, lo que garantiza que la nueva carpeta creada esté abierta al envío de recursos por parte de los usuarios de Brand Portal.  Esto desencadena automáticamente un flujo de trabajo que crea dos subcarpetas adicionales, llamadas **COMPARTIDO** y **NUEVO**, dentro de la carpeta **Contribución** recién creada.

**Para crear una nueva carpeta de contribución:**
1. Inicie sesión en la instancia de creación de AEMURL predeterminada: http:// localhost:4502/aem/start.html
1. Vaya a **[!UICONTROL Recursos &gt; Archivos]**. Muestra todas las carpetas existentes en el repositorio de AEM Assets.
1. Click **[!UICONTROL Create]** to create a new folder. Se abre la ventana emergente Crear carpeta.
1. Introduzca **[!UICONTROL Título]** y **[!UICONTROL Nombre]** de la carpeta y marque la casilla de verificación Contribución **[!UICONTROL de]**recursos.
Se recomienda utilizar alfabetos pequeños sin espacio para nombrar la carpeta.
1. Haga clic en **[!UICONTROL Crear]**.
   ![](assets/create-contribution-folder.png)
1. Puede ver la carpeta de contribución recién creada en el repositorio de AEM Assets.
1. Haga clic para abrir la carpeta de contribución. Verá dos subcarpetas:**[!UICONTROL COMPARTIDO]** y **[!UICONTROL NUEVO]** , que se crean automáticamente en la carpeta de contribución.\
   ![](assets/contribution-folder.png)

Ahora puede configurar las propiedades de la carpeta Contribution recién creada. Consulte [Configuración de las propiedades](brand-portal-configure-contribution-folder-properties.md)de la carpeta Contribution.