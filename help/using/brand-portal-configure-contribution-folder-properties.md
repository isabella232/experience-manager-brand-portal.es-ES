---
title: Configuración de las propiedades de la carpeta Contribution
seo-title: Configuración de las propiedades de la carpeta Contribution
description: 'Obtenga información sobre cómo configurar las propiedades de una carpeta de contribución en Recursos AEM. '
seo-description: 'Obtenga información sobre cómo configurar las propiedades de una carpeta de contribución en Recursos AEM. '
uuid: null
content-type: referencia
topic-tags: portal de marca
products: SG_EXPERIENCEMANAGER/Brand_Portal
discoiquuid: null
translation-type: tm+mt
source-git-commit: a32de22b7d5ac2b53b31aab8675dfdac1f5a724c

---


# Configuración de las propiedades de la carpeta de contribución {#configure-contribution-folder-properties}

El administrador de AEM realiza las siguientes actividades mientras configura las propiedades de una carpeta de contribución.

* **Agregar descripción**: Proporcione una descripción de alto nivel de la carpeta de contribución.
* **Cargar resumen**:  Cargar documento de requisitos de recursos que contiene información relacionada con los recursos.
* **Agregar colaboradores**: Agregue usuarios o grupos de Brand Portal para otorgarles acceso a la carpeta de contribución.

El requisito de recursos se refiere a los detalles proporcionados por los administradores para ayudar a los colaboradores (usuarios de Brand Portal) a comprender la necesidad y los requisitos de la carpeta de contribución. El administrador carga un documento de requisitos de recursos que contiene información sobre el tipo de recursos que se deben agregar a la carpeta de contribución y la información relacionada con los recursos, por ejemplo, el propósito, el tipo de imágenes, el tamaño máximo, etc.

A continuación, el administrador puede conceder acceso a los usuarios y grupos de Brand Portal a la carpeta de contribución antes de publicar la carpeta de contribución recién creada en Brand Portal.

**Para configurar las propiedades de la carpeta de contribución:**
1. Inicie sesión en la instancia de creación de AEMURL predeterminada: http:// localhost:4502/aem/start.html
1. Vaya a **[!UICONTROL Recursos &gt; Archivos]** y busque la carpeta de contribución.
1. Seleccione la carpeta de contribución y haga clic en **[!UICONTROL Propiedades]** ![](assets/properties.png). Se abre la ventana Propiedades de la carpeta.
   ![](assets/contribution-folder-property1.png)
1. Vaya a la ficha Contribución **[!UICONTROL de]** recursos.
1. Introduzca una **[!UICONTROL descripción]** de alto nivel de la carpeta de contribución.
1. Haga clic en **[!UICONTROL Cargar resumen]** ![](assets/upload.png) para buscar en el equipo local y cargar un documento **de requisitos de** recursos.
1. En **[!UICONTROL Agregar usuario o grupo]**, busque y **[!UICONTROL agregue]** usuarios o grupos de Brand Portal con los que desee compartir la carpeta de contribución.
Estos usuarios o grupos de Brand Portal tendrán permiso para acceder a la carpeta de contribución y cargar contenido desde la interfaz de Brand Portal sin necesidad de acceder a la instancia de creación de AEM.
1. Haga clic en **[!UICONTROL Guardar]**.
   ![](assets/contribution-folder-property2.png)

>[!NOTE]
>
>Los resultados de la búsqueda se basan en la lista de usuarios de Brand Portal configurada en Recursos AEM. Asegúrese de que dispone de la lista de usuarios de Brand Portal actualizada. Consulte [Carga de la lista](brand-portal-upload-user-list.md)de usuarios de Brand Portal.