---
title: Publicar ajustes preestablecidos, esquemas y facetas en Brand Portal
seo-title: Publish presets, schema, and facets to Brand Portal
description: Aprenda a publicar ajustes preestablecidos, esquema y facetas en Brand portal.
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

El artículo profundiza en la publicación de ajustes preestablecidos de imagen, esquemas de metadatos y facetas de búsqueda personalizadas de AEM Autor instancia en Brand portal. Publicación capacidad permite a las organizaciones reutilizar los ajustes preestablecidos de imagen, los esquemas de metadatos y las facetas de búsqueda creadas/modificadas en AEM Autor instancia, por lo tanto, reducir duplicado esfuerzos.

>[!NOTE]
>
>La capacidad de publicar ajustes preestablecidos de imagen, metadatos esquema y búsqueda facetas de AEM Autor instancia a Brand portal está disponible AEM 6,2 SP1-CFP7 y AEM 6,3 SP 1-PPC 1 (6.3.1.1) en adelante.

## Publish ajustes preestablecidos de imagen en Brand portal {#publish-image-presets-to-brand-portal}

Imagen ajustes preestablecidos son un conjunto de comandos de tamaño y formato que se aplican a la imagen en el momento de la imagen envío. Imagen ajustes preestablecidos se pueden crear y modificar en Brand portal. De forma alternativa, si AEM Autor instancia se ejecuta en modo medios dinámicos, los usuarios pueden crear ajustes preestablecidos en la AEM autor y publicar en Recursos AEM portal de marca y evitar volver a crear los mismos ajustes preestablecidos en el portal de marca.\
Una vez creado el ajuste preestablecido, se muestra como representación dinámico en recurso representaciones de detalle carril y descargar cuadro de diálogo.

>[!NOTE]
>
>Si AEM Autor instancia no se ejecuta en **[!UICONTROL el modo]** Dynamic media (el cliente no ha comprado Dynamic media), entonces el **[!UICONTROL representación de TIFF]**  piramidal del activos no se crea en el momento de la cargar. Imagen ajustes preestablecidos o representaciones dinámicas funcionan en **[!UICONTROL formato TIFF]** piramidal de un recurso, por lo tanto, si **[!UICONTROL el formato]** piramidal no está disponible en AEM autor instancia entonces no está disponible en Brand portal. Como resultado, no hay ninguna representación dinámica presente en las representaciones carril de recurso detalles Página y descargar cuadro de diálogo.

Para publicar ajustes preestablecidos de imagen en Brand Portal:

1. En AEM Autor instancia, toque o haga clic en el logotipo AEM para acceder a la consola de navegación global y pulse o haga clic en el icono Herramientas y desplácese hasta **[!UICONTROL assets > Imagen ajustes preestablecidos]** .
1. Seleccione el ajuste preestablecido de imagen o varios ajustes preestablecidos de imagen de la lista de ajustes preestablecidos de imagen y pulse o haga clic en **[!UICONTROL Publicar en Brand Portal]**.

![](assets/publishpreset.png)

>[!NOTE]
>
>Cuando los usuarios hacen clic en **[!UICONTROL Publish a Brand portal]** , los ajustes preestablecidos de imagen se ponen en cola para su publicación. Se recomienda a los usuarios monitor el registro de los agentes de replicación para confirmar si la publicar fue satisfactoria.

Para cancelar la publicación de un ajuste preestablecido de imagen de Brand Portal:

1. En AEM Autor instancia, toque o haga clic en el logotipo AEM para acceder a la consola de navegación global y pulse o haga clic en el **[!UICONTROL icono herramientas]** y desplácese hasta **[!UICONTROL Assets > imagen ajustes preestablecidos]** .
1. Seleccione un ajuste preestablecido de imagen y seleccione **[!UICONTROL quitar de Brand portal]** de las opciones disponibles en la parte superior.

## Publish metadatos esquema a Brand portal  {#publish-metadata-schema-to-brand-portal}

Metadatos esquema describe el diseño y las propiedades que se muestran en las Página de propiedades de recurso/colecciones.

![](assets/metadata-schema-editor.png) ![](assets/asset-properties-1.png)

Si los usuarios han editado la esquema predeterminada en AEM Autor instancia y están dispuestos a utilizar el mismo esquema que el valor predeterminado esquema en el portal de marca, puede simplemente publicar la metadatos esquema formularios a Brand portal. En tal caso, el esquema predeterminado de Brand portal es sustituido por los esquemas predeterminados publicados en AEM Autor instancia.

Si los usuarios han creado un esquema personalizado en AEM Autor instancia, pueden publicar el esquema personalizado a Brand portal en lugar de volver a crear los mismos esquema personalizados. A continuación, los usuarios pueden aplicar esta esquema personalizada a cualquier carpeta/colección en Brand portal.

>[!NOTE]
>
>Los esquemas predeterminados no se pueden publicar en Brand portal si están bloqueados en el AEM instancia (es decir, no se editan).

![](assets/default-schema-form.png)

>[!NOTE]
>
>Si una carpeta tiene una esquema aplicada en AEM Autor instancia, el mismo esquema debe existir también en el portal de marca para mantener la coherencia en el recurso propiedades página en AEM Autor y en el portal de marca.

Para publicar un metadatos esquema de AEM Autor instancia al portal de marca:

1. En AEM Autor instancia, toque o haga clic en el logotipo AEM para acceder a la consola de navegación global y pulse o haga clic en el icono Herramientas y desplácese hasta Assets esquemas ]**de**[!UICONTROL  metadatos de >.
1. Seleccione un esquema de metadatos y seleccione **[!UICONTROL Publish en Brand portal]** de las opciones disponibles en la parte superior.

>[!NOTE]
>
>Cuando los usuarios hacen clic en **[!UICONTROL Publish a Brand portal]** , los esquemas de metadatos se ponen en cola para su publicación. Se recomienda a los usuarios monitor el registro de los agentes de replicación para confirmar si la publicar fue satisfactoria.

Para cancelar la publicación de una metadatos esquema de Brand Portal:

1. En AEM Autor instancia, toque o haga clic en el logotipo AEM para acceder a la consola de navegación global y pulse o haga clic en el icono Herramientas y desplácese hasta Assets esquemas ]**de**[!UICONTROL  metadatos de >.
1. Seleccione un esquema de metadatos y seleccione **[!UICONTROL quitar de Brand portal]** de las opciones disponibles en la parte superior.

## Publicar facetas de búsqueda en Brand Portal {#publish-search-facets-to-brand-portal}

Los formularios de búsqueda proporcionan la capacidad de [búsqueda con facetas](../using/brand-portal-search-facets.md) a usuarios en Brand Portal. Las facetas de búsqueda proporcionan la buena granularidad a las búsquedas en Brand Portal. Todos los [predicados añadidos](https://experienceleague.adobe.com/docs/experience-manager-65/assets/administer/search-facets.html) en el formulario de búsqueda están disponibles para los usuarios como facetas de búsqueda en los filtros de búsqueda.

![](assets/property-predicate-removed.png)
![](assets/search-form.png)

Si desea utilizar el búsqueda **[!UICONTROL personalizado assets carril]** Search de administración de la AEM autor instancia, en lugar de volver a crear el mismo formulario en el portal de marca, puede publicar el formulario de búsqueda personalizado de AEM autor instancia a Brand portal.

>[!NOTE]
>
>Se bloqueó búsqueda formulario **[!UICONTROL assets el carril]** Search de administración en recursos AEM no se puede publicar en Brand portal a menos que se edite. Una vez editada y publicada en Brand portal, este búsqueda formulario anula el formulario búsqueda en Brand portal.

Para publicar el aspecto búsqueda editado de AEM Autor instancia en el portal de marca:

1. Pulse o haga clic en el logotipo de AEM y, a continuación, vaya a **[!UICONTROL Herramientas > General > Buscar formularios]**.
1. Seleccione el formulario de búsqueda editado y seleccione **[!UICONTROL Publish en Brand portal]** .

   >[!NOTE]
   >
   >Cuando los usuarios hacen clic en **[!UICONTROL Publish a Brand portal]** , las facetas de búsqueda se ponen en cola para su publicación. Se recomienda a los usuarios monitor el registro de los agentes de replicación para confirmar si la publicar fue satisfactoria.

Para cancelar la publicación de búsqueda Forms de Brand Portal:

1. En AEM Autor instancia, toque o haga clic en el logotipo AEM para acceder a la consola de navegación global y pulse o haga clic en el icono Herramientas y desplácese a **[!UICONTROL >]** General Search Forms.
1. Seleccione el formulario búsqueda y seleccione **[!UICONTROL quitar de Brand portal]** de las opciones disponibles en la parte superior.

>[!NOTE]
>
>La **[!UICONTROL acción cancelar la publicación de Brand portal]** deja el formulario de búsqueda predeterminado en el portal de marca y no se restaura al último búsqueda formulario utilizado antes de la publicación.

### Restricciones {#limitations}

1. Algunos predicados de búsqueda no se aplican a búsqueda filtros en Brand portal. Cuando estos predicados de búsqueda se publican como parte del formulario búsqueda de AEM Autor instancia en Brand portal, se filtran. Los usuarios, por lo tanto, ven menos de un número de predicados en el formulario publicado en el portal de marca. Consulte [ predicados de búsqueda aplicables a filtros en el portal ](../using/brand-portal-search-facets.md#list-of-search-predicates) de marca.

1. Para [!UICONTROL Predicado de opciones]Sin embargo, si un usuario utiliza cualquier ruta personalizada para leer opciones en la instancia de autor de AEM, no funcionará en la instancia de Brand Portal. Estas rutas y opciones adicionales no se publican en Brand Portal con el formulario de búsqueda. En este caso, los usuarios pueden seleccionar la variable **[!UICONTROL Manual]** opción en **[!UICONTROL Agregar opciones]** dentro **[!UICONTROL Predicado de opciones]** para añadir estas opciones manualmente en Brand Portal.

![](assets/options-predicate-manual.png)
