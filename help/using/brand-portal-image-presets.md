---
title: Aplicar ajustes preestablecidos de imagen o representaciones dinámicas
seo-title: Apply image presets or dynamic renditions
description: Al igual que una macro, un ajuste preestablecido de imagen es un colección predefinido de comandos de tamaño y formato guardados bajo un nombre. Imagen ajustes preestablecidos permiten que Experience Manager Assets Brand portal envíe dinámicamente imágenes de diferentes tamaños, formatos y propiedades.
seo-description: Like a macro, an image preset is a predefined collection of sizing and formatting commands saved under a name. Image presets enable Experience Manager Assets Brand Portal to dynamically deliver images of different sizes, formats, and properties.
uuid: a3c8705c-5fbd-472c-8b61-f65b3e552c1b
content-type: reference
topic-tags: administration
products: SG_EXPERIENCEMANAGER/Brand_Portal
discoiquuid: a512dfa0-fef3-4c3f-a389-a0a3a7415bac
role: Admin
exl-id: 212a1b3a-686f-4250-be06-b679b6039887
source-git-commit: 955cd8afe939ff47e9f08f312505e230e2f38495
workflow-type: tm+mt
source-wordcount: '814'
ht-degree: 3%

---

# Aplicar ajustes preestablecidos de imagen o representaciones dinámicas {#apply-image-presets-or-dynamic-renditions}

Al igual que una macro, un ajuste preestablecido de imagen es un colección predefinido de comandos de tamaño y formato guardados bajo un nombre. Imagen ajustes preestablecidos permiten que Experience Manager Assets Brand portal envíe dinámicamente imágenes de diferentes tamaños, formatos y propiedades.

Se utiliza un ajuste preestablecido de imagen para generar representaciones dinámicas de imágenes que se pueden previsualizar y descargar. Al obtener una vista previa de imágenes y sus representaciones, puede elegir un ajuste preestablecido para cambiar el formato de las imágenes según las especificaciones configuradas por el administrador.

( *Si Experience Manager assets author instancia se está ejecutando en **Dynamic media modo*** híbrido) para vista representaciones dinámicas de un recurso en Brand portal, asegúrese de que su representación de TIFF piramidal exista en el Experience Manager assets autor instancia desde donde publicar en Brand portal. Cuando publicar el recurso, su representación de PTIFF también se publica en Brand portal.

>[!NOTE]
>
>Al descargar imágenes y sus representaciones, no hay opción de elegir entre los ajustes preestablecidos existentes. En su lugar, puede especificar las propiedades de un ajuste preestablecido de imagen personalizado. Para obtener más información, consulte [ aplicar ajustes preestablecidos de imagen al descargar imágenes ](../using/brand-portal-image-presets.md#main-pars-text-1403412644) .


Para obtener más información sobre los parámetros necesarios al crear ajustes preestablecidos de imagen, consulte [Administrar ajustes preestablecidos de imagen](../using/brand-portal-image-presets.md).

## Crear un ajuste preestablecido de imagen {#create-an-image-preset}

Los administradores de Experience Manager Assets pueden crear ajustes preestablecidos de imagen que aparecen como representaciones dinámicas en la página de detalles del recurso. Puede crear un ajuste preestablecido de imagen desde cero o guardar uno existente con un nombre nuevo. Al crear un ajuste preestablecido de imagen, elija un tamaño para la entrega de imágenes y los comandos de formato. Cuando una imagen se entrega para su visualización, su aspecto se optimiza según los comandos elegidos.

>[!NOTE]
>
>Las representaciones dinámicas de una imagen se crean utilizando su TIFF piramidal. Si el TIFF piramidal no está disponible para ningún recurso, no se podrán recuperar las representaciones dinámicas de ese recurso en Brand Portal.
>
>Si la instancia de autor de Experience Manager Assets se ejecuta en **Modo híbrido de Dynamic Media**, las representaciones de TIFF piramidales de recursos de imagen se crean y guardan en el repositorio de Experience Manager Assets.
>
>Mientras que, si la instancia de autor de Experience Manager Assets se ejecuta en **Modo Dynamic Media Scene7** Además, existen representaciones de TIFF piramidales de recursos de imagen en el servidor de Scene7.
>
>Cuando estos recursos se publican en Brand Portal, se aplican ajustes preestablecidos de imagen y se muestran representaciones dinámicas.


1. En la barra de herramientas de la parte superior, haga clic en el logotipo del Experience Manager para acceder a las herramientas administrativas.

1. En el panel de herramientas administrativas, haga clic en **[!UICONTROL Ajustes preestablecidos de imagen]**.

   ![](assets/admin-tools-panel-4.png)

1. En el Página ajustes preestablecidos de imagen, haga clic en **[!UICONTROL crear]** .

   ![](assets/image_preset_homepage.png)

1. En el **[!UICONTROL Editar imagen ajuste preestablecido]** página, introduzca los valores en las **[!UICONTROL fichas básico]** y **[!UICONTROL avanzadas]** según corresponda, incluyendo un nombre. Los ajustes preestablecidos aparecen en el panel izquierdo y se pueden utilizar sobre la marcha con otros recursos.

   ![](assets/image_preset_create.png)

   >[!NOTE]
   >
   >También puede utilizar el **[!UICONTROL Editar imagen ajuste preestablecido]** Página para editar las propiedades de un ajuste preestablecido de imagen existente. Para editar un ajuste preestablecido de imagen, selecciónelo en el Página ajustes preestablecidos de imagen y haga clic en **[!UICONTROL Editar]** .

1. Haga clic en **[!UICONTROL Guardar]**. El ajuste preestablecido de imagen se crea y se muestra en la página de ajustes preestablecidos de imagen.
1. Para eliminar un ajuste preestablecido de imagen, selecciónelo en el Página ajustes preestablecidos de imagen y haga clic en **[!UICONTROL eliminar]** . En el Página de confirmación, haga clic en **[!UICONTROL eliminar]** para confirmar la eliminación. El ajuste preestablecido de imagen se elimina de la Página ajustes preestablecidos de imagen.

## Aplicar ajustes preestablecidos de imagen al obtener una vista previa de las imágenes  {#apply-image-presets-when-previewing-images}

Al obtener una vista previa de las imágenes y sus representaciones, elija entre los ajustes preestablecidos existentes para cambiar el formato de las imágenes según las especificaciones configuradas por el administrador.

1. En la interfaz de Brand portal, haga clic en una imagen para abrirla.
1. Haga clic en el icono superposición de la izquierda y elija **[!UICONTROL representaciones]** .

   ![](assets/image-preset-previewrenditions.png)

1. Desde el **[!UICONTROL Representaciones]** , seleccione la representación dinámica adecuada, por ejemplo, **[!UICONTROL Miniatura]**. La imagen de vista previa se procesará según la representación que haya elegido.

   ![](assets/image-preset-previewrenditionthumbnail.png)

## Aplicar ajustes preestablecidos de imagen al descargar imágenes {#apply-image-presets-when-downloading-images}

Al descargar imágenes y sus representaciones desde Brand Portal, no puede elegir entre los ajustes preestablecidos de imagen existentes. Sin embargo, puede personalizar las propiedades del ajuste preestablecido de imagen en función de qué imágenes desee volver a dar formato.

1. Desde la interfaz de Brand portal, realice una de las siguientes acciones:

   * Pase el puntero sobre la imagen que desee descargar. En las miniaturas de acciones rápidas disponibles, haga clic en **[!UICONTROL Descargar]** icono.

   ![](assets/downloadsingleasset.png)

   * Seleccione la imagen que desee descargar. En la barra de herramientas de la parte superior, haga clic en **[!UICONTROL Descargar]** icono.

   ![](assets/downloadassets.png)

1. Desde el **[!UICONTROL Descargar]** , seleccione las opciones necesarias en función de si desea descargar el recurso con o sin sus representaciones.

   ![](assets/donload-assets-dialog.png)

1. Para descargar representaciones dinámicas del recurso, seleccione la **[!UICONTROL Representación(es) dinámica(es)]** opción.
1. Personalice las propiedades del ajuste preestablecido de imagen en función de las cuales desee reformatear dinámicamente la imagen y sus representaciones durante la descarga. Especifique el tamaño, el formato, el espacio de color, la resolución y el modificador de imagen.

   ![](assets/dynamicrenditions.png)

1. Haga clic en **[!UICONTROL Descargar]**. Las representaciones dinámicas personalizadas se descargan en un archivo ZIP junto con la imagen y las representaciones que ha elegido para descargar. Sin embargo, no se crea ningún archivo zip si se descarga un solo recurso, lo que garantiza una descargar rápida.
