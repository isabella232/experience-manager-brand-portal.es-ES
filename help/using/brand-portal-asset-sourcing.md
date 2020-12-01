---
title: Origen de recursos en Brand Portal
seo-title: Origen de recursos en Brand Portal
description: Obtenga una visión detallada de la función de abastecimiento de recursos lanzada en Adobe Experience Manager Assets Brand Portal.
seo-description: Obtenga una visión detallada de la función de abastecimiento de recursos lanzada en Adobe Experience Manager Assets Brand Portal.
uuid: null
content-type: reference
contentOwner: Vishabh Gupta
topic-tags: brand-portal
products: SG_EXPERIENCEMANAGER/Brand_Portal
discoiquuid: null
product: experience-manager
sub-product: activos
feature: brand-portal
topics: collaboration, content-velocity, sharing
doc-type: feature-video
activity: use
audience: author, marketer
version: 6.5
kt: 3838
translation-type: tm+mt
source-git-commit: 9c937603cf325919cb49d3418b06266fa1b93cf1
workflow-type: tm+mt
source-wordcount: '457'
ht-degree: 0%

---


# Información general sobre el origen de recursos {#overview-asset-sourcing-in-bp}

**La** fuente de recursos permite a los usuarios AEM (administradores/usuarios no administradores) crear nuevas carpetas con una propiedad  **** de contribución de recursos adicional, lo que garantiza que la nueva carpeta creada esté abierta al envío de recursos por parte de los usuarios de Brand Portal. Esto desencadena automáticamente un flujo de trabajo que crea dos subcarpetas adicionales, llamadas **SHARED** y **NEW**, dentro de la carpeta **Contribution** recién creada. A continuación, el administrador de AEM define el requisito cargando un resumen sobre los tipos de recursos que se deben agregar a la carpeta de contribución, así como un conjunto de recursos de línea de base, a la carpeta **SHARED** para garantizar que los usuarios de BP tengan la información de referencia que necesitan. A continuación, el administrador puede otorgar a los usuarios activos de Brand Portal acceso a la carpeta de contribución antes de publicar la carpeta **Contribution** recién creada en Brand Portal. Una vez que el usuario ha terminado de agregar contenido en la carpeta **NEW**, puede publicar la carpeta de contribución en el entorno de creación de AEM. Tenga en cuenta que la importación puede tardar unos minutos en completarse y reflejar el contenido recién publicado en AEM Assets.

Además, todas las funcionalidades existentes permanecen sin cambios. Los usuarios de Brand Portal pueden realizar vistas, búsquedas y descargas de recursos desde la carpeta de contribución, así como desde las demás carpetas permitidas. Además, los administradores pueden compartir la carpeta de contribución, modificar las propiedades y añadir recursos a las colecciones.

## Requisitos previos {#prerequisites}

* AEM 6.5.2 o superior.
* Asegúrese de que la instancia de AEM Assets esté configurada con Brand Portal. Consulte [Configuración de AEM Assets con Brand Portal](../using/configure-aem-assets-with-brand-portal.md).
* Asegúrese de que el inquilino de Brand Portal está configurado con una instancia de autor de AEM Assets.

>[!NOTE]
>
>La fuente de recursos no es compatible con AEM Assets como Cloud Service.


>[!VIDEO](https://video.tv.adobe.com/v/29365/?quality=12)

![Abastecimiento de recursos de Brand Portal](assets/asset-sourcing.png)


>[!NOTE]
>
>Hay un problema conocido en AEM 6.5.4. Los usuarios de Brand Portal no pueden publicar los recursos de la carpeta de contribución en AEM Assets al actualizar a Adobe Developer Console.
>
>El problema se ha corregido en la AEM 6.5.5. Puede actualizar su instancia de AEM Assets al Service Pack más reciente AEM 6.5.5 y [actualizar sus configuraciones](https://docs.adobe.com/content/help/en/experience-manager-65/assets/brandportal/configure-aem-assets-with-brand-portal.html#upgrade-integration-65) en la Consola de Adobe Developer.
>
>Para una corrección inmediata en AEM 6.5.4, se recomienda [descargar la revisión](https://www.adobeaemcloud.com/content/marketplace/marketplaceProxy.html?packagePath=/content/companies/public/adobe/packages/cq650/hotfix/cq-6.5.0-hotfix-33041) e instalarla en la instancia de creación.


## Consulte también {#reference-articles}

**Para administradores**

* [Configuración de fuentes de recursos en AEM](brand-portal-configure-asset-sourcing.md)
* [Cargar lista de usuarios de Brand Portal](brand-portal-configure-asset-sourcing.md)
* [Configurar carpeta de contribución](brand-portal-contribution-folder.md)
* [Carga de recursos de línea de base en la carpeta de contribución](brand-portal-upload-baseline-assets.md)
* [Publicar carpeta de contribución en Brand Portal](brand-portal-publish-contribution-folder-to-brand-portal.md)

**Para usuarios de Brand Portal**

* [Descargar requisitos de recursos](brand-portal-download-asset-requirements.md)
* [Carga de recursos nuevos en la carpeta de contribución](brand-portal-upload-assets-to-contribution-folder.md)
* [Publicar carpeta de contribución en AEM Assets](brand-portal-publish-contribution-folder-to-aem-assets.md)
