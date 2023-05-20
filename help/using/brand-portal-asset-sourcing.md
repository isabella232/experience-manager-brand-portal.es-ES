---
title: Abastecimiento de recursos en Brand Portal
seo-title: Asset Sourcing in Brand Portal
description: Obtenga una conocimiento en la función de abastecimiento de recurso que se ha publicado en el portal de marca Adobe Experience Manager Assets.
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
source-git-commit: 955cd8afe939ff47e9f08f312505e230e2f38495
workflow-type: tm+mt
source-wordcount: '646'
ht-degree: 1%

---

# Información general sobre el abastecimiento de recursos {#overview-asset-sourcing-in-bp}

**El abastecimiento** de recursos permite a los usuarios de assets de Experience Manager (administradores/usuarios no administradores) crear nuevas carpetas con una contribución **de recursos adicional** propiedad, lo que garantiza que la nueva carpeta creada esté abierta para recurso envío por los usuarios de Brand portal. Esto almacena automáticamente en déclencheur un flujo de trabajo que crea dos subcarpetas adicionales, denominadas **COMPARTIDO** y **NUEVO**, en el recién creado **Contribución** carpeta. A continuación, el administrador define el requisito cargando una breve descripción de los tipos de recursos que se deben añadir a la carpeta Contribution, así como un conjunto de recursos de línea de base, a **COMPARTIDO** para garantizar que los usuarios de BP tengan la información de referencia que necesitan. El administrador puede otorgar a los usuarios activos de Brand Portal acceso a la carpeta de contribución antes de publicar el recién creado **Contribución** a Brand Portal. Una vez que el usuario haya terminado de agregar contenido en la **NUEVO** , pueden volver a publicar la carpeta de contribución en el entorno de creación de Experience Manager. Tenga en cuenta que puede tardar unos minutos en completar la importación y reflejar el contenido recién publicado en Experience Manager Assets.

Además, todas las funciones existentes permanecen sin cambios. Los usuarios de Brand Portal pueden ver, buscar y descargar recursos desde la carpeta de contribuciones y desde otras carpetas permitidas. Además, los administradores pueden compartir la carpeta de contribución, modificar las propiedades y añadir recursos a las colecciones.

![Abastecimiento de recursos Brand Portal](assets/asset-sourcing.png)

>[!VIDEO](https://video.tv.adobe.com/v/29365/?quality=12)

## Requisitos previos {#prerequisites}

* Instancia as a Cloud Service de Experience Manager Assets, Experience Manager Assets 6.5.2 o superior.
* Asegúrese de que la instancia de Experience Manager Assets esté configurada con Brand Portal. [Consulte Configuración de Experience Manager assets con Brand portal ](../using/configure-aem-assets-with-brand-portal.md) .

<!--
* Ensure that your Brand Portal tenant is configured with one AEM Assets author instance.
-->

>[!NOTE]
>
>La función de abastecimiento de recursos está habilitada de forma predeterminada en Experience Manager Assets como Cloud Service, Experience Manager Assets 6.5.9 y versiones posteriores.
>
>Las configuraciones existentes seguirán funcionando en las versiones anteriores.

>[!NOTE]
>
>Hay un problema conocido en Experience Manager Assets 6.5.4. Los usuarios de Brand Portal no pueden publicar los recursos de la carpeta Contribution en Experience Manager Assets al actualizar a la consola de Adobe Developer.
>
>El problema se corrige en Experience Manager Assets 6.5.5. Puede actualizar la instancia de Experience Manager Assets al Service Pack más reciente y [actualizar las configuraciones](https://experienceleague.adobe.com/docs/experience-manager-65/assets/brandportal/configure-aem-assets-with-brand-portal.html#upgrade-integration-65) en la consola de Adobe Developer.

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

Los administradores de Experience Manager Assets pueden cargar el archivo de configuración de usuario (.csv) de Brand Portal que contiene la lista de usuarios activos de Brand Portal en Experience Manager Assets para permitirles acceder a la función de obtención de recursos.

Una carpeta de contribución solo se puede compartir con los usuarios activos de Brand Portal definidos en la lista de usuarios. El administrador también puede agregar nuevos usuarios al archivo de configuración y cargar la lista de usuarios modificada.

>[!NOTE]
>
>Asegúrese de que la instancia de Experience Manager Assets esté configurada con Brand Portal. Consulte. [Configuración de Experience Manager Assets con Brand Portal](../using/configure-aem-assets-with-brand-portal.md).

>[!NOTE]
>
>La formato del archivo CSV es la misma que la que se admite en Admin Console para la importación masiva usuario. El correo electrónico, el nombre y los apellidos son obligatorios.

Los administradores pueden agregar nuevos usuarios en Admin Console, consulte [ Administración de usuarios ](brand-portal-adding-users.md) para obtener información detallada. Después de agregar usuarios en Admin Console, estos usuarios se pueden agregar al archivo de configuración usuario de Brand portal y, a continuación, asignar permiso para acceder a la carpeta de contribución.

**Para cargar usuarios de Brand portal lista:**

1. Inicie sesión en la instancia de Experience Manager Assets.
1. Desde el **Herramientas**  panel, vaya a **[!UICONTROL Assets]** > **[!UICONTROL Usuarios de Brand Portal]**.

1. Se abre la ventana Cargar colaboradores de Brand Portal.
Examine desde el equipo local y cargue **archivo de configuración (.csv)** que contiene la lista de usuarios activos de Brand Portal.
1. Haga clic en **[!UICONTROL Guardar]**.

   ![](assets/upload-user-list2.png)


Los administradores pueden proporcionar acceso a usuarios específicos desde esta lista de usuarios mientras configuran una carpeta de contribución. Solo los usuarios asignados a una carpeta de contribución tendrán acceso a la carpeta de contribución y publicarán recursos de Brand Portal en Experience Manager Assets.

## Consulte también {#reference-articles}

* [Configurar y publicar carpeta de contribución en Brand portal](brand-portal-publish-contribution-folder-to-brand-portal.md)

* [Publish carpeta de contribución para Experience Manager Assets](brand-portal-publish-contribution-folder-to-aem-assets.md)
