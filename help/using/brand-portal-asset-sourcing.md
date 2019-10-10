---
title: Origen de recursos en Brand Portal
seo-title: Origen de recursos en Brand Portal
description: Obtenga una visión detallada de la función de abastecimiento de recursos lanzada en Adobe Experience Manager Assets Brand Portal.
seo-description: Obtenga una visión detallada de la función de abastecimiento de recursos lanzada en Adobe Experience Manager Assets Brand Portal.
uuid: null
content-type: referencia
topic-tags: portal de marca
products: SG_EXPERIENCEMANAGER/Brand_Portal
discoiquuid: null
translation-type: tm+mt
source-git-commit: 413a6bd17d689d0af0cce20bbd7dedb6ae3cf9b5

---


# Información general sobre el origen de recursos {#overview-asset-sourcing-in-bp}

**La fuente** de recursos permite a los usuarios de AEM (administradores/usuarios no administradores) crear nuevas carpetas con una propiedad de contribución **de** recursos adicional, lo que garantiza que la nueva carpeta creada esté abierta al envío de recursos por parte de los usuarios de Brand Portal. Esto desencadena automáticamente un flujo de trabajo que crea dos subcarpetas adicionales, llamadas **COMPARTIDO** y **NUEVO**, dentro de la carpeta **Contribución** recién creada. A continuación, el administrador de AEM define el requisito cargando un resumen sobre los tipos de recursos que deben agregarse a la carpeta de contribución, así como un conjunto de recursos de línea de base, a la carpeta **COMPARTIDO** para garantizar que los usuarios de BP tengan la información de referencia que necesitan. A continuación, el administrador puede otorgar a los usuarios activos de Brand Portal acceso a la carpeta de contribución antes de publicar la carpeta de **contribución** recién creada en Brand Portal. Una vez que el usuario haya terminado de añadir contenido en la carpeta **NEW** , podrá volver a publicar la carpeta de contribución en el entorno de creación de AEM. Tenga en cuenta que la importación puede tardar unos minutos en completarse y reflejar el contenido recién publicado en Recursos AEM.

Además, todas las funcionalidades existentes permanecen sin cambios. Los usuarios de Brand Portal pueden ver, buscar y descargar recursos de la carpeta de contribución, así como de otras carpetas permitidas. Además, los administradores pueden compartir la carpeta de contribución, modificar las propiedades y añadir recursos a las colecciones.

>[!NOTE]
>
>La fuente de recursos en Brand Portal es compatible con AEM 6.5.2.0 y versiones posteriores.
>
>La función no es compatible con las versiones anteriores: AEM 6.3 y AEM 6.4.
>
>Póngase en contacto con el servicio de asistencia técnica de Adobe para actualizar su instancia de AEM a la última versión compatible de AEM.

![](assets/asset-sourcing.png)

## Consulte también {#reference-articles}

**Para administradores**
* [Configuración de fuentes de recursos en AEM](brand-portal-enable-asset-sourcing.md)
* [Cargar lista de usuarios de Brand Portal](brand-portal-upload-user-list.md)
* [Configurar carpeta de contribución](brand-portal-contribution-folder.md)
* [Carga de recursos de línea de base en la carpeta de contribución](brand-portal-upload-baseline-assets.md)
* [Publicar carpeta de contribución en Brand Portal](brand-portal-publish-contribution-folder-to-brand-portal.md)

**Para usuarios de Brand Portal**
* [Descargar requisitos de recursos](brand-portal-download-asset-requirements.md)
* [Carga de recursos nuevos en la carpeta de contribución](brand-portal-upload-assets-to-contribution-folder.md)
* [Publicación de la carpeta de contribución en Recursos AEM](brand-portal-publish-contribution-folder-to-aem-assets.md)
