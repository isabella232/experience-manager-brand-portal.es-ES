---
title: Aplicación de ajustes preestablecidos de imagen o representaciones dinámicas
seo-title: Aplicación de ajustes preestablecidos de imagen o representaciones dinámicas
description: 'Al igual que una macro, un ajuste preestablecido de imagen es una colección predefinida de comandos de tamaño y formato guardados con un nombre. Los ajustes preestablecidos de imagen permiten a AEM Assets Brand Portal distribuir imágenes de forma dinámica de diferentes tamaños, formatos y propiedades. '
seo-description: 'Al igual que una macro, un ajuste preestablecido de imagen es una colección predefinida de comandos de tamaño y formato guardados con un nombre. Los ajustes preestablecidos de imagen permiten a AEM Assets Brand Portal distribuir imágenes de forma dinámica de diferentes tamaños, formatos y propiedades. '
uuid: a 3 c 8705 c -5 fbd -472 c -8 b 61-f 65 b 3 e 552 c 1 b
content-type: referencia
topic-tags: administración
products: SG_ EXPERIENCEMANAGER/Brand_ Portal
discoiquuid: a 512 dfa 0-fef 3-4 c 3 f-a 389-a 0 a 3 a 7415 bac
translation-type: tm+mt
source-git-commit: 32c3cdb8e3fafd74cfb36e6bcfe0811e7152b2d0

---


# Aplicación de ajustes preestablecidos de imagen o representaciones dinámicas {#apply-image-presets-or-dynamic-renditions}

Al igual que una macro, un ajuste preestablecido de imagen es una [!UICONTROL colección] predefinida de comandos de tamaño y formato guardados con un nombre. Los ajustes preestablecidos de imagen permiten [!DNL AEM] a los recursos [!DNL Brand Portal] distribuir imágenes de forma dinámica de diferentes tamaños, formatos y propiedades.

Se utiliza un ajuste preestablecido de imagen para generar representaciones dinámicas de imágenes que se pueden previsualizar y descargar. Al obtener una vista previa de las imágenes y sus representaciones, puede elegir un ajuste preestablecido para dar formato a las imágenes según las especificaciones establecidas por el administrador.

Para ver representaciones dinámicas de un recurso en [!DNL Brand Portal], asegúrese de que su representación PTIFF existe en la instancia [!DNL AEM] de autor desde donde realice la publicación [!DNL Brand Portal]. Cuando publique el recurso, también se publicará su representación PTIFF [!DNL Brand Portal]. No hay manera de generar la representación PTIFF desde [!DNL Brand Portal].

>[!NOTE]
>
>Al descargar imágenes y sus representaciones, no existe ninguna opción para elegir entre los ajustes preestablecidos existentes. En su lugar, puede especificar las propiedades de un ajuste preestablecido de imagen personalizado. Para obtener más información, consulte [Aplicación de ajustes preestablecidos de imagen al descargar imágenes](../using/brand-portal-image-presets.md#main-pars-text-1403412644).

Para obtener más información sobre los parámetros requeridos al crear ajustes preestablecidos de imagen, consulte [Administración de ajustes preestablecidos]de imagen (https://docs.adobe.com/docs/en//6-0/administer/integration/dynamic-media/image-presets.html)[!DNL AEM].

## Creación de un ajuste preestablecido de imagen {#create-an-image-preset}

Los administradores pueden crear ajustes preestablecidos de imagen que aparecen como representaciones dinámicas en la página de detalles del recurso. Puede crear un ajuste preestablecido de imagen desde cero o guardar uno existente con un nuevo nombre. Al crear un ajuste preestablecido de imagen, elija un tamaño para la entrega de imágenes y los comandos de formato. Cuando se envía una imagen para su visualización, su aspecto se optimiza según los comandos elegidos.
Tenga [!DNL Brand Portal]en cuenta que solo los administradores pueden crear ajustes preestablecidos de imagen.

Tenga [!DNL Brand Portal]en cuenta que solo los administradores pueden crear ajustes preestablecidos de imagen.

>[!NOTE]
>
>Se crean representaciones dinámicas para los recursos para los que PTIFF está disponible. Así pues, si un recurso no tiene una representación Pyramid TIFF creada y [!DNL AEM] publicada en [!DNL Brand Portal], solo se pueden exportar sus representaciones del sistema, pero las representaciones dinámicas se presentan como opción.
Se debe habilitar el modo Híbrido de Dynamic Media en [!DNL AEM] (autor) para crear pyamid tiff (ptiff) de un recurso. Cuando se publica un recurso de este tipo, [!DNL Brand Portal]se aplican los ajustes preestablecidos de imagen y se muestran representaciones dinámicas.

1. En la [!DNL AEM] barra de herramientas de la parte superior, haga clic en el logotipo de Adobe para acceder a las herramientas administrativas.

   !![](assets/[!DNL AEM]logo. png)

2. En el panel de herramientas administrativas, haga clic en Ajustes preestablecidos **de imagen**.

   ![](assets/admin-tools-panel-4.png)

3. En la página Ajustes preestablecidos de imagen, haga clic **en Crear**.

   ![](assets/image_preset_homepage.png)

4. En la página **Editar ajuste preestablecido** de imagen, introduzca los valores en las fichas **Básico** y **Avanzado** , según corresponda, incluyendo un nombre. Las opciones se describen en [Opciones]de ajustes preestablecidos de imagen (https://docs.adobe.com/docs/en//6-0/administer/integration/dynamic-media/image-presets.html#Image%20preset%20options)[!DNL AEM]. Los ajustes preestablecidos aparecen en el panel izquierdo y se pueden utilizar sobre la marcha con otros recursos.

   ![](assets/image_preset_create.png)

   >[!NOTE]
   >
   >También puede utilizar la página **Editar ajuste preestablecido** de imagen para editar las propiedades de un ajuste preestablecido de imagen existente. Para editar un ajuste preestablecido de imagen, selecciónelo en la página Ajustes preestablecidos de imagen y haga clic **en Editar**.

5. Haga clic en **Guardar.** El ajuste preestablecido de imagen se crea y muestra en la página de ajustes preestablecidos de imagen.
6. Para eliminar un ajuste preestablecido de imagen, selecciónelo en la página de ajustes preestablecidos de imagen y haga clic **en Eliminar**. En la página de confirmación, haga clic **en Eliminar** para confirmar la eliminación. El ajuste preestablecido de imagen se quita de la página de ajustes preestablecidos de imagen.

## Aplicación de ajustes preestablecidos de imagen al previsualizar imágenes {#apply-image-presets-when-previewing-images}

Al obtener una vista previa de las imágenes y sus representaciones, elija entre los ajustes preestablecidos existentes para dar formato a las imágenes según las especificaciones establecidas por el administrador.

1. Desde [!DNL Brand Portal] la interfaz, haga clic en una imagen para abrirla.
2. Haga clic en el icono de superposición a la izquierda y elija **Representaciones**.

   ![](assets/image-preset-previewrenditions.png)

3. En la lista **Representaciones** , seleccione la representación dinámica adecuada, por ejemplo **Miniatura**. La imagen de vista previa se procesa según su elección de la representación.

   ![](assets/image-preset-previewrenditionthumbnail.png)

## Aplicación de ajustes preestablecidos de imagen al descargar imágenes {#apply-image-presets-when-downloading-images}

Al descargar imágenes y sus representaciones, [!DNL Brand Portal]no puede elegir entre los ajustes preestablecidos de imagen existentes. Sin embargo, puede personalizar las propiedades de ajustes preestablecidos de imagen en función de la que desee dar formato a las imágenes.

1. Desde [!DNL Brand Portal] la interfaz, realice una de las siguientes acciones:

   * Sitúe el puntero sobre la imagen que desee descargar. En las miniaturas de acción rápida disponibles, haga clic en el icono **Descargar** .
   ![](assets/downloadsingleasset.png)

   * Seleccione la imagen que desee descargar. En la barra de herramientas de la parte superior, haga clic en el icono **Descargar** .
   ![](assets/downloadassets.png)

2. En el cuadro **de** diálogo Descargar, seleccione las opciones necesarias en función de si desea descargar el recurso con o sin sus representaciones.

   ![](assets/donload-assets-dialog.png)

3. Para descargar representaciones dinámicas del recurso, seleccione la **opción Representaciones** dinámicas.
4. Personalice las propiedades del ajuste preestablecido de imagen en función de la que desee cambiar dinámicamente la imagen y sus representaciones durante la descarga. Especifique el tamaño, el formato, el espacio de color, la resolución y el modificador de imagen.

   ![](assets/dynamicrenditions.png)

5. Haga clic **en Descargar**. Las representaciones dinámicas personalizadas se descargan en un archivo ZIP junto con la imagen y las representaciones que elija descargar. Sin embargo, no se crea ningún archivo zip si se descarga un único recurso, lo que garantiza una descarga rápida.
