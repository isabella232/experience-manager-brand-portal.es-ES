---
title: Publicar ajustes preestablecidos, esquemas y facetas en Brand Portal
seo-title: Publicar ajustes preestablecidos, esquemas y facetas en Brand Portal
description: Descubra cómo publicar ajustes preestablecidos, esquemas y facetas en Brand Portal.
seo-description: Descubra cómo publicar ajustes preestablecidos, esquemas y facetas en Brand Portal.
uuid: c836d9bb-074a-4113-9c91-b2bf7658b88d
topic-tags: publicación
products: SG_EXPERIENCEMANAGER/Brand_Portal
content-type: referencia
discoiquuid: bc305abc-9373-4d33-9179-0a5f3904b352
translation-type: tm+mt
source-git-commit: 5a4d31622a5dee95045ee377e07c0c53f982aad3

---


# Publicar ajustes preestablecidos, esquemas y facetas en Brand Portal {#publish-presets-schema-and-facets-to-brand-portal}

El artículo profundiza en la publicación de ajustes preestablecidos de imagen, esquemas de metadatos y facetas de búsqueda personalizadas desde la instancia de AEM Author hasta Brand Portal. La capacidad de publicación permite a las organizaciones reutilizar los ajustes preestablecidos de imagen, esquemas de metadatos y facetas de búsqueda creados/modificados en la instancia de AEM Author, reduciendo así los esfuerzos duplicados.

>[!NOTE]
>
>La capacidad de publicar ajustes preestablecidos de imagen, esquemas de metadatos y facetas de búsqueda de la instancia de AEM Author en Brand Portal está disponible para AEM 6.2 SP1-CFP7 y AEM 6.3 SP 1-CFP 1 (6.3.1.1) en adelante.

## Publicación de ajustes preestablecidos de imagen en Brand Portal {#publish-image-presets-to-brand-portal}

Los ajustes preestablecidos de imagen son un conjunto de comandos de tamaño y formato que se aplican a la imagen en el momento de la publicación de la imagen. Los ajustes preestablecidos de imagen se pueden crear y modificar en Brand Portal. Como alternativa, si la instancia de AEM Author se está ejecutando en modo de medios dinámicos, los usuarios pueden crear ajustes preestablecidos en AEM Author y publicarlos en AEM Assets Brand Portal, y evitar volver a crear los mismos ajustes preestablecidos en Brand Portal.\
Una vez creado el ajuste preestablecido, se muestra como representación dinámica en el carril de representaciones de detalles de recursos y en el cuadro de diálogo de descarga.

>[!NOTE]
>
>Si la instancia de AEM Author no se está ejecutando en el modo [!UICONTROL de medios] dinámicos (el cliente no ha adquirido Dynamic Media), la representación TIFF [!UICONTROL de] pirámide de los recursos no se crea en el momento de la carga. Los ajustes preestablecidos de imagen o las representaciones dinámicas funcionan en el TIFF [!UICONTROL de] pirámide de un recurso, por lo que si el TIFF [!UICONTROL de] pirámide no está disponible en la instancia de AEM Author, tampoco estará disponible en Brand Portal. Como resultado, no hay representaciones dinámicas presentes en el carril de representaciones de la página de detalles de recursos ni en el cuadro de diálogo de descarga.

Para publicar ajustes preestablecidos de imagen en Brand Portal:

1. En la instancia de AEM Author, toque o haga clic en el logotipo de AEM para acceder a la consola de navegación global y toque o haga clic en el icono Herramientas y vaya a **[!UICONTROL Recursos &gt; Ajustes preestablecidos]** de imagen.
1. Seleccione el ajuste preestablecido de imagen o varios ajustes preestablecidos de imagen en la lista de ajustes preestablecidos de imagen y toque o haga clic en **[!UICONTROL Publicar en Brand Portal]**.

![](assets/publishpreset.png)

>[!NOTE]
>
>Cuando los usuarios hacen clic en **[!UICONTROL Publicar en Brand Portal]** , los ajustes preestablecidos de imagen se ponen en cola para su publicación. Se recomienda a los usuarios que supervisen el registro de los agentes de replicación para confirmar si la publicación se ha realizado correctamente.

Para cancelar la publicación de un ajuste preestablecido de imagen desde Brand Portal:

1. En la instancia de AEM Author, toque o haga clic en el logotipo de AEM para acceder a la consola de navegación global y toque o haga clic en el icono **[!UICONTROL Herramientas]** y vaya a **[!UICONTROL Recursos &gt; Ajustes preestablecidos]** de imagen.
1. Seleccione un ajuste preestablecido de imagen y seleccione **[!UICONTROL Quitar de Brand Portal]** en las opciones disponibles en la parte superior.

## Publicar esquema de metadatos en Brand Portal {#publish-metadata-schema-to-brand-portal}

El esquema de metadatos describe el diseño y las propiedades que se muestran en la página de propiedades de los recursos o las colecciones.

![](assets/metadata-schema-editor.png) ![](assets/asset-properties-1.png)

Si los usuarios han editado el esquema predeterminado en la instancia de AEM Author y están dispuestos a usar el mismo esquema que el esquema predeterminado en Brand Portal, simplemente pueden publicar los formularios de esquema de metadatos en Brand Portal. En este caso, los esquemas predeterminados publicados desde la instancia de AEM Author anulan el esquema predeterminado de Brand Portal.

Si los usuarios han creado un esquema personalizado en la instancia de AEM Author, pueden publicar el esquema personalizado en Brand Portal en lugar de volver a crear allí el mismo esquema personalizado. Los usuarios pueden aplicar este esquema personalizado a cualquier carpeta o colección de Brand Portal.

>[!NOTE]
>
>Los esquemas predeterminados no se pueden publicar en Brand Portal si están bloqueados en la instancia de AEM (es decir, no se han editado).

![](assets/default-schema-form.png)

>[!NOTE]
>
>Si una carpeta tiene un esquema aplicado en la instancia de AEM Author, también debe existir el mismo esquema en Brand Portal para mantener la coherencia en la página de propiedades de recursos de AEM Author y Brand Portal.

Para publicar un esquema de metadatos de la instancia de AEM Author en Brand Portal:

1. En la instancia de AEM Author, toque o haga clic en el logotipo de AEM para acceder a la consola de navegación global y toque o haga clic en el icono Herramientas y vaya a **[!UICONTROL Recursos &gt; Esquemas]** de metadatos.
1. Seleccione un esquema de metadatos y seleccione **[!UICONTROL Publicar en Brand Portal]** en las opciones disponibles en la parte superior.

>[!NOTE]
>
>Cuando los usuarios hacen clic en **[!UICONTROL Publicar en Brand Portal]**, los esquemas de metadatos se ponen en cola para su publicación. Se recomienda a los usuarios que supervisen el registro de los agentes de replicación para confirmar si la publicación se ha realizado correctamente.

Para cancelar la publicación de un esquema de metadatos desde Brand Portal:

1. En la instancia de AEM Author, toque o haga clic en el logotipo de AEM para acceder a la consola de navegación global y toque o haga clic en el icono Herramientas y vaya a **[!UICONTROL Recursos &gt; Esquemas]** de metadatos.
1. Seleccione un esquema de metadatos y seleccione **[!UICONTROL Quitar de Brand Portal]** de las opciones disponibles en la parte superior.

## Publicación de facetas de búsqueda en Brand Portal {#publish-search-facets-to-brand-portal}

Los formularios de búsqueda proporcionan a los usuarios la capacidad de buscar [por](../using/brand-portal-search-facets.md) facetas en Brand Portal. Las facetas de búsqueda proporcionan mayor granularidad a las búsquedas en Brand Portal. Todos los [predicados agregados](https://helpx.adobe.com/experience-manager/6-5/assets/using/search-facets.html#AddingaPredicate) en el formulario de búsqueda están disponibles para los usuarios como facetas de búsqueda en los filtros de búsqueda.

![](assets/property-predicate-removed.png)
![](assets/search-form.png)

Si desea utilizar el formulario de búsqueda personalizado **[!UICONTROL Recursos Administración Raíl]** de búsqueda de la instancia de AEM Author, en lugar de volver a crear el mismo formulario en Brand Portal, puede publicar el formulario de búsqueda personalizado de la instancia de AEM Author en Brand Portal.

>[!NOTE]
>
>El formulario de búsqueda bloqueada **[!UICONTROL Recursos Administración Raíz]** de búsqueda en Recursos AEM no se puede publicar en Brand Portal a menos que se edite. Una vez editado y publicado en Brand Portal, este formulario de búsqueda sobrescribe el formulario de búsqueda en Brand Portal.

Para publicar la faceta de búsqueda editada de la instancia de AEM Author en Brand Portal:

1. Toque o haga clic en el logotipo de AEM y, a continuación, vaya a **[!UICONTROL Herramientas &gt; General &gt; Buscar formularios]**.
1. Seleccione el formulario de búsqueda editado y seleccione **[!UICONTROL Publicar en Brand Portal]**.

   >[!NOTE]
   >
   >Cuando los usuarios hacen clic en **[!UICONTROL Publicar en Brand Portal]**, las facetas de búsqueda se ponen en cola para su publicación. Se recomienda a los usuarios que supervisen el registro de los agentes de replicación para confirmar si la publicación se ha realizado correctamente.

Para cancelar la publicación de formularios de búsqueda desde Brand Portal:

1. En la instancia de AEM Author, toque o haga clic en el logotipo de AEM para acceder a la consola de navegación global y toque o haga clic en el icono Herramientas y vaya a **[!UICONTROL General &gt; Buscar formularios]**.
1. Seleccione el formulario de búsqueda y seleccione **[!UICONTROL Quitar de Brand Portal]** en las opciones disponibles en la parte superior.

>[!NOTE]
>
>La acción **[!UICONTROL Cancelar publicación de Brand Portal]** deja el formulario de búsqueda predeterminado en Brand Portal y no restaura el último formulario de búsqueda utilizado antes de la publicación.

### Restricciones {#limitations}

1. Pocos predicados de búsqueda no son aplicables a los filtros de búsqueda en Brand Portal. Cuando estos predicados de búsqueda se publican como parte del formulario de búsqueda desde la instancia de AEM Author hasta Brand Portal, se filtran. Por lo tanto, los usuarios ven menos predicados en el formulario publicado en Brand Portal. Consulte los predicados [de búsqueda aplicables a los filtros en Brand Portal](../using/brand-portal-search-facets.md#list-of-search-predicates).

1. En Predicado [!UICONTROL de]opciones, si un usuario está utilizando una ruta personalizada para leer opciones en la instancia de AEM Author, no funcionará en el portal de marcas. Estas rutas y opciones adicionales no se publican en Brand Portal con el formulario de búsqueda. En este caso, los usuarios pueden seleccionar la opción **[!UICONTROL Manual]** en **[!UICONTROL Agregar opciones]** en Predicado **[!UICONTROL de]** opciones para agregar estas opciones manualmente en Brand Portal.

![](assets/options-predicate-manual.png)
