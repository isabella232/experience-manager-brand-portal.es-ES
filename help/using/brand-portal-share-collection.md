---
title: Compartir una colección
seo-title: Compartir una colección
description: Los administradores de AEM Assets Brand Portal pueden compartir y dejar de compartir una colección o una colección inteligente con usuarios autorizados. Los editores solo pueden ver y compartir las colecciones creadas por ellos, compartidas con ellos y las colecciones públicas.
seo-description: Los administradores de AEM Assets Brand Portal pueden compartir y dejar de compartir una colección o una colección inteligente con usuarios autorizados. Los editores solo pueden ver y compartir las colecciones creadas por ellos, compartidas con ellos y las colecciones públicas.
uuid: 965f39cd-1378-42c1-a58a-01e1bf825aa3
contentOwner: bdhar
content-type: reference
topic-tags: sharing
products: SG_EXPERIENCEMANAGER/Brand_Portal
discoiquuid: f053013e-5981-419f-927e-b5bb1d47eae2
translation-type: tm+mt
source-git-commit: 86078dd07b5d487f8cf5cd08bc46e4745529c873

---


# Uso compartido de colecciones en Brand Portal {#share-collections-bp}

Los administradores de AEM Assets Brand Portal pueden compartir y dejar de compartir una colección o una colección inteligente con usuarios autorizados. Los editores solo pueden ver y compartir las colecciones creadas por ellos, compartidas con ellos y las colecciones públicas. Sin embargo, los editores no pueden cambiar una colección pública a una colección no pública.

>[!NOTE]
>
>Los editores no pueden cambiar una colección pública a una colección no pública y, por lo tanto, no tienen la casilla Colección ****pública disponible en el cuadro de diálogo Configuración**[!UICONTROL  de]** colección.

## Compartir una colección {#share-collection}

Para compartir una colección, siga estos pasos:

1. Haga clic en el icono de superposición de la izquierda y elija **[!UICONTROL Navegación]**.

   ![](assets/contenttree-1.png)

1. Desde el lateral de la izquierda, haga clic en **[!UICONTROL Colecciones]**.

   ![](assets/access_collections.png)

1. Desde la consola **[!UICONTROL Colecciones]**, realice una de las siguientes acciones:

   * Pase el puntero sobre la colección que desee compartir. En las miniaturas de acción rápida disponibles para la colección, haga clic en el icono **[!UICONTROL Configuración]**.
   ![](assets/settings_thumbnail.png)

   * Seleccione la colección que desee compartir. En la barra de herramientas de la parte superior, haga clic en **[!UICONTROL Configuración]**.
   ![](assets/collection-sharing.png)

1. En el cuadro de diálogo Configuración [!UICONTROL de] colección, seleccione los usuarios o grupos con los que desea compartir la colección y seleccione la función de un usuario o grupo para que coincida con su función global. Por ejemplo, asigne la función Editor a un editor global y la función Visor a un visor global.

   Como alternativa, para que la colección esté disponible para todos los usuarios, independientemente de la pertenencia y función de su grupo, haga que se haga pública activando la casilla de verificación Colección ****pública.

   >[!NOTE]
   >
   >Sin embargo, los usuarios que no son administradores no pueden crear colecciones públicas para evitar tener muchas colecciones públicas y así poder guardar el espacio del sistema. Las organizaciones pueden desactivar la configuración **[!UICONTROL Permitir la creación]**de colecciones públicas desde la configuración[!UICONTROL General]disponible en el panel Herramientas de administración.

   ![](assets/collection_sharingadduser.png)

   Los editores no pueden cambiar una colección pública a una colección no pública y, por lo tanto, no tienen la casilla de verificación Colección ****pública disponible en el cuadro de diálogo Configuración**[!UICONTROL  de]** colección.

   ![](assets/collection-setting-editor.png)

1. Seleccione **[!UICONTROL Agregar]**y, a continuación,**[!UICONTROL  Guardar]**. La colección se comparte con los usuarios seleccionados.

   >[!NOTE]
   >
   >La función de usuario rige el acceso a los recursos y carpetas de una colección. Si un usuario no tiene acceso a los recursos, se comparte una colección vacía con el usuario. Además, la función de un usuario rige las acciones disponibles para las colecciones.

## Dejar de compartir una colección {#unshare-a-collection}

Para dejar de compartir una colección compartida anteriormente, haga lo siguiente:

1. En la consola **[!UICONTROL Colecciones]**, seleccione la colección que desee dejar de compartir.

   In the toolbar, click **[!UICONTROL Settings]**.

   ![](assets/collection_settings.png)

1. En el cuadro de diálogo Configuración **[!UICONTROL de]**colección, en**[!UICONTROL  Miembros]**, haga clic en el símbolo **[!UICONTROL x]**junto a usuarios o grupos para eliminarlos de la lista de usuarios con los que ha compartido la colección.

   ![](assets/unshare_collection.png)

1. En el cuadro de mensaje de advertencia, haga clic en **[!UICONTROL Confirmar]**para confirmar que no se comparte.

   Haga clic en **[!UICONTROL Guardar]**.

1. Inicie sesión en Brand Portal con las credenciales del usuario que ha eliminado de la lista compartida. La colección se elimina de la consola **[!UICONTROL Colecciones]**.
