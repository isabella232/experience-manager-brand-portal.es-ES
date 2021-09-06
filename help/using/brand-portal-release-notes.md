---
title: Notas de la versión
seo-title: Release Notes
description: Obtenga información sobre las funciones, las mejoras, los problemas críticos corregidos y los problemas conocidos de la versión Adobe Experience Manager Assets Brand Portal 2021.08.0.
seo-description: Get an insight into the enhancements, critical issues fixed, and known issues in the Adobe Experience Manager Assets Brand Portal 2021.08.0 release.
uuid: 3d6ffb6f-4608-4e83-8486-5c90e06cdb43
content-type: reference
contentOwner: Vishabh Gupta
topic-tags: brand-portal
products: SG_EXPERIENCEMANAGER/Brand_Portal
discoiquuid: 79ebb9fc-385c-48a8-979e-374f42517988
exl-id: e4e89080-9863-4857-8f3a-fcd516ef3271
source-git-commit: c7ffeda69beb92ce8fa549fe270cc5156fa1ec1c
workflow-type: tm+mt
source-wordcount: '494'
ht-degree: 10%

---

# Notas de la versión {#release-notes}

Obtenga información sobre las nuevas funciones, mejoras, problemas críticos corregidos y problemas conocidos de la versión Adobe Experience Manager Assets Brand Portal 2021.08.0.

## Información de la versión {#release-information}

| Producto | Adobe Experience Manager Assets Brand Portal |
|---|---|
| Versión | 2021.08.0 |
| Fecha | Agosto de 2021 |

## Información general {#overview}

Adobe Experience Manager (AEM) Assets Brand Portal le ayuda a adquirir, controlar y distribuir de forma segura recursos creativos aprobados a terceros externos y usuarios empresariales internos entre dispositivos. Ayuda a mejorar la eficiencia del uso compartido de activos, acelera el tiempo de comercialización de los activos y reduce el riesgo de incumplimiento y acceso no autorizado. Brand Portal permite a los usuarios examinar, buscar, previsualizar, descargar y exportar recursos en formatos aprobados por la empresa, en cualquier momento y lugar.

## Novedades de 2021.08.0 {#whats-new-in-2021.08.0}

<!--
### New Features {#new-features}

This release includes the following new features:

* AEM Assets as a Cloud Service is now entitled to have a pre-configured Brand Portal instance. The Cloud Manager user can activate Brand Portal on the AEM Assets as a Cloud Service instance.

* Asset Sourcing feature is now available on AEM Assets as a Cloud Service. It allows the Brand Portal users to upload assets to the permitted contribution folders and publish the contribution folder from Brand Portal to AEM Assets as a Cloud Service instance. 

* An additional **[!UICONTROL Asset Download]** setting has been introduced under the **[!UICONTROL Download Settings]**. It creates a separate folder for each asset while downloading the folders, collections, or bulk download of assets. 
-->
<!-- 
* The **[!UICONTROL Download]** dialog is revamped in a list view with additional options to exclude the renditions which are not required, apply the same set of rules for similar asset types, and download the selected asset renditions. See [steps to download assets from Brand Portal](https://docs.adobe.com/content/help/en/experience-manager-brand-portal/using/download/brand-portal-download-assets.html#download-assets).
-->

<!--
* The new **[!UICONTROL Download]** dialog now appears with all the renditions of the selected assets or folders containing assets in a list view, wherein the Brand Portal users can apply same set of renditions for similar asset types and download the selected asset renditions. 
-->

<!-- 
* Navigation to the **[!UICONTROL Files]**, **[!UICONTROL Collections]**, and **[!UICONTROL Shared Links]** is now possible from all the Brand Portal pages in one-click.  

* The **[!UICONTROL Renditions]** panel in the asset details page now allows the Brand Portal users to select the original asset and (or) specific asset renditions, and directly download them from the **[!UICONTROL Renditions]** panel without having to open the **[!UICONTROL Download]** dialog. See [download assets from asset details page](https://docs.adobe.com/content/help/en/experience-manager-brand-portal/using/download/brand-portal-download-assets.html#download-assets-from-asset-details-page).
-->

<!--
Brand Portal users can exclude specific renditions which are not required and directly download the original asset and its renditions from the **[!UICONTROL Renditions]** panel on the asset details page. 
-->

<!-- 
* In addition to the existing **[!UICONTROL Download]** configurations, the Brand Portal administrators can also [configure permissions for different group of users](https://docs.adobe.com/content/help/en/experience-manager-brand-portal/using/download/brand-portal-download-assets.html#configure-download-permissions) to view and (or) download the original asset and its renditions from the asset details page. These configurations will define who can access and (or) download the asset renditions.
-->


### Mejoras {#enhancements}

Brand Portal 2021.08.0 es una versión interna que presenta perfiles empresariales para clientes de empresas y equipos a fin de que las organizaciones puedan controlar mejor sus recursos.

Esta versión incluye las siguientes mejoras:

* Los usuarios ahora tienen derechos específicos de la organización en las organizaciones nuevas y migradas. Si un usuario tiene derecho a varias organizaciones, debe seleccionar la organización en el momento del inicio de sesión.

* Los nuevos usuarios que se agregan en el Admin Console deben **Unirse al equipo** para tener derecho a la organización.

>[!NOTE]
>
>Actualmente, los perfiles empresariales son aplicables a las nuevas organizaciones creadas después del 16 de agosto de 2021.
>
>Hasta que se migre su organización, puede seguir utilizando Adobe ID, Enterprise ID o tipos de Federated ID para acceder a la organización.

<!-- 
* For folder download, a separate folder is created for each asset using share link irrespective of the **[!UICONTROL Download Settings]**. 
* The Brand Portal **[!UICONTROL Usage Report]** has been modified to reflect only the active Brand Portal users.
-->

<!--
* The threshold of session timeout for the guest users has been reduced from 2 hours to 15 minutes.
* The additional **[!UICONTROL View pages]** option has been removed for multi-page PDFs as the user can now view the PDF pages from the Adobe Document Cloud Viewer.
-->


### Problemas críticos solucionados {#critical-issues-fixed}

Esta versión incluye correcciones para los siguientes problemas críticos:

* Las notificaciones por correo electrónico de Asset Sourcing no se entregan en algunas organizaciones.

* Los archivos de vídeo con la extensión `.mov` no se ejecutan en Brand Portal.

* En la lista desplegable **[!UICONTROL Colecciones inteligentes]** solo se ven diez colecciones guardadas.

<!--
* *_deleted tenants are listed as valid tenant which fails during the execution of TenantCustomizers/TenantUpdates where tenant id is returned as /etc/tenants/`<nodename>`.
-->

<!--
In case only the original assets are downloaded, the asset reflects its own extension and does not open until the extension is manually changed to zip. 
* The user interface of the collection folder does not respond on clicking the navigation arrow. 
* **[!UICONTROL Create]** button is visible in the **[!UICONTROL Column]** view even when the folders are empty.
* **[!UICONTROL Omni search]** fails with a 414 error message (Request-URI Too Long) if the dispatcher is bypassed while accessing the Brand Portal instance.
* An empty zip folder is downloaded if the asset contains a comma (`,`) in the file name.
* The viewer users get the option to add users to the collection they have created. 
* Inconsistent behavior is experienced when an asset (thumbnail or web rendition) is downloaded using share link.

See [what's new in Brand Portal 2021.02.0](whats-new.md).
-->


### Problemas conocidos {#known-issues}

Esta versión incluye los siguientes problemas conocidos:

* Los usuarios no pueden iniciar sesión en Brand Portal durante la migración de su organización existente.

   Sin embargo, los usuarios activos que han iniciado sesión en Brand Portal pueden seguir funcionando hasta que su sesión actual caduque.

* Al pasar de Brand Portal a Admin Console, es posible que los administradores vean una pantalla adicional para seleccionar la organización.

* Los usuarios no pueden quitar el perfil de esquema de metadatos aplicado de una carpeta.


<!--
### Known Issues {#known-issues}

This release includes the following known issue:

* Search on the **[!UICONTROL Asset Reports]** shows processing on the product interface with no search result.
* The video DM encodes are not visible to the non-admin users on the asset details page.
* The alignment of the size of individual asset renditions and total download size is distorted in the Download dialog.
-->


<!--
* Download Settings configuration to configure asset download from Brand Portal. Fast download, custom renditions, and system renditions are the available configurations. 
-->

<!--
* Document Viewer has been introduced to enhance the PDF viewing experience. New options are available for viewing the PDF files in Brand Portal.

* Advances in the asset download process which improves the Brand Portal user experience while [downloading assets from Brand Portal](brand-portal-download-assets.md). Brand Portal administrators can configure **[!UICONTROL Fast Download]**, **[!UICONTROL Custom Renditions]**, and **[!UICONTROL System Renditions]** from the **[!UICONTROL Download]** settings. 

For details, see [what's new in Brand Portal 6.4.7](whats-new.md). 

### Critical Issues Fixed {#critical-issues-fixed-647}

This release includes fixes to the following critical issues:

* The viewer users are not permitted to share link for collections but the option to share is visible to them on the product interface.

* The **[!UICONTROL Download]** button on the options bar does not list all the licensed assets of the selected folder.

* The search takes longer to show the results for certain keywords.

* The **[!UICONTROL Agree]** and **[!UICONTROL Disagree]** check boxes does not appear on bulk selection of licensed and unlicensed assets during download.

* Filter-based search shows processing on the product interface with no search result. 

* The assets do not download from share link if the shared folder contains numerous and large assets.


### Known Issues {#known-issues-647}

This release includes the following known issues:

* If multiple assets are selected, license text does not appear on clicking Terms and Conditions on the license agreement page during download using share link.   

-->

## Idiomas {#languages}

La interfaz de usuario de Brand Portal está disponible en los siguientes idiomas:

* Inglés
* Alemán
* Francés
* Español
* Italiano
* Portugués de Brasil
* Japonés
* Chino simplificado
* Coreano

## Plataformas certificadas {#certified-platforms}

Para determinar qué plataformas están certificadas para ejecutarse con esta versión de Brand Portal, consulte la columna **Compatibilidad con la IU táctil** en la tabla de la sección **Exploradores admitidos para la interfaz de usuario de creación** de [Requisitos técnicos](https://experienceleague.adobe.com/docs/experience-manager-65/deploying/introduction/technical-requirements.html).

## Vínculos {#links}

* [Página del producto Adobe Experience Manager en adobe.com](https://business.adobe.com/in/products/experience-manager/adobe-experience-manager.html)
* [Documentación de Assets Brand Portal](https://experienceleague.adobe.com/docs/experience-manager-brand-portal/using/home.html)

## Asistencia y acceso al producto (sitios restringidos) {#product-access-and-support-restricted-sites}

Estos sitios solo están disponibles para los clientes. Si es cliente de y requiere acceso, póngase en contacto con su administrador de cuentas de Adobe.

<!--
* [https://daycare.day.com](https://daycare.day.com) 
-->

* [Acceso a productos](https://login.marketing.adobe.com)

* [Asistencia al cliente](https://helpx.adobe.com/contact.html)
