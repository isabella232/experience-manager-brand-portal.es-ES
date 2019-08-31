---
title: Buscar recursos en Brand Portal
seo-title: Búsqueda de recursos y búsqueda guardada en AEM Brand Portal
description: La función de búsqueda de Brand Portal le permite buscar rápidamente recursos relevantes utilizando omnisearch y los filtros de búsqueda le ayudan a reducir aún más la búsqueda. Guarde las búsquedas como colecciones inteligentes para el futuro.
seo-description: La función de búsqueda de Brand Portal le permite buscar rápidamente recursos relevantes utilizando omnisearch y los filtros de búsqueda le ayudan a reducir aún más la búsqueda. Guarde las búsquedas como colecciones inteligentes para el futuro.
uuid: c 2955198-bdc 0-4853-a 13 a -661 e 6 a 9 ec 61 f
contentOwner: bdhar
content-type: referencia
products: SG_ EXPERIENCEMANAGER/Brand_ Portal
topic-tags: Searchandpromote
discoiquuid: dc 751 cd 7-f 663-46 d 2-84 c 4-5 bb 12 a 4 fe 1 ba
translation-type: tm+mt
source-git-commit: 068ce845c51de48fb677f7bd09a2f6d20ff6f1a5

---


# Buscar recursos en Brand Portal {#search-assets-on-brand-portal}

La función de búsqueda de Brand Portal le permite buscar rápidamente recursos relevantes utilizando omnisearch y una búsqueda factorial que utiliza filtros para reducir aún más la búsqueda. También puede guardar las búsquedas como colecciones inteligentes para el futuro.

## Buscar recursos con Omnisearch {#search-assets-using-omnisearch}

Para buscar recursos en Brand Portal:

1. En la barra de herramientas, haga clic en **[!UICONTROL el icono Buscar]** o presione la tecla "**[!UICONTROL /]**" para iniciar Omnisearch.

   ![](assets/omnisearchicon-1.png)

2. En el cuadro de búsqueda, escriba una palabra clave para los recursos que desee buscar.

   ![](assets/omnisearch.png)

   >[!NOTE]
   >
   >Se requieren al menos 3 caracteres en Omnisearch para que aparezcan las sugerencias de búsqueda.

3. Seleccione entre las sugerencias relacionadas que aparecen en la lista desplegable para acceder rápidamente a los recursos relevantes.

   ![](assets/assets-search-result.png)

   *Búsqueda de recursos mediante omnisearch*

## Búsqueda mediante facetas en el panel Filtros {#search-using-facets-in-filters-panel}

Las facetas de búsqueda del panel Filtros agregan granularidad a la experiencia de búsqueda y hacen que la funcionalidad de búsqueda sea eficaz. Las facetas de búsqueda utilizan varias dimensiones (predicados) que permiten realizar búsquedas intrincadas. Puede explorar fácilmente el nivel de detalle deseado para obtener una búsqueda más enfocada.

Por ejemplo, si busca una imagen, puede elegir si desea un mapa de bits o una imagen vectorial. Puede reducir aún más el ámbito de búsqueda especificando el tipo MIME para la imagen en la faceta de búsqueda Tipo de archivo. Asimismo, al buscar documentos, puede especificar el formato, por ejemplo, formato PDF o MS Word.

![Panel Filtros del panel portalfilters](assets/file-type-search.png "de Brand Portal")

El panel [!UICONTROL Filtros] incluye algunas facetas estándar, como - Navegador [!UICONTROL de rutas], Tipo [!UICONTROL de archivo], [!UICONTROL Tamaño de archivo], [!UICONTROL Estado]y [!UICONTROL Orientación]. Sin embargo, [puede agregar facetas de búsqueda personalizadas](../using/brand-portal-search-facets.md) o quitar facetas de búsqueda específicas del panel [!UICONTROL Filtros] agregando o quitando predicados en el formulario de búsqueda subyacente. Consulte la lista de predicados [de búsqueda disponibles y utilizables en Brand Portal](../using/brand-portal-search-facets.md#list-of-search-predicates).

Para aplicar filtros a la búsqueda, utilizando las facetas [de búsqueda disponibles](../using/brand-portal-search-facets.md):

1. Haga clic en el icono de superposición y seleccione **[!UICONTROL Filtro]**.

   ![](assets/selectorrail.png)

2. En el panel **[!UICONTROL Filtros]** de la izquierda, seleccione las opciones adecuadas para aplicar los filtros relevantes.
Por ejemplo, utilice los filtros estándar siguientes:

   * **[!UICONTROL Explorador de rutas]** para buscar recursos en un directorio específico. La ruta de búsqueda predeterminada del predicado para el navegador de rutas es **[!UICONTROL /content/dam/mac/ &lt; id-id &gt;/]**, que se puede configurar editando el formulario de búsqueda predeterminado.
   >[!NOTE]
   >
   >Para usuarios no administradores, [!UICONTROL el navegador] de rutas en [!UICONTROL el panel Filtro] muestra únicamente la estructura de contenido de las carpetas (y sus carpetas antecesoras) compartidas con ellos.\
   >Para administradores administradores, el navegador de rutas permite navegar a cualquier carpeta de Brand Portal.

   * **[!UICONTROL Tipo de archivo]** para especificar el tipo (imagen, documento, multimedia, archivo) del archivo de recurso que está buscando. Además, puede reducir el alcance de la búsqueda, por ejemplo, especifique el tipo MIME (Tiff, Mapa de bits, Imágenes GIMP) para la imagen o el formato (PDF o MS Word) para los documentos.
   * **[!UICONTROL Tamaño]** de archivo para buscar recursos según su tamaño. Puede especificar los límites inferior y superior del rango de tamaño para reducir la búsqueda y especificar la unidad de medida que desea buscar.
   * **[!UICONTROL Estado]** para buscar recursos en función de los estados de recursos, como Aprobación (Aprobado, Cambios solicitados, Rechazado, Pendiente) y Caducidad.
   * **[!UICONTROL Clasificación promedio]** para buscar recursos en función de la clasificación de los recursos.
   * **[!UICONTROL Orientación]** para buscar recursos en función de la orientación (horizontal, vertical, cuadrada) de los recursos.
   * **[!UICONTROL Estilo]** para buscar recursos en función del estilo (color, monocromo) de los recursos.
   * **[!UICONTROL Formato de vídeo]** para buscar recursos de vídeo en función de su formato (DVI, Flash, MPEG 4, MPEG, OGG Theora, quicktime, Windows Media, webm).
   Puede utilizar [facetas de búsqueda personalizadas](../using/brand-portal-search-facets.md) en el panel Filtros editando el formulario de búsqueda subyacente.

   * **[!UICONTROL Predicado de propiedad]** Si se utiliza en el formulario de búsqueda, permite buscar recursos que coinciden con una propiedad de metadatos a la que se asigna el predicado.\
      Por ejemplo, si se asigna el Predicado de propiedad, [!UICONTROL `jcr:content /metadata/dc:title`]puede buscar recursos en función de su título.\
      El Predicado [!UICONTROL de propiedad] admite búsquedas de texto para:

      **Frases parciales** Para permitir la búsqueda de recursos utilizando frases parciales en el predicado de propiedad, habilite la casilla **[!UICONTROL Búsqueda parcial]en el formulario de búsqueda.**\
      Esto le permite buscar los recursos deseados aunque no especifique las palabras o frases exactas utilizadas en los metadatos del recurso.\
      Puede:
* Especifique una palabra que se produzca en la frase buscada en la faceta del panel Filtros. For example, if you search for the term **climb** (and Property Predicate is mapped to [!UICONTROL `dc:title`] property), then all the assets with the word **climb** in their title phrase are returned.
* Especificar una parte de la palabra que aparece en la frase buscada, junto con el carácter comodín (*) para rellenar los huecos.
Por ejemplo, buscar:
      **escalada *** devuelve todos los recursos que tienen palabras que comienzan con los caracteres "escalada" en la frase del título.
      *** aumenta** todos los recursos que tienen palabras terminadas con caracteres "escalada" en la frase del título.
      *** escalada *** devuelve todos los recursos que tienen palabras que comprenden los caracteres "escalada" en la frase del título.\
      **Texto sin distinción de mayúsculas y**
minúsculas Para permitir búsquedas sin distinción entre mayúsculas y minúsculas en predicado de propiedad, habilite **[!UICONTROL la]** casilla Ignorar caso en el formulario de búsqueda. De forma predeterminada, la búsqueda de texto en predicado de propiedad distingue entre mayúsculas y minúsculas.
   >[!NOTE]
   >
   >Al seleccionar **[!UICONTROL la casilla de verificación Búsqueda]** parcial [!UICONTROL , Ignorar caso] está seleccionado de forma predeterminada.

   ![](assets/wildcard-prop-1.png)

   Los resultados de búsqueda se muestran según los filtros aplicados, junto con el recuento de resultados de búsqueda.

   ![](assets/omnisearch-with-filters.png)

   Resultado de búsqueda de recursos con recuento de resultados de búsqueda

3. Puede navegar fácilmente a un elemento desde el resultado de la búsqueda y regresar al mismo resultado de búsqueda utilizando el botón Atrás del explorador sin tener que volver a ejecutar la consulta de búsqueda.

## Guarde las búsquedas como una colección inteligente {#save-your-searches-as-smart-collection}

Puede guardar la configuración de búsqueda como una colección inteligente para poder repetir rápidamente la misma búsqueda sin tener que rehacer la misma configuración posteriormente.

Para guardar los ajustes de búsqueda como una colección inteligente:

1. Toque o haga clic **[!UICONTROL en Guardar colección]** inteligente y proporcione un nombre para la colección inteligente.

   Para que la colección inteligente sea accesible para todos los usuarios, seleccione **[!UICONTROL Público]**. Un mensaje confirma que la colección inteligente se creó y se agregó a la lista de las búsquedas guardadas.

   >[!NOTE]
   >
   >Los usuarios no administradores pueden no hacer públicos colecciones inteligentes, para evitar tener un gran número de colecciones inteligentes públicas creadas por usuarios no administradores en Brand Portal de la organización. Las organizaciones pueden desactivar la configuración **[!UICONTROL de creación]** de colecciones inteligentes públicas desde la configuración **[!UICONTROL General]** disponible en el panel de herramientas de administración.

   ![](assets/save_smartcollectionui.png)

2. Para guardar la colección inteligente en un nombre diferente y seleccionar o borrar la casilla **[!UICONTROL pública]** , haga clic **[!UICONTROL en Editar colección inteligente]**.

   ![](assets/edit_smartcollection.png)

3. En el cuadro **[!UICONTROL de diálogo Editar colecciones]** inteligentes, seleccione **[!UICONTROL Guardar como]** e introduzca un nombre para la colección inteligente. Haga clic en **[!UICONTROL Guardar]**.

   ![](assets/saveas_smartsearch.png)
