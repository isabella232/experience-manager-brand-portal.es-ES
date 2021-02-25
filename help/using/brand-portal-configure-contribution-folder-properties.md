---
title: Configuración de las propiedades de la carpeta Contribution
seo-title: Configuración de las propiedades de la carpeta Contribution
description: 'Obtenga información sobre cómo configurar las propiedades de una carpeta de contribución en AEM Assets. '
seo-description: 'Obtenga información sobre cómo configurar las propiedades de una carpeta de contribución en AEM Assets. '
uuid: null
content-type: reference
contentOwner: Vishabh Gupta
topic-tags: brand-portal
products: SG_EXPERIENCEMANAGER/Brand_Portal
version: 6.5
discoiquuid: null
translation-type: tm+mt
source-git-commit: 1a2ede041a08c687022108a3d5f52c258c6b945a
workflow-type: tm+mt
source-wordcount: '285'
ht-degree: 0%

---


# Configurar las propiedades de la carpeta de contribución {#configure-contribution-folder-properties}

AEM administrador realiza las siguientes actividades al configurar las propiedades de una carpeta de contribución.

* **Añadir descripción**: Proporcione una descripción de alto nivel de la carpeta de contribución.
* **Cargar resumen**: Cargar documento de requisitos de recursos que contiene información relacionada con los recursos.
* **Añadir colaboradores**: Añada a los usuarios de Brand Portal para que les concedan acceso a la carpeta de contribución.

El requisito de recursos se refiere a los detalles proporcionados por los administradores para ayudar a los colaboradores (usuarios de Brand Portal) a comprender la necesidad y los requisitos de la carpeta de contribución. El administrador carga un documento de requisitos de recursos que contiene información sobre el tipo de recursos que se deben agregar a la carpeta de contribución y la información relacionada con los recursos, por ejemplo, el propósito, el tipo de imágenes, el tamaño máximo, etc.

**Para configurar las propiedades de la carpeta de contribución:**

1. Inicie sesión en la instancia de creación de AEM
Dirección URL predeterminada: http:// localhost:4502/aem/start.html
1. Vaya a **[!UICONTROL Recursos > Archivos]** y busque la carpeta de contribución.
1. Seleccione la carpeta de contribución y haga clic en **[!UICONTROL Propiedades]** para abrir la ventana Propiedades de la carpeta.

   ![](assets/properties.png)

   ![](assets/contribution-folder-property1.png)

1. Vaya a la ficha **[!UICONTROL Contribución de recursos]**.
1. Introduzca **[!UICONTROL Description]** de alto nivel de la carpeta de contribución.
1. Haga clic en **[!UICONTROL Cargar resumen]** para examinar desde el equipo local y cargar un **Documento de requisitos de recursos**.

   ![](assets/upload.png)

1. En el campo **[!UICONTROL Añadir usuario]**, agregue usuarios de Brand Portal con los que desee compartir la carpeta de contribución. Estos usuarios pueden acceder y cargar contenido en la carpeta de contribución mediante la interfaz de Brand Portal.
1. Haga clic en **[!UICONTROL Guardar]**.

   ![](assets/contribution-folder-property3.png)

>[!NOTE]
>
>Los resultados de la búsqueda se basan en la lista de usuario de Brand Portal configurada en AEM Assets. Asegúrese de que dispone de la lista de usuario de Brand Portal actualizada. Consulte [Carga de la lista de usuario de Brand Portal](brand-portal-configure-asset-sourcing.md).
