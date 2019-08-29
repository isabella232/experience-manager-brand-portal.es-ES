---
title: Compartir una colección
seo-title: Compartir una colección
description: Los administradores de AEM Assets Brand Portal pueden compartir y dejar de compartir una colección o una colección inteligente con usuarios autorizados. Los editores pueden ver y compartir únicamente las colecciones creadas por ellos, compartidas con ellos y colecciones públicas.
seo-description: Los administradores de AEM Assets Brand Portal pueden compartir y dejar de compartir una colección o una colección inteligente con usuarios autorizados. Los editores pueden ver y compartir únicamente las colecciones creadas por ellos, compartidas con ellos y colecciones públicas.
uuid: 965 f 39 cd -1378-42 c 1-a 58 a -01 e 1 bf 825 aa 3
contentOwner: bdhar
content-type: referencia
topic-tags: compartir
products: SG_ EXPERIENCEMANAGER/Brand_ Portal
discoiquuid: f 053013 e -5981-419 f -927 e-b 5 bb 1 d 47 eae 2
translation-type: tm+mt
source-git-commit: 0b70e82d034ce56fcfc5b49396e6d3a9da4b49d4

---


# Uso compartido de colecciones en Brand Portal {#share-collections-bp}

Los administradores de AEM Assets Brand Portal pueden compartir y dejar de compartir una colección o una colección inteligente con usuarios autorizados. Los editores pueden ver y compartir únicamente las colecciones creadas por ellos, compartidas con ellos y colecciones públicas. Sin embargo, los editores no pueden cambiar una colección pública a una colección no pública.

>[!NOTE]
>
>Los editores no pueden cambiar una colección pública a una colección no pública y, por lo tanto, no tienen la casilla **de verificación Colección** pública disponible en **el cuadro de** diálogo Configuración de la colección.

## Compartir una colección {#share-collection}

Para compartir una colección, siga estos pasos:

1. Haga clic en el icono de superposición a la izquierda y elija **Navegación**.

   ![](assets/contenttree-1.png)

1. En el sideril de la izquierda, haga clic **en Colecciones**.

   ![](assets/access_collections.png)

1. Desde la **consola Colecciones** , realice una de las siguientes acciones:

   * Sitúe el puntero sobre la colección que desee compartir. Desde las miniaturas de acción rápida disponibles para la colección, haga clic en el icono **Configuración** .
   ![](assets/settings_thumbnail.png)

   * Seleccione la colección que desee compartir. En la barra de herramientas de la parte superior, haga clic **en Configuración**.
   ![](assets/collection-sharing.png)

1. En el **cuadro de** diálogo Configuración de la colección, seleccione los usuarios o grupos con los que desee compartir la colección y seleccione la función para un usuario o grupo que coincida con su función global. Por ejemplo, asigne la función Editor a un editor global, la función Visor a un visor global.

   Como alternativa, para que la colección esté disponible para todos los usuarios, independientemente de su pertenencia y función, haga pública la casilla **de** verificación Colección pública.

   >[!NOTE]
   >
   >Sin embargo, los usuarios no administradores pueden no crear colecciones públicas, para evitar tener varias colecciones públicas, a fin de guardar el espacio del sistema. Las organizaciones pueden desactivar la configuración **de creación** de colecciones públicas desde la configuración **General** disponible en el panel de herramientas de administración.

   ![](assets/collection_sharingadduser.png)

   Los editores no pueden cambiar una colección pública a una colección no pública y, por lo tanto, no tienen la casilla **de verificación Colección** pública disponible en **el cuadro de** diálogo Configuración de la colección.

   ![](assets/collection-setting-editor.png)

1. Haga clic **en Agregar** y, a continuación, **en Guardar**. La colección se comparte con los usuarios elegidos.

   >[!NOTE]
   >
   >La función de un usuario rige el acceso a los recursos y carpetas dentro de una colección. Si un usuario no tiene acceso a los recursos, se comparte una colección vacía con el usuario. Además, la función de un usuario rige las acciones disponibles para las colecciones.

## Dejar de compartir una colección {#unshare-a-collection}

Para dejar de compartir una colección compartida anteriormente, haga lo siguiente:

1. Desde la consola **Colecciones** , seleccione la colección que desee dejar de compartir.

   In the toolbar, click **Settings**.

   ![](assets/collection_settings.png)

1. En el **cuadro de** diálogo Configuración de la colección, en **Miembros**, haga clic en el símbolo **X** junto a usuarios o grupos para quitarlos de la lista de usuarios con los que compartió la colección.

   ![](assets/unshare_collection.png)

1. En el cuadro de mensaje de advertencia, haga clic **en Confirmar** para confirmar que no se comparte.

   Haga clic en **Guardar**.

1. Inicie sesión en Brand Portal con las credenciales del usuario que ha eliminado de la lista compartida. La colección se elimina de la **consola Colecciones** .
