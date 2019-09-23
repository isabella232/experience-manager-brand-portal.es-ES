---
title: Utilizar facetas de búsqueda personalizadas
seo-title: Utilizar facetas de búsqueda personalizadas
description: Los administradores pueden agregar predicados de búsqueda al panel Filtros para personalizar la búsqueda y hacer que la funcionalidad de búsqueda sea versátil.
seo-description: Los administradores pueden agregar predicados de búsqueda al panel Filtros para personalizar la búsqueda y hacer que la funcionalidad de búsqueda sea versátil.
uuid: 986fba5a-face5-4128-ac75-d04da5b52d45
content-type: referencia
topic-tags: administración
products: SG_EXPERIENCEMANAGER/Brand_Portal
discoiquuid: 19faa028-246b-42c7-869f-97c95c7a1349
translation-type: tm+mt
source-git-commit: 068ce845c51de48fb677f7bd09a2f6d20ff6f1a5

---


# Utilizar facetas de búsqueda personalizadas {#use-custom-search-facets}

Los administradores pueden agregar predicados de búsqueda al panel [!UICONTROL Filtros] para personalizar la búsqueda y hacer que la funcionalidad de búsqueda sea versátil.

Brand Portal admite la búsqueda [por](../using/brand-portal-searching.md#search-using-facets-in-filters-panel) facetas de búsquedas granulares de activos de marca aprobados, lo cual es posible gracias al panel [**Filtros**](../using/brand-portal-searching.md#search-using-facets-in-filters-panel). Las facetas de búsqueda están disponibles en el panel Filtros a través de **[!UICONTROL Buscar formulario]** en las herramientas de administración. Existe un formulario de búsqueda predeterminado denominado Asset Admin Search Rail en la página Buscar formularios en las herramientas de administración. Sin embargo, los administradores pueden personalizar el panel Filtros predeterminado editando el formulario de búsqueda predeterminado (carril de búsqueda de administrador de recursos) agregando, modificando o eliminando predicados de búsqueda, lo que hace que la funcionalidad de búsqueda sea versátil.

Puede utilizar varios predicados de búsqueda para personalizar el panel **[!UICONTROL Filtros]** . Por ejemplo, agregue el predicado de propiedades para buscar recursos que coincidan con una sola propiedad especificada en este predicado. Agregue el predicado de opciones para buscar recursos que coincidan con uno o varios valores especificados para una propiedad concreta. Agregue el predicado de intervalo de fechas para buscar recursos creados dentro de un intervalo de fechas especificado.

>[!NOTE]
>
>AEM permite a las organizaciones [publicar los formularios de búsqueda personalizados de AEM Author](../using/publish-schema-search-facets-presets.md#publish-search-facets-to-brand-portal) en Brand Portal, en lugar de volver a crear el mismo formulario en Brand Portal.

## Agregar un predicado de búsqueda {#add-a-search-predicate}

Para agregar un predicado de búsqueda al panel **[!UICONTROL Filtros]** :

1. Para acceder a las herramientas administrativas, haga clic en el logotipo de AEM en la barra de herramientas de la parte superior.

   ![](assets/aemlogo.png)

2. En el panel Herramientas administrativas, haga clic en **[!UICONTROL Buscar formularios]**.

   ![](assets/navigation-panel-1.png)

3. En la página **[!UICONTROL Buscar formularios]** , seleccione **[!UICONTROL Recursos Administración Barra]** de búsqueda.

   ![](assets/search-forms-page.png)

4. En la barra de herramientas que aparece en la parte superior, haga clic en **[!UICONTROL Editar]** para abrir el formulario de edición de búsqueda.

   ![](assets/edit-search-form-1.png)

5. En la página [!UICONTROL Editar formulario] de búsqueda, arrastre un predicado desde la ficha [!UICONTROL Seleccionar predicado] al panel principal. Por ejemplo, arrastre Predicado **[!UICONTROL de propiedades]**.

   El campo **[!UICONTROL Propiedad]** aparece en el panel principal y la ficha **[!UICONTROL Configuración]** de la derecha muestra los predicados de propiedades.

   ![](assets/partial-prop-predicate.png)

   >[!NOTE]
   >
   >La etiqueta de encabezado de la ficha **[!UICONTROL Configuración]** identifica el tipo de predicado que se selecciona.

6. En la ficha **[!UICONTROL Configuración]** , introduzca una etiqueta, un texto de marcador de posición y una descripción para el predicado de propiedades.

   * Seleccione Búsqueda **** parcial si desea permitir la búsqueda de frases parciales (y la búsqueda con comodines) de recursos en función del valor de propiedad especificado. De forma predeterminada, el predicado admite la búsqueda de texto completo.
   * Seleccione **[!UICONTROL Ignorar mayúsculas y minúsculas]** si desea que la búsqueda de recursos basada en el valor de la propiedad distinga entre mayúsculas y minúsculas. De forma predeterminada, la búsqueda de valores de propiedad en el filtro de búsqueda distingue entre mayúsculas y minúsculas.
   >[!NOTE]
   >
   >Al seleccionar la casilla de verificación Búsqueda **** parcial, se selecciona [!UICONTROL Omitir caso] de forma predeterminada.

7. En el campo Nombre [!UICONTROL de propiedad] , abra el selector de propiedades y seleccione la propiedad en función de la cual se realiza la búsqueda. También puede introducir un nombre para la propiedad. Por ejemplo, introduzca [!UICONTROL `  jcr :content/metadata/dc:title`] o [!UICONTROL `./jcr:content/metadata/dc:title`].

   ![](assets/title-prop.png)

8. Haga clic en **[!UICONTROL Listo]** para guardar la configuración.
9. En la interfaz de usuario de [!UICONTROL Recursos] , haga clic en el icono de superposición y elija **[!UICONTROL Filtro]** para desplazarse al panel **[!UICONTROL Filtros]** . El predicado **[!UICONTROL Propiedad]** se agrega al panel.

   ![](assets/property-filter-panel.png)

10. Introduzca un título para el recurso que desea buscar en el cuadro de texto **[!UICONTROL Propiedad]** . Por ejemplo, "Adobe". Cuando realiza una búsqueda, los recursos con el título que coincide con "Adobe" se muestran en los resultados de la búsqueda.

## Lista de predicados de búsqueda {#list-of-search-predicates}

De forma similar a como se agrega un predicado **[!UICONTROL Property]** , se pueden agregar los siguientes predicados al panel **[!UICONTROL Filtros]** :

| **Nombre del predicado** | **Descripción** | **Propiedades** |
|-------|-------|----------|
| [!UICONTROL Navegador de rutas] | El predicado de búsqueda busca recursos en una ubicación determinada. **** Nota: *Para un usuario que ha iniciado sesión, el navegador de rutas en Filtro muestra únicamente la estructura de contenido de las carpetas (y sus antecesores) compartidas con el usuario.* <br> Los usuarios administradores pueden buscar recursos en cualquier carpeta navegando a ella mediante el navegador de rutas. <br> Mientras que los usuarios que no son administradores pueden buscar recursos en una carpeta (a la que tienen acceso) navegando a esa carpeta en el navegador de rutas. | <ul><li>Etiqueta de campo</li><li>Ruta</li><li>Descripción</li></ul> |
| [!UICONTROL Propiedad] | Buscar recursos en función de una propiedad de metadatos concreta. **** Nota: *Al seleccionar Búsqueda parcial, se selecciona Omitir mayúsculas y minúsculas de forma predeterminada*. | <ul><li>Etiqueta de campo</li><li>Marcador de posición</li><li>Nombre de propiedad</li><li>Búsqueda parcial</li><li>Ignorar mayúsculas y minúsculas</li><li> Descripción</li></ul> |
| [!UICONTROL Propiedad de varios valores] | Similar al predicado de propiedades pero permite varios valores de entrada, separados por un delimitador (el valor predeterminado es COMMA[,]) los recursos que coinciden con cualquiera de los valores de entrada se devuelven en los resultados. | <ul><li>Etiqueta de campo</li><li>Marcador de posición</li><li>Nombre de la propiedad </li><li>Compatibilidad con el delimitador</li><li>Ignorar mayúsculas y minúsculas</li><li>Descripción</li></ul> |
| [!UICONTROL Etiquetas] | Busque en el predicado para buscar recursos en función de etiquetas. Puede configurar la propiedad Ruta para rellenar varias etiquetas en la lista Etiquetas. *Nota: Es posible que los administradores necesiten cambiar el valor de la ruta, por ejemplo, [!UICONTROL `/etc/tags/mac/<tenant_id>/<custom_tag_namespace>`]si publican el formulario de búsqueda desde AEM, donde la ruta no incluye la información del inquilino, por ejemplo, [!UICONTROL `/etc/tags/<custom_tag_namespace>`]. | <ul><li>Etiqueta de campo</li><li>Nombre de la propiedad </li><li>Ruta</li><li>Descripción</li></ul> |
| [!UICONTROL Ruta] | El predicado de búsqueda busca recursos en una ubicación determinada. | <ul><li>Etiqueta de campo</li><li>Ruta</li><li>Descripción</li></ul> |  |
| [!UICONTROL Fecha relativa] | El predicado de búsqueda busca recursos en función de la fecha relativa de su creación. | <ul><li>Etiqueta de campo</li><li>Nombre de la propiedad </li><li>Fecha relativa</li></ul> |
| [!UICONTROL Intervalo] | El predicado de búsqueda busca recursos que se encuentran dentro de un rango especificado de valores de propiedad. En el panel Filtros, puede especificar valores de propiedad mínimos y máximos para el rango. | <ul><li>Etiqueta de campo</li><li>Nombre de la propiedad </li><li>Descripción</li></ul> |
| [!UICONTROL Intervalo de fechas] | El predicado de búsqueda busca recursos creados dentro de un intervalo especificado para una propiedad de fecha. En el panel Filtros, puede especificar las fechas de inicio y finalización. | <ul><li>Etiqueta de campo</li><li>Marcador de posición</li><li>Nombre de la propiedad </li><li>Texto de rango (Desde)</li><li>Texto de intervalo (hasta)</li><li>Descripción</li></ul> |
| [!UICONTROL Fecha] | Busque en el predicado una búsqueda de recursos basada en deslizadores basada en una propiedad de fecha. | <ul><li>Etiqueta de campo</li><li>Nombre de la propiedad </li><li>Descripción</li></ul> |
| [!UICONTROL Tamaño del archivo] | El predicado de búsqueda busca recursos en función de su tamaño. | <ul><li>Etiqueta de campo</li><li>Nombre de la propiedad </li><li>Ruta</li><li>Descripción</li></ul> |
| [!UICONTROL Última modificación del recurso] | El predicado de búsqueda busca recursos en función de la fecha de la última modificación. | <ul><li>Etiqueta de campo</li><li>Nombre de la propiedad </li><li>Descripción</li></ul> |
| [!UICONTROL Estado de aprobación] | Busque en el predicado para buscar recursos según la propiedad de metadatos de aprobación. El nombre de propiedad predeterminado es **dam:status**. | <ul><li>Etiqueta de campo</li><li>Nombre de la propiedad </li><li>Descripción</li></ul> |
| [!UICONTROL Estado de extracción] | El predicado de búsqueda busca recursos en función del estado de cierre de compra de un recurso cuando se publicó desde Recursos AEM. | <ul><li>Etiqueta de campo</li><li>Nombre de la propiedad </li><li>Descripción</li></ul> |
| [!UICONTROL Extraído por] | El predicado de búsqueda busca recursos en función del usuario que ha extraído el recurso. | <ul><li>Etiqueta de campo</li><li>Nombre de la propiedad </li><li>Descripción</li></ul> |
| [!UICONTROL Estado de caducidad] | El predicado de búsqueda busca recursos en función del estado de caducidad. | <ul><li>Etiqueta de campo</li><li>Nombre de la propiedad </li><li>Descripción</li></ul> |
| [!UICONTROL Miembro de la colección] | El predicado de búsqueda busca recursos en función de si un recurso forma parte de una colección. | Descripción |
| [!UICONTROL Oculto] | Este predicado no es explícitamente visible para los usuarios finales y se utiliza para cualquier restricción oculta que se utilice normalmente para restringir el tipo de resultados de búsqueda a **dam:Asset**. | <ul><li>Etiqueta de campo</li><li>Nombre de la propiedad </li><li>Descripción</li></ul> |

>[!NOTE]
>
>No utilice Predicado **[!UICONTROL de]** opciones, Predicado **[!UICONTROL de estado de]** publicación y Predicado **[!UICONTROL de]** clasificación, ya que estos predicados no funcionan en Brand Portal.

## Eliminar un predicado de búsqueda {#delete-a-search-predicate}

Para eliminar un predicado de búsqueda, siga estos pasos:

1. Haga clic en el logotipo de Adobe para acceder a las herramientas administrativas.

   ![](assets/aemlogo.png)

2. En el panel Herramientas administrativas, haga clic en **[!UICONTROL Buscar formularios]**.

   ![](assets/navigation-panel-2.png)

3. En la página **[!UICONTROL Buscar formularios]** , seleccione **[!UICONTROL Recursos Administración Barra]** de búsqueda.

   ![](assets/search-forms-page.png)

4. En la barra de herramientas que aparece en la parte superior, haga clic en **[!UICONTROL Editar]** para abrir el formulario de edición de búsqueda.

   ![](assets/edit-search-form-2.png)

5. En la página [!UICONTROL Editar formulario] de búsqueda, en el panel principal, seleccione el predicado que desee eliminar. Por ejemplo, seleccione Predicado **[!UICONTROL de propiedades]**.

   La ficha **[!UICONTROL Configuración]** de la derecha muestra los campos de predicado de propiedades.

6. Para eliminar el predicado de propiedades, haga clic en el icono bin. En el cuadro de diálogo **[!UICONTROL Eliminar campo]** , haga clic en **[!UICONTROL Eliminar]** para confirmar la acción de eliminar.

   El campo Predicado **[!UICONTROL de]** propiedades se elimina del panel principal y la ficha **[!UICONTROL Configuración]** se queda vacía.

   ![](assets/search-form-delete-predicate.png)

7. Para guardar los cambios, haga clic en **[!UICONTROL Hecho]** en la barra de herramientas.
8. En la interfaz de usuario de **[!UICONTROL Recursos]** , haga clic en el icono de superposición y elija **[!UICONTROL Filtro]** para desplazarse al panel **[!UICONTROL Filtros]** . El predicado **[!UICONTROL Propiedad]** se elimina del panel.

   ![](assets/property-predicate-removed.png)
