---
title: Notas de la versión
seo-title: Notas de la versión
description: Obtenga una visión detallada de las funciones, las mejoras, los problemas críticos solucionados y los problemas conocidos de la versión 2021.02.0 de Adobe Experience Manager Assets Brand Portal.
seo-description: Obtenga una visión detallada de las mejoras, los problemas críticos solucionados y los problemas conocidos en la versión 2021.02.0 de Adobe Experience Manager Assets Brand Portal.
uuid: 3d6ffb6f-4608-4e83-8486-5c90e06cdb43
content-type: reference
contentOwner: Vishabh Gupta
topic-tags: brand-portal
products: SG_EXPERIENCEMANAGER/Brand_Portal
discoiquuid: 79ebb9fc-385c-48a8-979e-374f42517988
translation-type: tm+mt
source-git-commit: 69cf1756a546355ed767ac13c51fb09932254dbc
workflow-type: tm+mt
source-wordcount: '515'
ht-degree: 11%

---


# Notas de la versión {#release-notes}

Obtenga una visión detallada de las nuevas funciones, mejoras, problemas importantes solucionados y problemas conocidos de la versión 2021.02.0 de Adobe Experience Manager Assets Brand Portal.

## Información de la versión {#release-information}

| Producto | Adobe Experience Manager Assets Brand Portal |
|---|---|
| Versión | 2021.02.0 |
| Fecha | Febrero de 2021 |

## Información general {#overview}

Adobe Experience Manager (AEM) Assets Brand Portal le ayuda a adquirir, controlar y distribuir de forma segura recursos creativos aprobados a partes externas y usuarios empresariales internos entre dispositivos. Ayuda a mejorar la eficiencia del uso compartido de activos, acelera el tiempo de comercialización de los activos y reduce el riesgo de incumplimiento y acceso no autorizado. Brand Portal permite a los usuarios explorar, buscar, previsualización, descargar y exportar recursos en formatos aprobados por la empresa, en cualquier momento y lugar.

## Novedades de 2021.02.0 {#whats-new-in-2021.02.0}

### Nuevas funciones {#new-features}

Esta versión incluye las siguientes nuevas funciones:

* Se ha introducido una configuración adicional de **[!UICONTROL descarga de recursos]** en **[!UICONTROL configuración de descarga]**. Crea una carpeta independiente para cada recurso mientras descarga las carpetas, las colecciones o la descarga masiva de recursos. Consulte [configuración de descarga](https://docs.adobe.com/content/help/en/experience-manager-brand-portal/using/download/brand-portal-download-assets.html#configure-download).

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

Esta versión incluye las siguientes mejoras:

* Para la descarga de carpetas, se crea una carpeta independiente para cada recurso mediante un vínculo compartido, independientemente de la **[!UICONTROL configuración de descarga]**.
* El informe de uso de Brand Portal **** se ha modificado para reflejar únicamente los usuarios activos de Brand Portal.

<!--
* The threshold of session timeout for the guest users has been reduced from 2 hours to 15 minutes.
* The additional **[!UICONTROL View pages]** option has been removed for multi-page PDFs as the user can now view the PDF pages from the Adobe Document Cloud Viewer.
-->


### Problemas críticos solucionados {#critical-issues-fixed}

Esta versión incluye correcciones a los siguientes problemas críticos:

* Si solo se descargan los recursos originales, el recurso refleja su propia extensión y no se abre hasta que la extensión se cambia manualmente a zip.
* La interfaz de usuario de la carpeta de recopilación no responde al hacer clic en la flecha de navegación.
* **[!UICONTROL El botón]** Crear está visible en la  **** vista de columnas aunque las carpetas estén vacías.
* **[!UICONTROL La]** búsqueda de Omni falla con un mensaje de error 414 (Solicitar-URI demasiado largo) si se omite el despachante al acceder a la instancia de Brand Portal.
* Se descarga una carpeta zip vacía si el recurso contiene una coma (`,`) en el nombre del archivo.
* Los usuarios del visor obtienen la opción de agregar usuarios a la colección que han creado.
* Se produce un comportamiento incoherente cuando un recurso (miniatura o representación web) se descarga mediante un vínculo compartido.

Consulte [novedades en Brand Portal 2021.02.0](whats-new.md).

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

Para determinar qué plataformas están certificadas para ejecutarse con esta versión de Brand Portal, consulte la columna **Compatibilidad con IU táctil** de la tabla de la sección **Exploradores admitidos para la creación de la interfaz de usuario** de [Requisitos técnicos](https://helpx.adobe.com/experience-manager/6-4/sites/deploying/using/technical-requirements.html).

## Vínculos {#links}

* [Página del producto Adobe Experience Manager en adobe.com](http://www.adobe.com/in/marketing-cloud/experience-manager.html)
* [Documentación de Assets Brand Portal](https://helpx.adobe.com/es/experience-manager/brand-portal/user-guide.html)

## Asistencia y acceso al producto (sitios restringidos) {#product-access-and-support-restricted-sites}

Estos sitios solo están disponibles para los clientes. Si es cliente y necesita acceso, póngase en contacto con el administrador de cuentas de Adobe.

<!--
* [https://daycare.day.com](https://daycare.day.com) 
-->

* [Acceso a productos](https://login.marketing.adobe.com)

* [Servicio de atención al cliente de Adobe](https://helpx.adobe.com/contact.html)
