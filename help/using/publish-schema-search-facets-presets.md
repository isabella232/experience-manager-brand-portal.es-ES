---
title: Publicar ajustes preestablecidos, esquemas y facetas en Brand Portal
seo-title: Publish presets, schema, and facets to Brand Portal
description: Aprenda a publicar ajustes preestablecidos, esquemas y facetas en Brand Portal.
seo-description: Learn how to publish presets, schema, and facets to Brand Portal.
uuid: c836d9bb-074a-4113-9c91-b2bf7658b88d
topic-tags: publish
products: SG_EXPERIENCEMANAGER/Brand_Portal
content-type: reference
discoiquuid: bc305abc-9373-4d33-9179-0a5f3904b352
exl-id: 9b585606-6538-459b-87a9-2e68df0087b3
source-git-commit: 4caa4263bd74b51af7504295161c421524e51f0c
workflow-type: tm+mt
source-wordcount: '1141'
ht-degree: 2%

---

# Publicar ajustes preestablecidos, esquemas y facetas en Brand Portal {#publish-presets-schema-and-facets-to-brand-portal}

El artículo profundiza en la publicación de ajustes preestablecidos de imagen, esquemas de metadatos y facetas de búsqueda personalizadas desde la instancia de autor de AEM a Brand Portal. La capacidad de publicación permite a las organizaciones reutilizar los ajustes preestablecidos de imagen, los esquemas de metadatos y las facetas de búsqueda creadas o modificadas en la instancia de AEM Author, lo que reduce los esfuerzos duplicados.

>[!NOTE]
>
>La capacidad para publicar ajustes preestablecidos de imagen, esquemas de metadatos y facetas de búsqueda de la instancia de AEM Author a Brand Portal está disponible AEM 6.2 SP1-CFP7 y AEM 6.3 SP 1-CFP 1 (6.3.1.1) en adelante.

## Publicar ajustes preestablecidos de imagen en Brand Portal {#publish-image-presets-to-brand-portal}

Los ajustes preestablecidos de imagen son un conjunto de comandos de tamaño y formato que se aplican a la imagen en el momento de la entrega de la imagen. Los ajustes preestablecidos de imagen se pueden crear y modificar en Brand Portal. Alternativamente, si la instancia de AEM Author se está ejecutando en modo de Dynamic Media, los usuarios pueden crear ajustes preestablecidos en AEM Author y publicarlos en AEM Assets Brand Portal, y evitar volver a crear los mismos ajustes preestablecidos en Brand Portal.\
Una vez creado el ajuste preestablecido, aparece como representación dinámica en el carril representaciones de detalles de recursos y en el cuadro de diálogo de descarga.

>[!NOTE]
>
>Si la instancia de autor de AEM no se está ejecutando en **[!UICONTROL Dynamic Media Mode]** (el cliente no ha comprado Dynamic Media), la **[!UICONTROL representación de TIFF pirámide]** de los recursos no se crea en el momento de la carga. Los ajustes preestablecidos de imagen o las representaciones dinámicas funcionan en **[!UICONTROL TIFF piramidal]** de un recurso, por lo que si **[!UICONTROL TIFF piramidal]** no está disponible en la instancia de AEM Author, tampoco está disponible en Brand Portal. Como resultado, no hay representaciones dinámicas presentes en el carril de representaciones de la página de detalles del recurso y en el cuadro de diálogo de descarga.

Para publicar ajustes preestablecidos de imagen en Brand Portal:

1. En la instancia de autor de AEM, pulse o haga clic en el logotipo de AEM para acceder a la consola de navegación global, pulse o haga clic en el icono Herramientas y vaya a **[!UICONTROL Assets > Ajustes preestablecidos de imagen]**.
1. Seleccione el ajuste preestablecido de imagen o varios ajustes preestablecidos de imagen en la lista de ajustes preestablecidos de imagen y pulse o haga clic en **[!UICONTROL Publicar en Brand Portal]**.

![](assets/publishpreset.png)

>[!NOTE]
>
>Cuando los usuarios hacen clic en **[!UICONTROL Publicar en Brand Portal]**, los ajustes preestablecidos de imagen se ponen en cola para su publicación. Se recomienda a los usuarios que controlen el registro de los agentes de replicación para confirmar si la publicación se ha realizado correctamente.

Para cancelar la publicación de un ajuste preestablecido de imagen desde Brand Portal:

1. En la instancia de autor de AEM, pulse o haga clic en el logotipo de AEM para acceder a la consola de navegación global, pulse o haga clic en el icono **[!UICONTROL Herramientas]** y vaya a **[!UICONTROL Assets > Ajustes preestablecidos de imagen]**.
1. Seleccione un ajuste preestablecido de imagen y seleccione **[!UICONTROL Quitar de Brand Portal]** en las opciones disponibles en la parte superior.

## Publicar esquema de metadatos en Brand Portal  {#publish-metadata-schema-to-brand-portal}

El esquema de metadatos describe el diseño y las propiedades que se muestran en la página de propiedades de los recursos o las colecciones.

![](assets/metadata-schema-editor.png) ![](assets/asset-properties-1.png)

Si los usuarios han editado el esquema predeterminado en la instancia de AEM Author y están dispuestos a utilizar el mismo esquema como esquema predeterminado en Brand Portal, simplemente pueden publicar los formularios de esquema de metadatos en Brand Portal. En tal caso, el esquema predeterminado en Brand Portal se sobrescribe por los esquemas predeterminados publicados desde la instancia de autor de AEM.

Si los usuarios han creado un esquema personalizado en la instancia de autor de AEM, pueden publicar el esquema personalizado en Brand Portal en lugar de volver a crear allí el mismo esquema personalizado. Los usuarios pueden aplicar este esquema personalizado a cualquier carpeta o colección de Brand Portal.

>[!NOTE]
>
>Los esquemas predeterminados no se pueden publicar en Brand Portal si están bloqueados en la instancia de AEM (es decir, no se han editado).

![](assets/default-schema-form.png)

>[!NOTE]
>
>Si una carpeta tiene un esquema aplicado en la instancia de AEM Author, también debe existir el mismo esquema en Brand Portal para mantener la coherencia en la página de propiedades de recursos de AEM Author y Brand Portal.

Para publicar un esquema de metadatos de la instancia de AEM Author en Brand Portal:

1. En la instancia de autor de AEM, pulse o haga clic en el logotipo de AEM para acceder a la consola de navegación global, pulse o haga clic en el icono Herramientas y vaya a **[!UICONTROL Assets > Esquemas de metadatos]**.
1. Seleccione un esquema de metadatos y seleccione **[!UICONTROL Publish to Brand Portal]** en las opciones disponibles en la parte superior.

>[!NOTE]
>
>Cuando los usuarios hacen clic en **[!UICONTROL Publicar en Brand Portal]**, los esquemas de metadatos se ponen en cola para su publicación. Se recomienda a los usuarios que controlen el registro de los agentes de replicación para confirmar si la publicación se ha realizado correctamente.

Para cancelar la publicación de un esquema de metadatos de Brand Portal:

1. En la instancia de autor de AEM, pulse o haga clic en el logotipo de AEM para acceder a la consola de navegación global, pulse o haga clic en el icono Herramientas y vaya a **[!UICONTROL Assets > Esquemas de metadatos]**.
1. Seleccione un esquema de metadatos y seleccione **[!UICONTROL Quitar de Brand Portal]** en las opciones disponibles en la parte superior.

## Publicar facetas de búsqueda en Brand Portal {#publish-search-facets-to-brand-portal}

Los formularios de búsqueda ofrecen la capacidad de [búsqueda faceteada](../using/brand-portal-search-facets.md) a los usuarios de Brand Portal. Las facetas de búsqueda proporcionan buena granularidad para las búsquedas en Brand Portal. Todos los [predicados añadidos](https://experienceleague.adobe.com/docs/experience-manager-65/assets/administer/search-facets.html) en el formulario de búsqueda están disponibles para los usuarios como facetas de búsqueda en los filtros de búsqueda.

![](assets/property-predicate-removed.png)
![](assets/search-form.png)

Si desea utilizar el formulario de búsqueda personalizada **[!UICONTROL Carril de búsqueda de administración de Assets]** de la instancia de autor de AEM, en lugar de volver a crear el mismo formulario en Brand Portal, puede publicar el formulario de búsqueda personalizado de la instancia de autor de AEM en Brand Portal.

>[!NOTE]
>
>El formulario de búsqueda bloqueado **[!UICONTROL Carril de búsqueda de administración de Assets]** en AEM Assets no se puede publicar en Brand Portal a menos que se edite. Una vez editado y publicado en Brand Portal, este formulario de búsqueda anula el formulario de búsqueda en Brand Portal.

Para publicar la faceta de búsqueda editada de la instancia de AEM Author en Brand Portal:

1. Pulse o haga clic en el logotipo de AEM y, a continuación, vaya a **[!UICONTROL Herramientas > General > Buscar formularios]**.
1. Seleccione el formulario de búsqueda editado y seleccione **[!UICONTROL Publicar en Brand Portal]**.

   >[!NOTE]
   >
   >Cuando los usuarios hacen clic en **[!UICONTROL Publicar en Brand Portal]**, las facetas de búsqueda se ponen en cola para su publicación. Se recomienda a los usuarios que controlen el registro de los agentes de replicación para confirmar si la publicación se ha realizado correctamente.

Para cancelar la publicación de formularios de búsqueda desde Brand Portal:

1. En la instancia de autor de AEM, pulse o haga clic en el logotipo de AEM para acceder a la consola de navegación global, pulse o haga clic en el icono Herramientas y vaya a **[!UICONTROL General > Buscar en Forms]**.
1. Seleccione el formulario de búsqueda y seleccione **[!UICONTROL Quitar de Brand Portal]** en las opciones disponibles en la parte superior.

>[!NOTE]
>
>La acción **[!UICONTROL Cancelar publicación de Brand Portal]** deja el formulario de búsqueda predeterminado en Brand Portal y no restaura al último formulario de búsqueda utilizado antes de la publicación.

### Restricciones     {#limitations}

1. Pocos predicados de búsqueda no son aplicables a los filtros de búsqueda en Brand Portal. Cuando estos predicados de búsqueda se publican como parte del formulario de búsqueda de la instancia de autor de AEM a Brand Portal, se filtran. Por lo tanto, los usuarios ven menos predicados en el formulario publicado en Brand Portal. Consulte [predicados de búsqueda aplicables a los filtros de Brand Portal](../using/brand-portal-search-facets.md#list-of-search-predicates).

1. En el caso del [!UICONTROL predicado de opciones], si un usuario está utilizando una ruta personalizada para leer las opciones en la instancia de autor de AEM, no funcionará en Brand Portal. Estas rutas y opciones adicionales no se publican en Brand Portal con el formulario de búsqueda. En este caso, los usuarios pueden seleccionar la opción **[!UICONTROL Manual]** en **[!UICONTROL Agregar opciones]** dentro del **[!UICONTROL Predicado de opciones]** para agregar estas opciones manualmente en Brand Portal.

![](assets/options-predicate-manual.png)
