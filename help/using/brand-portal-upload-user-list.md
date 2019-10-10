---
title: Cargar lista de usuarios de Brand Portal
seo-title: Cargar lista de usuarios de Brand Portal
description: 'Obtenga información sobre cómo cargar la lista de usuarios de Brand Portal en Recursos AEM. '
seo-description: Obtenga información sobre cómo cargar la lista de usuarios de Brand Portal en Recursos AEM.
uuid: null
content-type: referencia
topic-tags: portal de marca
products: SG_EXPERIENCEMANAGER/Brand_Portal
discoiquuid: null
translation-type: tm+mt
source-git-commit: f7f8c507d7f9866025987317af23f25c0b51c332

---


# Cargar lista de usuarios de Brand Portal {#upload-bp-user-list}

Los administradores de AEM pueden cargar el archivo de configuración de usuario de Brand Portal (.csv) que contiene la lista de usuarios activa de Brand Portal en Recursos AEM. Una carpeta de contribución solo se puede compartir con los usuarios activos de Brand Portal definidos en la lista de usuarios. El administrador también puede agregar usuarios nuevos en el archivo de configuración y cargar la lista de usuarios modificada.

El administrador puede agregar usuarios nuevos en la Consola de administración de AEM. Consulte [Administrar usuarios](brand-portal-adding-users.md) para obtener información detallada. Después de agregar usuarios en Admin Console, estos usuarios se pueden agregar al archivo de configuración de usuario de Brand Portal y, a continuación, se les puede asignar permiso para acceder a la carpeta de contribución.

**Para cargar la lista de usuarios de Brand Portal:**
1. Inicie sesión en la instancia de creación de AEMURL predeterminada: http:// localhost:4502/aem/start.html
1. En el panel **Herramientas** ![](assets/tools.png) , vaya a **[!UICONTROL Recursos &gt; Usuarios de Brand Portal]**
   ![](assets/upload-user-list1.png)
1. Se abre la ventana Contribuyentes de carga de Brand Portal.
Navegue desde el equipo local y cargue el archivo **de** configuración (.csv) que contiene la lista de usuarios activa de Brand Portal.
1. Haga clic en **[!UICONTROL Guardar]**.
   ![](assets/upload-user-list2.png)


Los administradores pueden proporcionar acceso a usuarios o grupos específicos desde esta lista de usuarios mientras configuran la carpeta de contribución.

Para obtener más información, consulte [Configurar carpeta](brand-portal-contribution-folder.md)de contribución.
