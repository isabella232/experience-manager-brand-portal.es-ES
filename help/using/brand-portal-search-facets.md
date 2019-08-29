---
title: Usar facetas de búsqueda personalizadas
seo-title: Usar facetas de búsqueda personalizadas
description: Los administradores pueden agregar predicados de búsqueda al panel Filtros para personalizar la búsqueda y hacer que la funcionalidad de búsqueda sea versátil.
seo-description: Los administradores pueden agregar predicados de búsqueda al panel Filtros para personalizar la búsqueda y hacer que la funcionalidad de búsqueda sea versátil.
uuid: 986 fba 5 a-fac 5-4128-ac 75-d 04 da 5 b 52 d 45
content-type: referencia
topic-tags: administración
products: SG_ EXPERIENCEMANAGER/Brand_ Portal
discoiquuid: 19 faa 028-246 b -42 c 7-869 f -97 c 95 c 7 a 1349
translation-type: tm+mt
source-git-commit: ea7fdd2df0696ed309227fa77e3f79d0141bcb58

---


# Usar facetas de búsqueda personalizadas {#use-custom-search-facets}

Los administradores pueden agregar predicados de búsqueda al panel Filtros para personalizar la búsqueda y hacer que la funcionalidad de búsqueda sea versátil.

[!DNL Brand Portal] admite [la búsqueda masiva](../using/brand-portal-searching.md#search-using-facets-in-filters-panel) de búsquedas granulares de recursos de marca aprobados, que es posible debido al panel [**Filtros**](../using/brand-portal-searching.md#search-using-facets-in-filters-panel). Las facetas de búsqueda están disponibles en el panel Filtros a través de Formulario **de búsqueda** en las herramientas de administración. Existe un formulario de búsqueda predeterminado denominado Raíl de búsqueda de administrador de recursos en la página Formularios de búsqueda de las herramientas de administración. Sin embargo, los administradores pueden personalizar el panel de filtros predeterminado editando el formulario de búsqueda predeterminado (carril de búsqueda de administración de recursos) agregando, modificando o eliminando predicados de búsqueda, de modo que la funcionalidad de búsqueda sea versátil.

Puede utilizar varios predicados de búsqueda para personalizar el panel **Filtros** . Por ejemplo, agregue el predicado de propiedad para buscar recursos que coincidan con una única propiedad especificada en este predicado. Agregue las opciones predicado para buscar recursos que coincidan con uno o más valores especificados para una propiedad concreta. Agregue el predicado de intervalo de fechas para buscar recursos creados dentro de un intervalo de fechas especificado.

>[!NOTE]
>
>[!DNL AEM] permite a las organizaciones [publicar los formularios de búsqueda personalizados desde [! Autor DNL AEM]](../using/publish-schema-search-facets-presets.md#publish-search-facets-to-brand-portal) en [!DNL Brand Portal]lugar de volver a crear el mismo formulario.[!DNL Brand Portal]

## Agregar un predicado de búsqueda {#add-a-search-predicate}

Para agregar un predicado de búsqueda al panel **Filtros** :

1. Para acceder a las herramientas administrativas, haga clic [!DNL AEM] en el logotipo de la barra de herramientas en la parte superior.

   ![](assets/aemlogo.png)

2. En el panel de herramientas administrativas, haga clic **en Buscar formularios**.

   ![](assets/navigation-panel-1.png)

3. En la página **Buscar formularios** , seleccione **la barra de búsqueda de administración de recursos**.

   ![](assets/search-forms-page.png)

4. En la barra de herramientas que aparece en la parte superior, haga clic **en Editar** para abrir el formulario de búsqueda de edición.

   ![](assets/edit-search-form-1.png)

5. En la página **Editar formulario** de búsqueda, arrastre un predicado de la **ficha Seleccionar predicado** al panel principal. Por ejemplo, arrastre **Predicado de propiedad**.

   El campo **Propiedad** aparece en el panel principal y la ficha **Configuración** de la derecha muestra los predicados de propiedad.

   ![](assets/partial-prop-predicate.png)

   >[!NOTE]
   >
   >La etiqueta de encabezado de **la** ficha Configuración identifica el tipo de predicado seleccionado.

6. En la ficha **Configuración** , introduzca una etiqueta, un texto de marcador de posición y una descripción para el predicado de propiedades.

   * Seleccione **Búsqueda parcial**, si desea permitir la búsqueda parcial de frases (y búsqueda comodín) de los recursos según el valor de propiedad especificado. De forma predeterminada, el predicado admite la búsqueda de texto completo.
   * Seleccione **Omitir mayúsculas y minúsculas** si desea que la búsqueda de recursos basada en el valor de la propiedad no distinga entre mayúsculas y minúsculas. De forma predeterminada, la búsqueda de valores de propiedad en Filtro de búsqueda distingue entre mayúsculas y minúsculas.
   >[!NOTE]
   >
   >Al seleccionar **la casilla de verificación Búsqueda** parcial **, Ignorar caso** está seleccionado de forma predeterminada.

7. En el campo **Nombre** de propiedad, abra el selector de propiedades y seleccione la propiedad en función de la que se realice la búsqueda. También puede introducir un nombre para la propiedad. Por ejemplo, introduzca `  jcr :content/metadata/dc:title` o `./jcr:content/metadata/dc:title`.

   ![](assets/title-prop.png)

8. Haga clic en **Hecho** para guardar la configuración.
9. En la interfaz de usuario **de Recursos** , haga clic en el icono de superposición y elija **Filtro** para desplazarse al panel **Filtros** . El predicado **de propiedad** se agrega al panel.

   ![](assets/property-filter-panel.png)

10. Introduzca un título para el recurso que desee buscar en el cuadro de texto **Propiedad** . Por ejemplo, si introduce "Adobe". Cuando realiza una búsqueda, los recursos con el título que coincida con "Adobe" se muestran en los resultados de búsqueda.

## Lista de predicados de búsqueda {#list-of-search-predicates}

De manera similar al modo de agregar un predicado **de Propiedad** , puede agregar los siguientes predicados al panel **Filtros** :

| **Nombre de predicado** | **Descripción** | **Propiedades** |
|-------|-------|----------|
| Navegador de rutas | Busque predicado para buscar recursos en una ubicación concreta. **Nota:***Para un usuario registrado, el navegador de rutas en Filtro muestra únicamente la estructura de contenido de las carpetas (y sus antecesores) compartidas con el usuario.*<br> Los usuarios administradores pueden buscar recursos en cualquier carpeta navegando a la carpeta mediante el navegador de rutas. <br> Mientras que los usuarios no administradores pueden buscar recursos en una carpeta (accesible para ellos) navegando a esa carpeta en el Navegador de rutas. | <ul><li>Etiqueta de campo</li><li>Ruta</li><li>Descripción</li></ul> |
| Propiedad | Busque recursos en función de una propiedad de metadatos concreta. **Nota:***Al seleccionar Búsqueda parcial, Ignorar caso está seleccionado de forma predeterminada*. | <ul><li>Etiqueta de campo</li><li>Marcador de posición</li><li>Nombre de propiedad</li><li>Búsqueda parcial</li><li>Ignorar mayúsculas y minúsculas</li><li> Descripción</li></ul> |
| Propiedad de varios valores | Similar al predicado de la propiedad pero permite varios valores de entrada, separados por un delimitador (el valor predeterminado es COMA[,]los recursos que coincidan con alguno de los valores de entrada se devuelven en resultados. | <ul><li>Etiqueta de campo</li><li>Marcador de posición</li><li>Nombre de la propiedad </li><li>Compatibilidad con el delimitador</li><li>Ignorar mayúsculas y minúsculas</li><li>Descripción</li></ul> |
| Etiquetas | Busque predicado para buscar recursos basados en etiquetas. Puede configurar la propiedad Path para rellenar varias etiquetas de la lista Etiquetas. *Nota: Es posible que los administradores necesiten cambiar el valor de la ruta,* `/etc/tags/mac/<tenant_id>/<custom_tag_namespace>`*por ejemplo, si publican el formulario de búsqueda desde[!DNL AEM], donde la ruta no incluye la información del usuario, por ejemplo*`/etc/tags/<custom_tag_namespace>`. | <ul><li>Etiqueta de campo</li><li>Nombre de la propiedad </li><li>Ruta</li><li>Descripción</li></ul> |
| Ruta | Busque predicado para buscar recursos en una ubicación concreta. | <ul><li>Etiqueta de campo</li><li>Ruta</li><li>Descripción</li></ul> |  |
| Fecha relativa | Busque predicado para buscar recursos en función de la fecha relativa de su creación. | <ul><li>Etiqueta de campo</li><li>Nombre de la propiedad </li><li>Fecha relativa</li></ul> |
| Intervalo | Busque predicado para buscar recursos que se encuentren dentro de un rango específico de valores de propiedad. En el panel Filtros, puede especificar valores de propiedad mínimo y máximo para el rango. | <ul><li>Etiqueta de campo</li><li>Nombre de la propiedad </li><li>Descripción</li></ul> |
| Intervalo de fechas | Busque predicción para buscar recursos creados dentro de un intervalo especificado para una propiedad de fecha. En el panel Filtros, puede especificar fechas de inicio y finalización. | <ul><li>Etiqueta de campo</li><li>Marcador de posición</li><li>Nombre de la propiedad </li><li>Texto de rango (Desde)</li><li>Texto de intervalo (hasta)</li><li>Descripción</li></ul> |
| Fecha | Busque predicción de los recursos basados en deslizadores en función de una propiedad de fecha. | <ul><li>Etiqueta de campo</li><li>Nombre de la propiedad </li><li>Descripción</li></ul> |
| Tamaño del archivo | Busque predicciones para buscar recursos según su tamaño. | <ul><li>Etiqueta de campo</li><li>Nombre de la propiedad </li><li>Ruta</li><li>Descripción</li></ul> |
| Última modificación del recurso | Busque predicado para buscar recursos en función de la fecha de la última modificación. | <ul><li>Etiqueta de campo</li><li>Nombre de la propiedad </li><li>Descripción</li></ul> |
| Estado de aprobación | Busque predicado para buscar recursos según la propiedad de metadatos de aprobación. El nombre de propiedad predeterminado **es dam: status**. | <ul><li>Etiqueta de campo</li><li>Nombre de la propiedad </li><li>Descripción</li></ul> |
| Estado de extracción | Realice un predicado de búsqueda para buscar recursos según el estado de salida de un recurso cuando se publique desde [!DNL AEM] Assets. | <ul><li>Etiqueta de campo</li><li>Nombre de la propiedad </li><li>Descripción</li></ul> |
| Extraído por | Busque predicción para buscar recursos en función del usuario que haya extraído el recurso. | <ul><li>Etiqueta de campo</li><li>Nombre de la propiedad </li><li>Descripción</li></ul> |
| Estado de caducidad | Busque predicado para buscar recursos según el estado de caducidad. | <ul><li>Etiqueta de campo</li><li>Nombre de la propiedad </li><li>Descripción</li></ul> |
| Miembro de la colección | Busque predicado para buscar recursos en función de si un recurso forma parte de una colección. | Descripción |
| Oculto | Este predicado no es visible explícitamente para los usuarios finales y se utiliza para cualquier restricción oculta, normalmente para restringir el tipo de resultados de búsqueda a **DAM: Recurso**. | <ul><li>Etiqueta de campo</li><li>Nombre de la propiedad </li><li>Descripción</li></ul> |

>[!NOTE]
>
>No utilice **Predicado de opciones**, **Predicado de estado de publicación** y Predicado **de clasificación** ya que estos predicados no funcionan [!DNL Brand Portal]en.

## Eliminar un predicado de búsqueda {#delete-a-search-predicate}

Para eliminar un predicado de búsqueda, siga estos pasos:

1. Haga clic en el logotipo de Adobe para acceder a las herramientas administrativas.

   ![](assets/aemlogo.png)

2. En el panel de herramientas administrativas, haga clic **en Buscar formularios**.

   ![](assets/navigation-panel-2.png)

3. En la página **Buscar formularios** , seleccione **la barra de búsqueda de administración de recursos**.

   ![](assets/search-forms-page.png)

4. En la barra de herramientas que aparece en la parte superior, haga clic **en Editar** para abrir el formulario de búsqueda de edición.

   ![](assets/edit-search-form-2.png)

5. En la página **Editar formulario** de búsqueda, desde el panel principal, seleccione el predicado que desee eliminar. Por ejemplo, seleccione **Predicado de propiedad**.

   La ficha **Configuración** de la derecha muestra los campos de predicado de propiedades.

6. Para eliminar el predicado de la propiedad, haga clic en el icono de bandeja. En el cuadro **de** diálogo Eliminar campo, haga clic **en Eliminar** para confirmar la acción de eliminar.

   El campo **Predicado** de propiedad se quita del panel principal y la ficha **Configuración** queda vacía.

   ![](assets/search-form-delete-predicate.png)

7. Para guardar los cambios, haga clic **en Hecho** en la barra de herramientas.
8. En la interfaz de usuario **de Recursos** , haga clic en el icono de superposición y elija **Filtro** para desplazarse al panel **Filtros** . El predicado **de propiedad** se elimina del panel.

   ![](assets/property-predicate-removed.png)
