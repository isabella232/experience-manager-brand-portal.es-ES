---
title: Notas de la versión
seo-title: Notas de la versión
description: Obtenga una visión detallada de las funciones, las mejoras, los problemas críticos solucionados y los problemas conocidos de la versión 2020.10.0 de Adobe Experience Manager Assets Brand Portal.
seo-description: Obtenga una visión detallada de las mejoras, los problemas críticos solucionados y los problemas conocidos en la versión 2020.10.0 de Adobe Experience Manager Assets Brand Portal.
uuid: 3d6ffb6f-4608-4e83-8486-5c90e06cdb43
content-type: reference
contentOwner: Vishabh Gupta
topic-tags: brand-portal
products: SG_EXPERIENCEMANAGER/Brand_Portal
discoiquuid: 79ebb9fc-385c-48a8-979e-374f42517988
translation-type: tm+mt
source-git-commit: 8881e9d171c3a4e750a906caadd8aa26f6fc0674
workflow-type: tm+mt
source-wordcount: '544'
ht-degree: 10%

---


# Notas de la versión {#release-notes}

Obtenga una visión detallada de las nuevas funciones, mejoras, problemas importantes solucionados y problemas conocidos de la versión 2020.10.0 de Adobe Experience Manager Assets Brand Portal.

## Información de la versión {#release-information}

| Producto | Adobe Experience Manager Assets Brand Portal |
|---|---|
| Versión | 2020.10.0 |
| Fecha | Octubre de 2020 |

## Información general {#overview}

Adobe Experience Manager (AEM) Assets Brand Portal le ayuda a adquirir, controlar y distribuir de forma segura recursos creativos aprobados a partes externas y usuarios empresariales internos entre dispositivos. Ayuda a mejorar la eficiencia del uso compartido de activos, acelera el tiempo de comercialización de los activos y reduce el riesgo de incumplimiento y acceso no autorizado. Brand Portal permite a los usuarios explorar, buscar, previsualización, descargar y exportar recursos en formatos aprobados por la empresa, en cualquier momento y lugar.

## Novedades de 2020.10.0 {#whats-new-in-2020.10.0}

### New Features {#new-features}

Esta versión incluye las siguientes nuevas funciones:

* El cuadro de diálogo **[!UICONTROL Descargar]** se ha reformado en una vista de lista con opciones adicionales para excluir las representaciones que no son necesarias, aplicar el mismo conjunto de reglas para tipos de recursos similares y descargar las representaciones de recursos seleccionadas.

<!--
* The new **[!UICONTROL Download]** dialog now appears with all the renditions of the selected assets or folders containing assets in a list view, wherein the Brand Portal users can apply same set of renditions for similar asset types and download the selected asset renditions. 
-->

* La navegación a **[!UICONTROL archivos]**, **[!UICONTROL colecciones]** y vínculos **** compartidos ahora es posible desde todas las páginas de Brand Portal con un solo clic.

* El panel **[!UICONTROL Representaciones]** de la página de detalles de recursos ahora permite a los usuarios de Brand Portal seleccionar el recurso original y (o) representaciones de recursos específicas, y descargarlos directamente desde el panel **[!UICONTROL Representaciones]** sin tener que abrir el cuadro de diálogo **[!UICONTROL Descargar]** .

<!--
Brand Portal users can exclude specific renditions which are not required and directly download the original asset and its renditions from the **[!UICONTROL Renditions]** panel on the asset details page. 
-->

* Además de las configuraciones de **[!UICONTROL descarga]** existentes, los administradores de Brand Portal también pueden configurar permisos para que distintos grupos de usuarios realicen vistas y (o) descarguen el recurso original y sus representaciones desde la página de detalles del recurso. Estas configuraciones definirán quién puede acceder a las representaciones de recursos y (o) descargarlas.

### Mejoras {#enhancements}

Esta versión incluye las siguientes mejoras:

* El umbral de tiempo de espera de sesión para los usuarios invitados se ha reducido de 2 horas a 15 minutos.
* La opción de páginas **[!UICONTROL de]** Vista adicionales se ha eliminado para archivos PDF de varias páginas, ya que el usuario puede realizar la vista de las páginas PDF desde el visor de Adobe Document Cloud.


<!--
### Critical Issues Fixed {#critical-issues-fixed}

This release includes fixes to the following critical issue:

* The users are not able to view the PDF pages if the PDF contains sub assets.
-->

### Problemas conocidos {#known-issues}

Esta versión incluye el siguiente problema conocido:

* La búsqueda en los informes **[!UICONTROL de]** recursos muestra el procesamiento en la interfaz del producto sin resultados de búsqueda.
* Las codificaciones de DM de vídeo no son visibles para los usuarios no administradores en la página de detalles de recursos.
* La alineación del tamaño de las representaciones de recursos individuales y el tamaño total de descarga se distorsiona en el cuadro de diálogo Descargar.



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

Para determinar qué plataformas están certificadas para ejecutarse con esta versión de Brand Portal, consulte la columna **Asistencia para la IU** táctil en la tabla de la sección Exploradores **admitidos para la interfaz** de usuario de creación de Requisitos [](https://helpx.adobe.com/experience-manager/6-4/sites/deploying/using/technical-requirements.html)técnicos.

## Vínculos {#links}

* [Página del producto Adobe Experience Manager en adobe.com](http://www.adobe.com/in/marketing-cloud/experience-manager.html)
* [Documentación de Assets Brand Portal](https://helpx.adobe.com/es/experience-manager/brand-portal/user-guide.html)

## Asistencia y acceso al producto (sitios restringidos) {#product-access-and-support-restricted-sites}

Estos sitios solo están disponibles para los clientes. Si es cliente y necesita acceso, póngase en contacto con el administrador de cuentas de Adobe.

* [https://daycare.day.com](https://daycare.day.com)

* [Acceso a productos](https://login.marketing.adobe.com)

* [Servicio de atención al cliente de Adobe](https://helpx.adobe.com/contact.html)
