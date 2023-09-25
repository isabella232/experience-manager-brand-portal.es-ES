---
title: Utilizar facetas de búsqueda personalizadas
seo-title: Use custom search facets
description: Los administradores pueden agregar predicados de búsqueda al panel Filtros para personalizar la búsqueda y hacer que la funcionalidad de búsqueda sea versátil.
seo-description: Administrators can add search predicates to the Filters panel to customize search and make the search functionality versatile.
uuid: 986fba5a-fac5-4128-ac75-d04da5b52d45
content-type: reference
topic-tags: administration
products: SG_EXPERIENCEMANAGER/Brand_Portal
discoiquuid: 19faa028-246b-42c7-869f-97c95c7a1349
role: Admin
exl-id: c07e1268-2c83-40ba-8dcd-5dade3a10141
source-git-commit: c5c16d2aa1b488efac90dbc77023bba9897ae929
workflow-type: tm+mt
source-wordcount: '1325'
ht-degree: 10%

---

# Utilizar facetas de búsqueda personalizadas {#use-custom-search-facets}

Los administradores pueden agregar predicados de búsqueda a [!UICONTROL Filtros] panel para personalizar la búsqueda y hacer que la funcionalidad de búsqueda sea versátil.

Brand Portal admite [búsqueda con facetas](../using/brand-portal-searching.md#search-using-facets-in-filters-panel) para búsquedas granulares de recursos de marca aprobados, lo que es posible debido a [**Filtros** panel](../using/brand-portal-searching.md#search-using-facets-in-filters-panel). Las facetas de búsqueda están disponibles en el panel Filtros mediante **[!UICONTROL Formulario de búsqueda]** en las herramientas de administración. Existe un formulario de búsqueda predeterminado denominado Carril de búsqueda de administración de recursos en la página Buscar Forms en las herramientas de administración. Sin embargo, los administradores pueden personalizar el panel de filtros predeterminado editando el formulario de búsqueda predeterminado (carril de búsqueda de administración de recursos) agregando, modificando o eliminando predicados de búsqueda, lo que hace que la funcionalidad de búsqueda sea versátil.

Puede utilizar varios predicados de búsqueda para personalizar la variable **[!UICONTROL Filtros]** panel. Por ejemplo, agregue el predicado de propiedades para buscar recursos que coincidan con una sola propiedad que especifique en este predicado. Agregue el predicado de opciones para buscar recursos que coincidan con uno o varios valores especificados para una propiedad en particular. Agregue el predicado de intervalo de fechas para buscar recursos creados dentro de un intervalo de fechas especificado.

>[!NOTE]
>
>Experience Manager Assets permite a las organizaciones [AEM publicar los formularios de búsqueda personalizados desde el autor de la](../using/publish-schema-search-facets-presets.md#publish-search-facets-to-brand-portal) a Brand Portal, en lugar de volver a crear el mismo formulario en Brand Portal.

## Añadir un predicado de búsqueda {#add-a-search-predicate}

Para agregar un predicado de búsqueda a **[!UICONTROL Filtros]** panel:

1. Para acceder a las herramientas administrativas, haga clic en el logotipo del Experience Manager en la barra de herramientas de la parte superior.

   ![](assets/aemlogo.png)

1. En el panel de herramientas administrativas, haga clic en **[!UICONTROL Buscar Forms]**.

   ![](assets/navigation-panel-1.png)

1. En el **[!UICONTROL Buscar Forms]** página, seleccione **[!UICONTROL Carril de búsqueda de administración de Assets]**.

   ![](assets/search-forms-page.png)

1. En la barra de herramientas que aparece en la parte superior, haga clic en **[!UICONTROL Editar]** para abrir el formulario editar búsqueda.

   ![](assets/edit-search-form-1.png)

1. En el [!UICONTROL Editar formulario de búsqueda] , arrastre un predicado desde la página [!UICONTROL Seleccionar predicado] al panel principal. Por ejemplo, arrastre **[!UICONTROL Predicado de propiedad]**.

   El **[!UICONTROL Propiedad]** aparece en el panel principal y la variable **[!UICONTROL Configuración]** La pestaña de la derecha muestra los predicados de propiedad.

   ![](assets/partial-prop-predicate.png)

   >[!NOTE]
   >
   >La etiqueta de encabezado de la variable **[!UICONTROL Configuración]** La pestaña identifica el tipo de predicado que selecciona.

1. En el **[!UICONTROL Configuración]** , escriba una etiqueta, un texto de marcador de posición y una descripción para el predicado de propiedad.

   * Seleccionar **[!UICONTROL Búsqueda parcial]**, si desea permitir la búsqueda parcial de frases (y la búsqueda con comodines) de recursos en función del valor de propiedad especificado. De forma predeterminada, el predicado admite la búsqueda de texto completo.
   * Seleccionar **[!UICONTROL Ignorar mayúsculas y minúsculas]**, si desea que la búsqueda de recursos basada en el valor de la propiedad no distinga mayúsculas de minúsculas. De forma predeterminada, la búsqueda de valores de propiedad en el filtro de búsqueda distingue entre mayúsculas y minúsculas.

   >[!NOTE]
   >
   >Al seleccionar **[!UICONTROL Búsqueda parcial]** casilla, **[!UICONTROL Ignorar mayúsculas y minúsculas]** está seleccionado de forma predeterminada.

1. En el **[!UICONTROL Nombre de propiedad]** , abra el selector de propiedades y seleccione la propiedad en función de la cual se realiza la búsqueda. También puede introducir un nombre para la propiedad. Por ejemplo, escriba `jcr :content/metadata/dc:title` o `./jcr:content/metadata/dc:title`.

   >[!NOTE]
   >
   >En Brand Portal, todas las propiedades de cadena (excepto las que comienzan por ) `xmp`) en `jcrcontent/metadata` de `dam:asset` están indexados de forma predeterminada. De forma predeterminada, el resto de propiedades personalizadas de cualquier tipo no están indizadas.
   >
   >Cualquier propiedad que esté indexada puede utilizarse al crear un predicado de propiedad. Si se configura cualquier propiedad no indizada, es posible que la consulta de búsqueda de una propiedad no indizada no proporcione ningún resultado de búsqueda.

   ![](assets/title-prop.png)

1. Haga clic en **[!UICONTROL Listo]** para guardar los cambios.
1. Desde el [!UICONTROL Assets] , haga clic en el icono de superposición y seleccione **[!UICONTROL Filtrar]** para ir al **[!UICONTROL Filtros]** panel. El **[!UICONTROL Propiedad]** el predicado se agrega al panel.

   ![](assets/property-filter-panel.png)

1. Escriba un título para el recurso que se buscará en la **[!UICONTROL Propiedad]** cuadro de texto. Por ejemplo, &quot;Adobe&quot;. Al realizar una búsqueda, los recursos cuyo título coincida con &quot;Adobe&quot; se muestran en los resultados de la búsqueda.

## Lista de predicados de búsqueda {#list-of-search-predicates}

Similar a la forma de agregar un **[!UICONTROL Propiedad]** predicado, puede agregar los siguientes predicados al **[!UICONTROL Filtros]** panel:

| **Nombre de predicado** | **Descripción** | **Propiedades** |
|-------|-------|----------|
| **[!UICONTROL Navegador de rutas]** | Predicado de búsqueda para buscar recursos en una ubicación concreta. **Nota:** *Para un usuario que ha iniciado sesión, el explorador de rutas del filtro muestra únicamente la estructura de contenido de las carpetas (y sus antecesores) compartidas con el usuario.* <br> Los usuarios administradores pueden buscar recursos en cualquier carpeta navegando a ella mediante el Explorador de rutas. <br> Por su parte, los usuarios no administradores pueden buscar recursos en una carpeta (a la que pueden acceder) navegando a esa carpeta en el Explorador de rutas. | <ul><li>Etiqueta de campo</li><li>Ruta</li><li>Descripción</li></ul> |
| **[!UICONTROL Propiedad]** | Busque recursos en función de una propiedad de metadatos determinada. **Nota:** *Al seleccionar Búsqueda parcial, la opción Ignorar mayúsculas y minúsculas está seleccionada de forma predeterminada*. | <ul><li>Etiqueta de campo</li><li>Marcador de posición</li><li>Nombre de la propiedad</li><li>Búsqueda parcial</li><li>Ignorar mayúsculas y minúsculas</li><li> Descripción</li></ul> |
| **[!UICONTROL Propiedad de varios valores]** | Es similar al predicado de propiedades, pero permite varios valores de entrada, separados por un delimitador (el valor predeterminado es COMA[,]) los recursos que coincidan con cualquiera de los valores de entrada se devolverán en los resultados. | <ul><li>Etiqueta de campo</li><li>Marcador de posición</li><li>Nombre de la propiedad</li><li>Compatibilidad con el delimitador</li><li>Ignorar mayúsculas y minúsculas</li><li>Descripción</li></ul> |
| **[!UICONTROL Etiquetas]** | Predicado de búsqueda para buscar recursos en función de etiquetas. Puede configurar la propiedad Ruta para rellenar varias etiquetas en la lista Etiquetas. *Nota: Es posible que los administradores tengan que cambiar el valor de la ruta, por ejemplo, [!UICONTROL `/etc/tags/mac/<tenant_id>/<custom_tag_namespace>`]AEM , si publican el formulario de búsqueda desde el sitio web, donde la ruta no incluye información sobre el inquilino, por ejemplo, [!UICONTROL `/etc/tags/<custom_tag_namespace>`]. | <ul><li>Etiqueta de campo</li><li>Nombre de la propiedad</li><li>Ruta</li><li>Descripción</li></ul> |
| **[!UICONTROL Ruta]** | Predicado de búsqueda para buscar recursos en una ubicación concreta. | <ul><li>Etiqueta de campo</li><li>Ruta</li><li>Descripción</li></ul> |                                                     |
| **[!UICONTROL Fecha relativa]** | Predicado de búsqueda para buscar recursos en función de la fecha relativa de su creación. | <ul><li>Etiqueta de campo</li><li>Nombre de la propiedad</li><li>Fecha relativa</li></ul> |
| **[!UICONTROL Intervalo]** | Predicado de búsqueda para buscar recursos que se encuentren dentro de un rango especificado de valores de propiedad. En el panel Filtros, puede especificar los valores de propiedad mínimos y máximos del rango. | <ul><li>Etiqueta de campo</li><li>Nombre de la propiedad</li><li>Descripción</li></ul> |
| **[!UICONTROL Intervalo de fechas]** | Predicado de búsqueda para buscar recursos creados dentro de un intervalo especificado para una propiedad de fecha. En el panel Filtros, puede especificar las fechas de inicio y finalización. | <ul><li>Etiqueta de campo</li><li>Marcador de posición</li><li>Nombre de la propiedad</li><li>Texto de intervalo (desde)</li><li>Texto de intervalo (hasta)</li><li>Descripción</li></ul> |
| **[!UICONTROL Fecha]** | Predicado de búsqueda para una búsqueda de recursos basada en un control deslizante y basada en una propiedad de fecha. | <ul><li>Etiqueta de campo</li><li>Nombre de la propiedad</li><li>Descripción</li></ul> |
| **[!UICONTROL Tamaño del archivo]** | Predicado de búsqueda para buscar recursos en función de su tamaño. | <ul><li>Etiqueta de campo</li><li>Nombre de la propiedad</li><li>Ruta</li><li>Descripción</li></ul> |
| **[!UICONTROL Última modificación del recurso]** | Predicado de búsqueda para buscar recursos en función de la última fecha de modificación. | <ul><li>Etiqueta de campo</li><li>Nombre de la propiedad</li><li>Descripción</li></ul> |
| **[!UICONTROL Estado de aprobación]** | Predicado de búsqueda para buscar recursos en función de la propiedad de metadatos de aprobación. El nombre de propiedad predeterminado es **dam:status**. | <ul><li>Etiqueta de campo</li><li>Nombre de la propiedad</li><li>Descripción</li></ul> |
| **[!UICONTROL Estado de extracción]** | Predicado de búsqueda para buscar recursos en función del estado de cierre de compra de un recurso cuando se publicó desde AEM Assets. | <ul><li>Etiqueta de campo</li><li>Nombre de la propiedad</li><li>Descripción</li></ul> |
| **[!UICONTROL Extraído por]** | Predicado de búsqueda para buscar recursos en función del usuario que ha desprotegido el recurso. | <ul><li>Etiqueta de campo</li><li>Nombre de la propiedad</li><li>Descripción</li></ul> |
| **[!UICONTROL Estado de caducidad]** | Predicado de búsqueda para buscar recursos en función del estado de caducidad. | <ul><li>Etiqueta de campo</li><li>Nombre de la propiedad</li><li>Descripción</li></ul> |
| **[!UICONTROL Miembro de colección]** | Predicado de búsqueda para buscar recursos en función de si un recurso es parte de una colección. | Descripción |
| **[!UICONTROL Oculto]** | Este predicado no es visible explícitamente para los usuarios finales y se utiliza para cualquier restricción oculta normalmente para restringir el tipo de resultados de búsqueda a **dam:Asset**. | <ul><li>Etiqueta de campo</li><li>Nombre de la propiedad</li><li>Descripción</li></ul> |

>[!NOTE]
>
>* No use **[!UICONTROL Predicado de opciones]**, **[!UICONTROL Predicado de estado de publicación]**, y **[!UICONTROL Predicado de clasificación]** ya que estos predicados no funcionan en Brand Portal.
>* Predicado de tipo de carpeta `(nt:folder type)` no es compatible con Brand Portal y puede causar problemas de rendimiento. Si está presente en el formulario de búsqueda personalizado publicado, se puede eliminar editando el formulario de búsqueda.

## Eliminar un predicado de búsqueda {#delete-a-search-predicate}

Para eliminar un predicado de búsqueda, siga estos pasos:

1. Haga clic en el logotipo del Adobe para acceder a las herramientas administrativas.

   ![](assets/aemlogo.png)

1. En el panel de herramientas administrativas, haga clic en **[!UICONTROL Buscar Forms]**.

   ![](assets/navigation-panel-2.png)

1. En el **[!UICONTROL Buscar Forms]** página, seleccione **[!UICONTROL Carril de búsqueda de administración de Assets]**.

   ![](assets/search-forms-page.png)

1. En la barra de herramientas que aparece en la parte superior, haga clic en **[!UICONTROL Editar]** para abrir el formulario editar búsqueda.

   ![](assets/edit-search-form-2.png)

1. En el [!UICONTROL Editar formulario de búsqueda] , en el panel principal, seleccione el predicado que desea eliminar. Por ejemplo, seleccione **[!UICONTROL Predicado de propiedad]**.

   El **[!UICONTROL Configuración]** La pestaña de la derecha muestra los campos de predicado de propiedad.

1. Para eliminar el predicado de propiedad, haga clic en el icono bin. En el **[!UICONTROL Eliminar campo]** , haga clic en **[!UICONTROL Eliminar]** para confirmar la acción de eliminación.

   El **[!UICONTROL Predicado de propiedad]** El campo se elimina del panel principal y la variable **[!UICONTROL Configuración]** La pestaña está vacía.

   ![](assets/search-form-delete-predicate.png)

1. Para guardar los cambios, haga clic en **[!UICONTROL Listo]** en la barra de herramientas.
1. Desde el **[!UICONTROL Assets]** , haga clic en el icono de superposición y seleccione **[!UICONTROL Filtrar]** para ir al **[!UICONTROL Filtros]** panel. El **[!UICONTROL Propiedad]** el predicado se elimina del panel.

   ![](assets/property-predicate-removed.png)
