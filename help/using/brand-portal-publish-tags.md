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
source-git-commit: 32c3cdb8e3fafd74cfb36e6bcfe0811e7152b2d0

---


# Publish tags to Brand Portal {#publish-tags-to-brand-portal}

Descubra cómo publicar etiquetas de [!DNL AEM] Recursos en [!DNL Brand Portal].

Las etiquetas son útiles para organizar recursos y mejorar la búsqueda de recursos a los que están asociados. Las etiquetas se pueden considerar como palabras clave o etiquetas (metadatos) que se adjuntan con recursos y permiten que los recursos se encuentren rápidamente como resultado de una búsqueda. Para saber cómo asignar etiquetas a recursos en [!DNL AEM] Recursos, consulte las etiquetas [de uso para organizar los recursos](https://helpx.adobe.com/experience-manager/6-5/assets/using/organize-assets.html#Usetagstoorganizeassets).

Las etiquetas (asociadas con recursos y colecciones en [!DNL AEM]) se publican automáticamente [!DNL Brand Portal] cuando se publican los recursos (y colecciones) con etiquetas asociadas [!DNL Brand Portal]. Las etiquetas publicadas son útiles para habilitar las búsquedas a fin de encontrar los activos asociados.

>[!NOTE]
>
>Sin embargo, se recomienda publicar exclusivamente etiquetas antes [!DNL Brand Portal] de publicar los recursos (y colecciones) con los que están asociados las etiquetas. Esto garantiza la publicación rápida de recursos (y colecciones) en [!DNL Brand Portal].

## Manage tags {#manage-tags}

Puede utilizar las etiquetas preexistentes para adjuntar a un recurso o crear nuevas etiquetas desde la consola [!DNL AEM] Etiquetas (**Herramientas | Etiquetado |[!DNL AEM]Etiquetas**). En ambos casos, primero debe publicar las etiquetas y [!DNL Brand Portal] asociarlas a los recursos correspondientes.

Para crear etiquetas en [!DNL AEM], publicar las etiquetas y [!DNL Brand Portal]asociar las etiquetas con los recursos (o colecciones) adecuados, siga estos pasos:

1. **Cree Etiquetas**
de inicio de sesión en [!DNL AEM] la instancia de Autor con privilegios administrativos y acceda **[!DNL AEM]a la consola Etiquetas** desde la navegación global:

   1. Seleccionar **herramientas**

   2. Seleccionar **general**

   3. Seleccionar **etiquetado**

2. Seleccione **Crear** y, a continuación, seleccione **Crear etiqueta** .
3. Especifique:

   * **Título**
      *(requerido)* Un título para la etiqueta.
   * **Nombre**
      *(requerido)* Un nombre para la etiqueta. Si no se especifica, se crea un nombre de nodo válido a partir del Título. Consulte [tagid](https://helpx.adobe.com/experience-manager/6-5/sites/developing/using/framework.html#TagID).
   * **Descripción**
      *(opcional)* Descripción de la etiqueta.
   * **Ruta de etiqueta**JCR de ruta
de la etiqueta.

4. Seleccione **Enviar** para crear la etiqueta.

   Una vez creada una etiqueta en [!DNL AEM] la instancia, la etiqueta estará disponible para adjuntarse a un recurso (mediante la sección Propiedades o la sección Administrar etiquetas de ese recurso).

5. **Publique la etiqueta en[!DNL Brand Portal]**.

   Ir a **[!DNL AEM]la consola Etiquetas** (Herramientas | Etiquetado | [!DNL AEM] Etiquetas), seleccione la etiqueta y Publicar en **[!DNL Brand Portal]**.

6. **Adjunte la etiqueta a un recurso (o colección)**.

   Seleccione un recurso (o colección) y adjunte la etiqueta que desee mediante la sección Propiedades o la sección Administrar etiquetas de dicho recurso. Para obtener más información sobre cómo asignar etiquetas a recursos en [!DNL AEM] Recursos, consulte [las etiquetas de uso para organizar los recursos](https://helpx.adobe.com/experience-manager/6-5/assets/using/organize-assets.html#Usetagstoorganizeassets).

7. **Publicar recursos (o colecciones) en[!DNL Brand Portal]**.\
   Cuando publica un recurso (o colección) en [!DNL Brand Portal], también está disponible la etiqueta adjunta.[!DNL Brand Portal]

   Para ver la etiqueta adjunta en el recurso correspondiente (o colección) en [!DNL Brand Portal], inicie sesión en [!DNL Brand Portal] el recurso y selecciónelo, en la sección Propiedades verá la Etiqueta adjunta.

## Buscar Promocionar {#search-promote}

[!DNL AEM] Los recursos [!DNL Brand Portal] le permiten proporcionar recursos específicos como resultados principales para búsquedas basadas en una etiqueta de palabra clave.

Para elevar un recurso para una palabra clave de búsqueda, siga estos pasos:

1. Abra la página **Propiedades** de un recurso en [!DNL AEM] la instancia de creación.
2. Vaya a la ficha **Avanzado** .
3. En **Buscar promoción** dentro **de Elevar para palabras clave** de búsqueda, seleccione **Agregar** para agregar las etiquetas o palabras clave de búsqueda.

   ![](assets/search-promote.png)

4. Guarde los cambios.
5. Publique el recurso en [!DNL Brand Portal].
6. Inicie sesión [!DNL Brand Portal]. Consulte **la ficha Avanzado** en **la sección Propiedades** del recurso.
Tenga en cuenta que la palabra clave **Search Promote** también está visible en las propiedades de dicho recurso.
