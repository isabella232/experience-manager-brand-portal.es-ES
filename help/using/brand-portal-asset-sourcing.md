---
title: Abastecimiento de recursos en Brand Portal
seo-title: Abastecimiento de recursos en Brand Portal
description: Obtenga información sobre la función de abastecimiento de recursos lanzada en Adobe Experience Manager Assets Brand Portal.
seo-description: Obtenga información sobre la función de abastecimiento de recursos lanzada en Adobe Experience Manager Assets Brand Portal.
uuid: null
content-type: reference
contentOwner: Vishabh Gupta
topic-tags: brand-portal
products: SG_EXPERIENCEMANAGER/Brand_Portal
discoiquuid: null
product: experience-manager
sub-product: activos
feature: portal de marca
topics: collaboration, content-velocity, sharing
doc-type: feature-video
activity: use
audience: author, marketer
version: 6.5
kt: 3838
translation-type: tm+mt
source-git-commit: 5a61c42762e111b824163ce7d054d413a4da56bc
workflow-type: tm+mt
source-wordcount: '842'
ht-degree: 0%

---


# Información general sobre el abastecimiento de recursos {#overview-asset-sourcing-in-bp}

**La** fuente de recursos permite a los usuarios de AEM (administradores/usuarios no administradores) crear nuevas carpetas con una propiedad de  **contribución de** recursos adicional, lo que garantiza que la nueva carpeta creada esté abierta al envío de recursos por los usuarios de Brand Portal. Esto activa automáticamente un flujo de trabajo que crea dos subcarpetas adicionales, llamadas **SHARED** y **NEW**, dentro de la carpeta **Contribution** recién creada. A continuación, el administrador de AEM define el requisito cargando un resumen sobre los tipos de recursos que deben añadirse a la carpeta de contribución, así como un conjunto de recursos de línea de base, a la carpeta **SHARED** para garantizar que los usuarios de BP tengan la información de referencia que necesitan. A continuación, el administrador puede otorgar a los usuarios activos de Brand Portal acceso a la carpeta de contribución antes de publicar la carpeta **Contribution** recién creada en Brand Portal. Una vez que el usuario ha terminado de añadir contenido en la carpeta **NEW** , puede volver a publicar la carpeta de contribución en el entorno de creación de AEM. Tenga en cuenta que puede tardar unos minutos en completar la importación y reflejar el contenido recién publicado en AEM Assets.

Además, todas las funcionalidades existentes permanecen inalteradas. Los usuarios de Brand Portal pueden ver, buscar y descargar recursos de la carpeta de contribución, así como de otras carpetas permitidas. Y los administradores pueden compartir aún más la carpeta de contribución, modificar las propiedades y añadir recursos a las colecciones.

## Requisitos previos {#prerequisites}

* Instancia de AEM Assets as a Cloud Service, AEM Assets 6.5.2 o superior.
* Asegúrese de que la instancia de AEM Assets esté configurada con Brand Portal. Consulte [Configuración de AEM Assets con Brand Portal](../using/configure-aem-assets-with-brand-portal.md).
* Asegúrese de que el inquilino de Brand Portal esté configurado con una instancia de autor de AEM Assets.

>[!VIDEO](https://video.tv.adobe.com/v/29365/?quality=12)

![Abastecimiento de recursos de Brand Portal](assets/asset-sourcing.png)


>[!NOTE]
>
>Hay un problema conocido en AEM Assets 6.5.4. Los usuarios de Brand Portal no pueden publicar los recursos de la carpeta de contribución en AEM Assets al actualizar a Adobe Developer Console.
>
>El problema se ha solucionado en AEM 6.5.5. Puede actualizar la instancia de AEM Assets al último Service Pack AEM 6.5.5 y [actualizar sus configuraciones](https://docs.adobe.com/content/help/en/experience-manager-65/assets/brandportal/configure-aem-assets-with-brand-portal.html#upgrade-integration-65) en Adobe Developer Console.
>
>Para una corrección inmediata en AEM 6.5.4, se recomienda [descargar la corrección](https://www.adobeaemcloud.com/content/marketplace/marketplaceProxy.html?packagePath=/content/companies/public/adobe/packages/cq650/hotfix/cq-6.5.0-hotfix-33041) e instalarla en la instancia de autor.

## Configurar el abastecimiento de recursos {#configure-asset-sourcing}

**La fuente de** recursos se configura desde la instancia de creación de AEM Assets. Los administradores pueden habilitar la configuración del indicador de función de abastecimiento de recursos desde **AEM Web Console Configuration** y cargar la lista de usuarios activa de Brand Portal en **AEM Assets**.

>[!NOTE]
>
>El abastecimiento de recursos está habilitado de forma predeterminada en AEM Assets as a Cloud Service. El administrador de AEM puede cargar directamente los usuarios activos de Brand Portal para permitirles acceder a la función de abastecimiento de recursos.

>[!NOTE]
>
>Antes de comenzar con la configuración, asegúrese de que la instancia de AEM Assets esté configurada con Brand Portal. Consulte [Configuración de AEM Assets con Brand Portal](../using/configure-aem-assets-with-brand-portal.md).

En el siguiente vídeo se muestra cómo configurar el abastecimiento de recursos en la instancia de autor de AEM Assets:

>[!VIDEO](https://video.tv.adobe.com/v/29771)

### Habilitar el abastecimiento de recursos {#enable-asset-sourcing}

Los administradores de AEM pueden habilitar el indicador de la función de abastecimiento de recursos desde la Configuración de la consola web de AEM (también denominada Administrador de configuración).

>[!NOTE]
>
>Este paso no es aplicable a AEM Assets as a Cloud Service.


**Para habilitar el abastecimiento de recursos:**
1. Inicie sesión en la instancia de creación de AEM Assets y abra Configuration Manager.
Dirección URL predeterminada: http:// localhost:4502/system/console/configMgr.
1. Busque con la palabra clave **Asset Sourcing** para localizar **[!UICONTROL Asset Sourcing Feature Flag Config]**.
1. Haga clic en **[!UICONTROL Configuración del indicador de característica de abastecimiento de recursos]** para abrir la ventana de configuración.
1. Seleccione la casilla de verificación **[!UICONTROL feature.flag.active.status]**.
1. Haga clic en **[!UICONTROL Guardar]**.

![](assets/enable-asset-sourcing.png)

### Cargar la lista de usuarios de Brand Portal {#upload-bp-user-list}

Los administradores de AEM pueden cargar el archivo de configuración de usuario de Brand Portal (.csv) que contiene la lista de usuarios activa de Brand Portal en AEM Assets. Una carpeta de contribución solo se puede compartir con los usuarios activos de Brand Portal definidos en la lista de usuarios. El administrador también puede agregar nuevos usuarios en el archivo de configuración y cargar la lista de usuarios modificada.

>[!NOTE]
>
>El formato del archivo CSV es el mismo que se admite en Admin Console para la importación masiva de usuarios. El correo electrónico, el nombre y los apellidos son obligatorios.

Los administradores pueden agregar nuevos usuarios en AEM Admin Console; consulte [Administrar usuarios](brand-portal-adding-users.md) para obtener información detallada. Después de agregar usuarios en Admin Console, estos usuarios se pueden agregar al archivo de configuración de usuario de Brand Portal y se les puede asignar permisos para acceder a la carpeta de contribución.

**Para cargar la lista de usuarios de Brand Portal:**
1. Inicie sesión en la instancia de AEM Assets.
1. En el panel **Herramientas**, vaya a **[!UICONTROL Assets]** > **[!UICONTROL Usuarios de Brand Portal]**.

1. Se abre la ventana Cargar colaboradores de Brand Portal.
Busque desde el equipo local y cargue el archivo **de configuración (.csv)** que contiene la lista de usuarios activa de Brand Portal.
1. Haga clic en **[!UICONTROL Guardar]**.

   ![](assets/upload-user-list2.png)


Los administradores pueden proporcionar acceso a usuarios específicos desde esta lista de usuarios mientras configuran una carpeta de contribución. Solo los usuarios asignados a una carpeta de contribución tendrán acceso a la carpeta de contribución y publicarán recursos de Brand Portal en AEM Assets.

## Consulte también {#reference-articles}

* [Configuración y publicación de la carpeta de contribución en Brand Portal](brand-portal-publish-contribution-folder-to-brand-portal.md)

* [Publicar carpeta de contribución en AEM Assets](brand-portal-publish-contribution-folder-to-aem-assets.md)
