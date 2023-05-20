---
title: Buscar recursos en Brand Portal
seo-title: Asset searching and saved search on Experience Manager Assets Brand Portal
description: La capacidad de búsqueda de Brand portal le permite búsqueda rápidamente la activos relevante mediante omnisearch y búsqueda filtros ayudarle a reducir aún más su búsqueda. Guardar las búsquedas como colecciones inteligentes para el futuro.
seo-description: Brand Portal search capability lets you quickly search for relevant assets using omnisearch, and search filters help you further narrow down your search. Save your searches as smart collections for future.
uuid: c2955198-bdc0-4853-a13a-661e6a9ec61f
contentOwner: bdhar
content-type: reference
products: SG_EXPERIENCEMANAGER/Brand_Portal
topic-tags: SearchandPromote
discoiquuid: dc751cd7-f663-46d2-84c4-5bb12a4fe1ba
exl-id: 7297bbe5-df8c-4d0b-8204-218a9fdc2292
source-git-commit: cbdd943b904882cc9a455bab24c3cf732d5966ca
workflow-type: tm+mt
source-wordcount: '1358'
ht-degree: 5%

---

# Buscar recursos en Brand Portal {#search-assets-on-brand-portal}

La capacidad de búsqueda de Brand portal le permite búsqueda activos relevantes rápidamente mediante omnisearch, y búsqueda de faceta que utiliza filtros para ayudarle a reducir aún más el búsqueda. Puede búsqueda activos en el nivel de archivos o carpetas y guardar los resultados de búsqueda como colecciones inteligentes.

>[!NOTE]
>
>Brand Portal no admite la recopilación búsqueda mediante omnisearch.
>
>Sin embargo, puede utilizar [ búsqueda filtros para obtener la lista de colecciones ](#search-collection) relevantes.

## Search activos con Omnisearch {#search-assets-using-omnisearch}

Para búsqueda para activos en el portal de marca:

1. En la barra de herramientas, haga clic en el **[!UICONTROL icono Search]** o pulse la tecla &quot; **[!UICONTROL /]** &quot; para iniciar Omnisearch.

   ![](assets/omnisearchicon-1.png)

1. En el cuadro búsqueda, escriba una palabra clave para el activos que desee búsqueda.

   ![](assets/omnisearch.png)

   >[!NOTE]
   >
   >* Se requieren al menos 3 caracteres en omnisearch para que las sugerencias de búsqueda aparezcan.
   >* Cuando búsqueda para `mountain biking` , omnisearch devuelve todos los activos en los búsqueda resultados que `mountain` `biking` están disponibles en los campos metadatos. Por ejemplo, `mountain` en el `Title` campo y `biking` en el `Description` campo. Ambos términos deben estar disponibles en los campos metadatos para que se muestren en los resultados de búsqueda. Sin embargo, omnisearch devuelve el recurso en el búsqueda resultados igualado si solo uno de los dos términos está disponible en el campo de etiquetas inteligentes metadatos. Por ejemplo, si una recurso contiene `mountain` como una de las etiquetas inteligentes y no contiene `biking` ningún otro campo de metadatos y búsqueda para `mountain biking` , omnisearch sigue deteniendo la recurso en los resultados búsqueda.


1. Seleccione una de las sugerencias relacionadas que aparecen en la lista desplegable lista para acceder rápidamente a activos relevantes.

   ![](assets/assets-search-result.png)

   *búsqueda de recursos con omnisearch*

Para conocer el comportamiento de búsqueda con etiquetado inteligente activos, consulte [ comprender los resultados y el comportamiento ](https://experienceleague.adobe.com/docs/experience-manager-65/assets/using/search-assets.html) de búsqueda.

## Search el uso de facetas en el panel filtros {#search-using-facets-in-filters-panel}

Las facetas de Search en el panel filtros añaden Granularidad a la experiencia de búsqueda y hacen que el búsqueda funcionalidad sea eficaz. Las facetas de Search utilizan varias dimensiones (predicados) que permiten realizar búsquedas intrincadas. Puede explorar en profundidad fácilmente al nivel de detalle deseado para obtener un búsqueda más orientado.

Por ejemplo, si busca una imagen, puede elegir si desea un mapa de bits o una imagen vectorial. Puede reducir el ámbito de búsqueda si especifica el tipo MIME para la imagen en la faceta búsqueda Archivo tipo. Del mismo modo, al buscar documentos, puede especificar la formato, por ejemplo, PDF o MS® Word formato.

![Panel filtros en el panel filtros del portal ](assets/file-type-search.png " de marca de Brand portal")

El **[!UICONTROL Panel filtros]** incluye algunas facetas estándar, como- **[!UICONTROL Path Browser]** , **[!UICONTROL archivo Type]** , **[!UICONTROL archivo size]** , **[!UICONTROL estado]** y **[!UICONTROL Orientation]** . Sin embargo, puede [ Agregar facetas ](../using/brand-portal-search-facets.md) de búsqueda personalizadas o quitar facetas de búsqueda específicas del **[!UICONTROL Panel filtros]** añadiendo o eliminando predicados en el formulario Search subyacente. Consulte la lista de los predicados de búsqueda disponibles y útiles [ en Brand portal ](../using/brand-portal-search-facets.md#list-of-search-predicates) .

Para aplicar filtros a su búsqueda, utilice las facetas ](../using/brand-portal-search-facets.md) de búsqueda disponibles [ :

1. Haga clic en el icono superposición y seleccione **[!UICONTROL filtrar]** .

   ![](assets/selectorrail.png)

1. **[!UICONTROL En el panel filtros]** de la izquierda, seleccione las opciones apropiadas para aplicar la filtros correspondiente.
Por ejemplo, utilice las siguientes filtros estándar:

   * **[!UICONTROL Explorador]** de rutas de acceso para búsqueda activos en un directorio específico. La ruta de búsqueda predeterminada del predicado para el explorador de rutas es, que se `/content/dam/mac/<tenant-id>/` puede configurar editando el formulario búsqueda predeterminado.
   >[!NOTE]
   >
   >Para los usuarios que no son administradores, [!UICONTROL  el navegador ] de rutas en [!UICONTROL  filtrar ] panel muestra únicamente la estructura contenido de las carpetas (y sus carpetas antecesoras) compartidas con ellas.\
   >Para los usuarios administradores, Path Browser permite navegar a cualquier carpeta en Brand portal.

   * **[!UICONTROL Archivo tipo]** para especificar el tipo (imagen, documento, multimedia, archivo) de recurso archivo que está buscando. Además, puede reducir el ámbito de su búsqueda, por ejemplo, especificar el tipo MIME (TIFF, Mapa de bits, imágenes GIMP) para la imagen o formato (PDF o MS® Word) para el documentos.
   * **[!UICONTROL Archivo tamaño]** para búsqueda para activos basado en su tamaño. Puede especificar los límites inferior y superior para el intervalo de tamaño a fin de reducir el búsqueda y especificar la unidad de medir a búsqueda.
   * **[!UICONTROL Estado]** para búsqueda por activos en función de los estados recurso, como la aprobación (aprobada, los cambios solicitados, la rechazado pendiente) y la caducidad.
   * **[!UICONTROL Clasificación]** promedio para búsqueda para activos según la clasificación de la activos.
   * **[!UICONTROL Orientación]** a búsqueda para activos basada en la orientación (horizontal, vertical, cuadrada) de la activos.
   * **[!UICONTROL Estilo]** que se va a búsqueda para activos basado en el estilo (color, monocromo) de la activos.
   * **[!UICONTROL Vídeo formato]** a búsqueda para vídeo activos basado en sus formato (DVI, Flash, MPEG4, MPEG, ogg Theora, QuickTime, Windows Media, WebM).

   Puede utilizar [ facetas ](../using/brand-portal-search-facets.md) de búsqueda personalizadas en el panel filtros editando el formulario de Search subyacente.

   * **[!UICONTROL El predicado]** de propiedad si se utiliza en el formulario búsqueda, permite búsqueda activos que se corresponden con una Propiedad metadatos a la que se asigna el predicado.\
      Por ejemplo, si el predicado de propiedad está asignado a [!UICONTROL `jcr:content /metadata/dc:title`] , puede búsqueda activos en función de su título.\
      El [!UICONTROL  predicado ] de propiedad admite búsquedas de texto para:

      **Frases parciales** Para permitir la búsqueda de recursos utilizando frases parciales en el predicado de propiedad, habilite la casilla **[!UICONTROL Búsqueda parcial]** en el formulario de búsqueda. Esto le permite buscar los recursos deseados aunque no especifique las palabras o frases exactas utilizadas en los metadatos del recurso.

      >[!NOTE]
      >
      > Brand portal admite los siguientes campos para Search parciales:
      >* JCR: contenido/metadatos/DC: title
      >* JCR: contenido/JCR: title
      >* JCR: contenido/metadatos/Dam: search_promote
      >* jcr:content/metadata/dc:format


      Puede hacer lo siguiente:
      * Especifique una palabra en la frase buscada en la faceta en el panel filtros. Por ejemplo, si búsqueda para el término **Climb** (y el predicado de propiedad está asignado a [!UICONTROL `dc:title`] propiedad), se devuelven todos los activos con la palabra **Climb** en su frase de título.
      * Especifique una parte de la palabra, que se produzca en la frase buscada, junto con un carácter comodín ( &#42; ) para completar las brechas.
Por ejemplo, buscar:
         * **Climb&#42;** devuelve todos los activos que tienen palabras que empiezan con los caracteres &quot;Climb&quot; en la frase del título.
         * **&#42;Climb** devuelve todos los activos que tienen palabras que terminan con los caracteres &quot;Climb&quot; en la frase del título.
         * **&#42;Climb&#42;** devuelve todos los activos que tienen palabras que comprenden los caracteres &quot;Climb&quot; en la frase del título.

Para permitir búsqueda no con distinción de mayúsculas y minúsculas en Propiedad predicado, active la       **Texto** no con distinción de mayúsculas y minúsculas
Para permitir búsqueda no con distinción de mayúsculas y minúsculas en Propiedad predicado, active la **[!UICONTROL casilla ignorar mayúsculas y minúsculas]** en Search Form. De forma predeterminada, el búsqueda de texto en Propiedad predicado distingue entre mayúsculas y minúsculas.
   >[!NOTE]
   >
   >Al seleccionar **[!UICONTROL la casilla de verificación parcial Search]** , la opción ignorar mayúsculas y **[!UICONTROL minúsculas]** está seleccionada de forma predeterminada.

   ![](assets/wildcard-prop-1.png)

   Los resultados de búsqueda se muestran según la filtros aplicada, junto con el recuento de resultados de búsqueda.

   ![](assets/omnisearch-with-filters.png)

   Resultado de búsqueda de recursos con recuento de resultado de búsqueda.

1. Puede desplazarse fácilmente a un elemento de la resultado de búsqueda y volver a la misma resultado de búsqueda con el fondo botón de la explorador sin tener que volver a ejecutar el consulta de búsqueda.

## Guardar las búsquedas como colección inteligente {#save-your-searches-as-smart-collection}

Puede guardar la configuración de búsqueda como colección inteligente para poder repetir rápidamente la misma búsqueda sin tener que rehacer la misma configuración posteriormente. Sin embargo, no se puede aplicar búsqueda filtros en un colección.

Para guardar la configuración de búsqueda como colección inteligente:

1. Toque o haga clic en **[!UICONTROL Guardar colección]** inteligente y proporcione un nombre para el colección inteligente.

   Para que el colección inteligente pueda acceder a todos los usuarios, seleccione **[!UICONTROL público]** . Un mensaje confirma que la colección inteligente se creó y se agregó al lista de las búsquedas guardadas.

   >[!NOTE]
   >
   >A los usuarios que no son administradores se les puede restringir la publicación de colecciones inteligentes para evitar tener un gran número de colecciones inteligentes públicas creadas por usuarios que no son administradores en el portal de marca de la organización. Las organizaciones pueden desactivar la opción permitir la configuración de creación ]**de colecciones inteligentes públicas desde**[!UICONTROL  las opciones generales ]**disponibles en el**[!UICONTROL  panel herramientas de administración.

   ![](assets/save_smartcollectionui.png)

1. Para guardar el colección inteligente en otro nombre, Active o desactive la **[!UICONTROL casilla Public]** , haga clic en **[!UICONTROL Editar colección]** inteligente.

   ![](assets/edit_smartcollection.png)

1. En el **[!UICONTROL cuadro de diálogo Editar colección]** inteligente, seleccione **[!UICONTROL Guardar as]** e introduzca un nombre para el colección inteligente. Haga clic en **[!UICONTROL Guardar]**.

   ![](assets/saveas_smartsearch.png)


## Search colección {#search-collection}

Omnisearch no es compatible con las colecciones. No obstante, se puede aplicar búsqueda filtros para lista las colecciones correspondientes desde la [!UICONTROL  interfaz de colecciones ] .

Desde la [!UICONTROL  interfaz de colecciones ] , haga clic en el icono de superposición para abrir el panel de filtro en el carril izquierdo. Aplicar uno o varios búsqueda filtros de la filtros disponibles ( `modified date` , `access type` , y `tags` ). Enumera el conjunto de colecciones más relevante en función de la filtros aplicada.

![](assets/collection-search.png)
