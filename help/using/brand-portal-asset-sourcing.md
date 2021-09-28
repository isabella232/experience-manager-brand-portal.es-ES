---
title: Abastecimiento de recursos en Brand Portal
seo-title: Asset Sourcing in Brand Portal
description: Obtenga información sobre la función de abastecimiento de recursos lanzada en Adobe Experience Manager Assets Brand Portal.
seo-description: Get an insight into the asset sourcing feature released in the Adobe Experience Manager Assets Brand Portal.
uuid: null
content-type: reference
contentOwner: Vishabh Gupta
topic-tags: brand-portal
products: SG_EXPERIENCEMANAGER/Brand_Portal
discoiquuid: null
sub-product: assets
topics: collaboration, content-velocity, sharing
doc-type: feature-video
activity: use
audience: author, marketer
version: 6.5
kt: 3838
exl-id: 2c132a7a-ed10-4856-8378-67939167ea60
source-git-commit: d7dbf9ae2d27dda2edb60d8f861e618fb6332ec7
workflow-type: tm+mt
source-wordcount: '626'
ht-degree: 1%

---

# Información general de Asset Sourcing {#overview-asset-sourcing-in-bp}

**La** fuente de recursos permite a los usuarios AEM (administradores/usuarios no administradores) crear nuevas carpetas con una propiedad de  **contribución de** recursos adicional, lo que garantiza que la nueva carpeta creada esté abierta al envío de recursos por los usuarios de Brand Portal. Esto déclencheur automáticamente un flujo de trabajo que crea dos subcarpetas adicionales, llamadas **SHARED** y **NEW**, dentro de la carpeta **Contribution** recién creada. A continuación, el administrador de AEM define el requisito cargando un resumen sobre los tipos de recursos que deben agregarse a la carpeta de contribución, así como un conjunto de recursos de línea de base, a la carpeta **SHARED** para garantizar que los usuarios de BP tengan la información de referencia que necesitan. A continuación, el administrador puede otorgar a los usuarios activos de Brand Portal acceso a la carpeta de contribución antes de publicar la carpeta **Contribution** recién creada en Brand Portal. Una vez que el usuario ha terminado de añadir contenido en la carpeta **NEW** , puede volver a publicar la carpeta de contribución en el entorno de creación de AEM. Tenga en cuenta que puede tardar unos minutos en completar la importación y reflejar el contenido recién publicado en AEM Assets.

Además, todas las funcionalidades existentes permanecen inalteradas. Los usuarios de Brand Portal pueden ver, buscar y descargar recursos de la carpeta de contribución, así como de otras carpetas permitidas. Y los administradores pueden compartir aún más la carpeta de contribución, modificar las propiedades y añadir recursos a las colecciones.

![Abastecimiento de recursos de Brand Portal](assets/asset-sourcing.png)

>[!VIDEO](https://video.tv.adobe.com/v/29365/?quality=12)

## Requisitos previos {#prerequisites}

* AEM Assets como instancia de Cloud Service, AEM Assets 6.5.2 o superior.
* Asegúrese de que la instancia de AEM Assets esté configurada con Brand Portal. Consulte [Configuración de AEM Assets con Brand Portal](../using/configure-aem-assets-with-brand-portal.md).

<!--
* Ensure that your Brand Portal tenant is configured with one AEM Assets author instance.
-->

>[!NOTE]
>
>La función de abastecimiento de recursos está activada de forma predeterminada en AEM Assets as a Cloud Service, AEM Assets 6.5.9 y versiones posteriores.
>
>Las configuraciones existentes seguirán funcionando en las versiones anteriores.

>[!NOTE]
>
>Hay un problema conocido en AEM Assets 6.5.4. Los usuarios de Brand Portal no pueden publicar los recursos de las carpetas de contribución en AEM Assets al actualizar a Adobe Developer Console.
>
>El problema se ha solucionado en AEM 6.5.5. Puede actualizar la instancia de AEM Assets al último Service Pack AEM 6.5.5 y [actualizar sus configuraciones](https://experienceleague.adobe.com/docs/experience-manager-65/assets/brandportal/configure-aem-assets-with-brand-portal.html#upgrade-integration-65) en Adobe Developer Console.

<!--

>For immediate fix on AEM 6.5.4, it is recommended to [download the hotfix](https://www.adobeaemcloud.com/content/marketplace/marketplaceProxy.html?packagePath=/content/companies/public/adobe/packages/cq650/hotfix/cq-6.5.0-hotfix-33041) and install on your author instance.
-->

<!--
## Configure Asset Sourcing {#configure-asset-sourcing}

**Asset Sourcing** is configured from within the AEM Assets author instance. The administrators can enable the Asset Sourcing feature flag configuration from the **AEM Web Console Configuration** and upload the active Brand Portal users list in **AEM Assets**.

>[!NOTE]
>
>Asset Sourcing is by default enabled on AEM Assets as a Cloud Service. The AEM administrator can directly upload the active Brand Portal users to allow them access to the Asset Sourcing feature.

>[!NOTE]
>
>Before you begin with the configuration, ensure that your AEM Assets instance is configured with Brand Portal. See, [Configure AEM Assets with Brand Portal](../using/configure-aem-assets-with-brand-portal.md). 

The following video demonstrates, how to configure Asset Sourcing on your AEM Assets author instance:

>[!VIDEO](https://video.tv.adobe.com/v/29771)
-->

<!--
### Enable Asset Sourcing {#enable-asset-sourcing}

AEM administrators can enable the Asset Sourcing feature flag from within the AEM Web Console Configuration (a.k.a Configuration Manager).

>[!NOTE]
>
>This step is not applicable for AEM Assets as a Cloud Service.


**To enable Asset Sourcing:**
1. Log in to your AEM Assets author instance and open Configuration Manager. 
Default URL: http:// localhost:4502/system/console/configMgr.
1. Search using the keyword **Asset Sourcing** to locate **[!UICONTROL Asset Sourcing Feature Flag Config]**.
1. Click **[!UICONTROL Asset Sourcing Feature Flag Config]** to open the configuration window.
1. Select the **[!UICONTROL feature.flag.active.status]** check box.
1. Click **[!UICONTROL Save]**.

![](assets/enable-asset-sourcing.png)
-->


### Cargar lista de usuarios de Brand Portal {#upload-bp-user-list}

AEM administradores pueden cargar el archivo de configuración de usuario de Brand Portal (.csv) que contiene la lista de usuarios de Brand Portal activa en AEM Assets para permitirles acceder a la función de abastecimiento de recursos.

Una carpeta de contribución solo se puede compartir con los usuarios activos de Brand Portal definidos en la lista de usuarios. El administrador también puede agregar nuevos usuarios en el archivo de configuración y cargar la lista de usuarios modificada.

>[!NOTE]
>
>Asegúrese de que la instancia de AEM Assets esté configurada con Brand Portal. Consulte [Configuración de AEM Assets con Brand Portal](../using/configure-aem-assets-with-brand-portal.md).

>[!NOTE]
>
>El formato del archivo CSV es el mismo que se admite en el Admin Console para la importación masiva de usuarios. El correo electrónico, el nombre y los apellidos son obligatorios.

Los administradores pueden agregar nuevos usuarios en AEM Admin Console; consulte [Administrar usuarios](brand-portal-adding-users.md) para obtener información detallada. Después de agregar usuarios en el Admin Console, estos usuarios se pueden agregar al archivo de configuración de usuario de Brand Portal y se les puede asignar permisos para acceder a la carpeta de contribución.

**Para cargar la lista de usuarios de Brand Portal:**

1. Inicie sesión en la instancia de AEM Assets.
1. En el panel **Herramientas**, vaya a **[!UICONTROL Recursos]** > **[!UICONTROL Usuarios de Brand Portal]**.

1. Se abre la ventana Brand Portal Upload Contributors .
Busque desde el equipo local y cargue el archivo **de configuración (.csv)** que contiene la lista de usuarios activa de Brand Portal.
1. Haga clic en **[!UICONTROL Guardar]**.

   ![](assets/upload-user-list2.png)


Los administradores pueden proporcionar acceso a usuarios específicos desde esta lista de usuarios mientras configuran una carpeta de contribución. Solo los usuarios asignados a una carpeta de contribución tendrán acceso a la carpeta de contribución y publicarán recursos de Brand Portal a AEM Assets.

## Consulte también {#reference-articles}

* [Configuración y publicación de la carpeta de contribución en Brand Portal](brand-portal-publish-contribution-folder-to-brand-portal.md)

* [Publicar carpeta de contribución en AEM Assets](brand-portal-publish-contribution-folder-to-aem-assets.md)
