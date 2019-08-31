---
title: Publicar etiquetas en Brand Portal
seo-title: Publicar etiquetas en Brand Portal
description: Descubra cómo publicar etiquetas de AEM Assets en Brand Portal.
seo-description: Descubra cómo publicar etiquetas de AEM Assets en Brand Portal.
uuid: 4167367 e -1 af 8-476 b -97 a 5-730 c 43 bd 0816
topic-tags: publicación
products: SG_ EXPERIENCEMANAGER/Brand_ Portal
content-type: referencia
discoiquuid: 3 c 8 e 9251-195 d -4 c 56-a 9 a 9-27 bc 8 b 2 a 82 a 4
translation-type: tm+mt
source-git-commit: 068ce845c51de48fb677f7bd09a2f6d20ff6f1a5

---


# Publish tags to Brand Portal {#publish-tags-to-brand-portal}

Descubra cómo publicar etiquetas de AEM Assets en Brand Portal.

Las etiquetas son útiles para organizar recursos y mejorar la búsqueda de recursos a los que están asociados. Las etiquetas se pueden considerar como palabras clave o etiquetas (metadatos) que se adjuntan con recursos y permiten que los recursos se encuentren rápidamente como resultado de una búsqueda. Para saber cómo asignar etiquetas a recursos en Recursos AEM, consulte las etiquetas [de uso para organizar los recursos](https://helpx.adobe.com/experience-manager/6-5/assets/using/organize-assets.html#Usetagstoorganizeassets).

Las etiquetas (asociadas con recursos y colecciones en AEM) se publican automáticamente en Brand Portal cuando los recursos (y colecciones) con etiquetas asociadas se publican en Brand Portal. Las etiquetas publicadas son útiles para habilitar las búsquedas a fin de encontrar los activos asociados.

>[!NOTE]
>
>Sin embargo, se recomienda publicar exclusivamente etiquetas en Brand Portal antes de publicar los recursos (y colecciones) con los que están asociados las etiquetas. Esto garantiza una publicación más rápida de los recursos (y colecciones) en Brand Portal.

## Manage tags {#manage-tags}

Puede utilizar las etiquetas preexistentes para adjuntar a un recurso o crear nuevas etiquetas a partir de la consola de etiquetas AEM (**[!UICONTROL Herramientas | Etiquetado | Etiquetas AEM]**). En ambos casos, primero debe publicar las etiquetas en Brand Portal y asociarlas a los recursos correspondientes.

Para crear etiquetas en AEM, publicar las etiquetas en Brand Portal y asociar las etiquetas con los recursos (o colecciones) adecuados, siga estos pasos:

1. **Cree etiquetas**
de inicio de sesión en la instancia de AEM Author con privilegios administrativos y acceda **[!UICONTROL a la consola Etiquetas]** AEM desde la navegación global:

   1. Seleccionar **[!UICONTROL herramientas]**

   2. Seleccionar **[!UICONTROL general]**

   3. Seleccionar **[!UICONTROL etiquetado]**

2. Seleccione **[!UICONTROL Crear]** y, a continuación, seleccione **[!UICONTROL Crear etiqueta]** .
3. Especifique:

   * **[!UICONTROL Título]**
      *(requerido)* Un título para la etiqueta.
   * **[!UICONTROL Nombre]**
      *(requerido)* Un nombre para la etiqueta. Si no se especifica, se crea un nombre de nodo válido a partir del Título. Consulte [tagid](https://helpx.adobe.com/experience-manager/6-5/sites/developing/using/framework.html#TagID).
   * **Descripción**
      *(opcional)* Descripción de la etiqueta.
   * **Ruta de etiqueta**JCR de ruta
de la etiqueta.

4. Seleccione **[!UICONTROL Enviar]** para crear la etiqueta.

   Una vez creada una etiqueta en la instancia de AEM, la etiqueta estará disponible para adjuntarse a un recurso (mediante la sección Propiedades o la sección Administrar etiquetas de ese recurso).

5. **Publique la etiqueta en Brand Portal**.

   Ir a **[!UICONTROL la consola Etiquetas]** AEM ([!UICONTROL Herramientas | Etiquetado | Etiquetas AEM]), seleccione la etiqueta que desee y Publique en Brand Portal.

6. **Adjunte la etiqueta a un recurso (o colección)**.

   Seleccione un recurso (o colección) y adjunte la etiqueta que desee mediante la sección Propiedades o la sección Administrar etiquetas de dicho recurso. Para obtener más información sobre cómo asignar etiquetas a recursos en Recursos AEM, consulte [las etiquetas de uso para organizar recursos](https://helpx.adobe.com/experience-manager/6-5/assets/using/organize-assets.html#Usetagstoorganizeassets).

7. **Publique recursos (o colecciones) en Brand Portal**.\
   Cuando publica un recurso (o colección) en Brand Portal, la etiqueta adjunta también está disponible en Brand Portal.

   Para ver la etiqueta adjunta en el recurso (o colección) correspondiente en Brand Portal, inicie sesión en Brand Portal y seleccione el recurso. En la sección Propiedades, verá la etiqueta adjunta.

## Buscar Promocionar {#search-promote}

AEM Assets Brand Portal permite que los recursos específicos se conviertan en los principales resultados de las búsquedas basadas en una etiqueta de palabra clave.

Para elevar un recurso para una palabra clave de búsqueda, siga estos pasos:

1. Abra la página **[!UICONTROL Propiedades]** de un recurso en la instancia de autor de AEM.
2. Vaya a la ficha **[!UICONTROL Avanzado]** .
3. En **[!UICONTROL Buscar promoción]** dentro **[!UICONTROL de Elevar para palabras clave]** de búsqueda, seleccione **[!UICONTROL Agregar]** para agregar las etiquetas o palabras clave de búsqueda.

   ![](assets/search-promote.png)

4. Guarde los cambios.
5. Publicar el recurso en el portal de marca.
6. Inicie sesión en Brand Portal. Consulte **[!UICONTROL la ficha Avanzado]** en **[!UICONTROL la sección Propiedades]** del recurso.
Tenga en cuenta que la palabra clave **[!UICONTROL Search Promote]** también está visible en las propiedades de dicho recurso.
