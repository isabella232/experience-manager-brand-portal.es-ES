---
title: Publicar etiquetas en Brand Portal
seo-title: Publicar etiquetas en Brand Portal
description: Obtenga información sobre cómo publicar etiquetas de AEM Assets en Brand Portal.
seo-description: Obtenga información sobre cómo publicar etiquetas de AEM Assets en Brand Portal.
uuid: 4167367e-1af8-476b-97a5-730c43bd0816
topic-tags: publish
products: SG_EXPERIENCEMANAGER/Brand_Portal
content-type: reference
discoiquuid: 3c8e9251-195d-4c56-a9a9-27bc8b2a82a4
translation-type: tm+mt
source-git-commit: 86d4d5c358ea795e35db2dce8c9529ed14e9ee2d
workflow-type: tm+mt
source-wordcount: '623'
ht-degree: 4%

---


# Publicar etiquetas en Brand Portal {#publish-tags-to-brand-portal}

Obtenga información sobre cómo publicar etiquetas de AEM Assets en Brand Portal.

Las etiquetas son útiles para organizar los recursos y mejorar la capacidad de búsqueda de los recursos a los que están asociados. Las etiquetas se pueden considerar palabras clave o etiquetas (metadatos) que se adjuntan a los recursos y permiten encontrarlos rápidamente como resultado de una búsqueda. Para saber cómo asignar etiquetas a recursos en AEM Assets, consulte [Uso de etiquetas para organizar recursos](https://helpx.adobe.com/experience-manager/6-5/assets/using/organize-assets.html#Usetagstoorganizeassets).

Las etiquetas (asociadas con recursos y colecciones en AEM) se publican automáticamente en Brand Portal cuando los recursos (y las colecciones) con etiquetas asociadas se publican en Brand Portal. Las etiquetas publicadas son útiles para permitir que las búsquedas encuentren los recursos asociados.

>[!NOTE]
>
>Sin embargo, se recomienda publicar únicamente etiquetas en Brand Portal antes de publicar los recursos (y colecciones) con los que están asociadas las etiquetas. Esto garantiza una publicación más rápida de los recursos (y las colecciones) en Brand Portal.

## Manage tags {#manage-tags}

Puede utilizar las etiquetas preexistentes para adjuntar a un recurso o crear nuevas etiquetas desde la consola Etiquetas AEM (**[!UICONTROL Herramientas) | Etiquetado | Etiquetas]** AEM). En ambos casos, primero debe publicar las etiquetas en Brand Portal y, a continuación, asociarlas con los recursos adecuados.

Para crear etiquetas en AEM, publique las etiquetas en Brand Portal y asócielas a los recursos (o colecciones) adecuados, siga estos pasos:

1. **Crear etiquetas** Inicie sesión en la instancia de AEM Author con privilegios de administrador y acceda a la consola Etiquetas **[!UICONTROL de]** AEM desde la navegación global:

   1. Seleccionar **[!UICONTROL herramientas]**

   1. Seleccionar **[!UICONTROL general]**

   1. Seleccionar **[!UICONTROL etiquetado]**

1. Seleccione **[!UICONTROL Crear]** y, a continuación, seleccione la opción **[!UICONTROL Crear etiqueta]** .
1. Especifique:

   * **[!UICONTROL Título]**

      *(obligatorio)* Un título de visualización para la etiqueta.
   * **[!UICONTROL Nombre]**
      *(obligatorio)* Un nombre para la etiqueta. Si no se especifica, se crea un nombre de nodo válido a partir del título. Consulte [TagID](https://helpx.adobe.com/experience-manager/6-5/sites/developing/using/framework.html#TagID).
   * **Descripción**

      *(opcional)* Descripción de la etiqueta.
   * **Ruta** de etiqueta JCR de la etiqueta.

1. Seleccione **[!UICONTROL Enviar]** para crear la etiqueta.

   Una vez que haya creado una etiqueta en una instancia de AEM, la etiqueta estará disponible para adjuntarse a un recurso (mediante la sección Propiedades o la sección Administrar etiquetas de ese recurso).

1. **Publique la etiqueta en Brand Portal**.

   Vaya a la consola Etiquetas **** AEM ([!UICONTROL Herramientas) | Etiquetado | Etiquetas]AEM), seleccione la etiqueta que desee y Publicar en Brand Portal.

1. **Adjunte la etiqueta a un recurso (o colección)**.

   Seleccione un recurso (o colección) y adjunte la etiqueta deseada mediante la sección Propiedades o la sección Administrar etiquetas de ese recurso. Para obtener más información sobre cómo asignar etiquetas a recursos en AEM Assets, consulte [Uso de etiquetas para organizar recursos](https://helpx.adobe.com/experience-manager/6-5/assets/using/organize-assets.html#Usetagstoorganizeassets).

1. **Publique recursos (o colecciones) en Brand Portal**.\
   Cuando publica un recurso (o colección) en Brand Portal, la etiqueta adjunta también está disponible en Brand Portal.

   Para ver la etiqueta adjunta en el recurso (o colección) correspondiente en Brand Portal, inicie sesión en Brand Portal y seleccione el recurso. En la sección Propiedades verá la etiqueta adjunta.

## Buscar Promocionar {#search-promote}

El portal de marcas de AEM Assets le permite incluir recursos específicos como los principales resultados de las búsquedas basadas en una etiqueta de palabra clave.

Para elevar un recurso para una palabra clave de búsqueda, siga estos pasos:

1. Abra la página **[!UICONTROL Propiedades]** de un recurso en una instancia de autor de AEM.
1. Vaya a la ficha **[!UICONTROL Avanzado]** .
1. En la sección **[!UICONTROL Buscar promociones]** dentro de **[!UICONTROL Elevar para palabras clave]** de búsqueda, seleccione **[!UICONTROL Añadir]** para agregar las palabras clave o etiquetas de búsqueda.

   ![](assets/search-promote.png)

1. Guarde los cambios.
1. Publicar el recurso en el portal de marca.
1. Inicie sesión en Brand Portal. Ficha **[!UICONTROL Avanzado]** de Vista en la sección **[!UICONTROL Propiedades]** del recurso.
Tenga en cuenta que la palabra clave de **[!UICONTROL Search Promote]** también está visible en las Propiedades de ese recurso.
