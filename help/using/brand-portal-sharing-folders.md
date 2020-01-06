---
title: Compartir carpetas
seo-title: Compartir carpetas
description: Brand Portal no admite la ingestión de recursos, por lo que los recursos deben publicarse en Brand Portal desde una instancia de AEM Author preconfigurada. Los recursos publicados no son accesibles para los usuarios no administradores de Brand Portal, a menos que estén configurados durante la configuración de la replicación con la instancia de AEM, y deben compartirse con ellos.
seo-description: Brand Portal no admite la ingestión de recursos, por lo que los recursos deben publicarse en Brand Portal desde una instancia de AEM Author preconfigurada. Los recursos publicados no son accesibles para los usuarios no administradores de Brand Portal, a menos que estén configurados durante la configuración de la replicación con la instancia de AEM, y deben compartirse con ellos.
uuid: 340d0a49-b708-4f0e-9fb8-99c824942f34
content-type: reference
topic-tags: sharing
products: SG_EXPERIENCEMANAGER/Brand_Portal
discoiquuid: 2332c16f-40be-4673-8cc6-2360d5b74116
translation-type: tm+mt
source-git-commit: 86078dd07b5d487f8cf5cd08bc46e4745529c873

---


# Uso compartido de carpetas en Brand Portal {#share-folders}

Los recursos deben publicarse en Brand Portal desde una instancia de AEM Author preconfigurada, ya que Brand Portal no admite la ingestión de recursos.

## Flujo de trabajo de uso compartido de carpetas en Brand Portal {#folder-sharing-workflow-in-brand-portal}

A continuación se describe el flujo de trabajo de uso compartido de carpetas y el acceso del usuario:

* De forma predeterminada, todas las carpetas publicadas desde Recursos AEM a Brand Portal solo son visibles para el administrador de Brand Portal, a menos que estén marcadas como públicas al configurar la replicación.
* El administrador utiliza la consola Propiedades **[!UICONTROL de la]**carpeta para compartir una carpeta con usuarios o grupos determinados. Solo los usuarios o grupos con los que se comparte la carpeta pueden verla después de iniciar sesión en Brand Portal. La carpeta no está visible para otros usuarios.
* El administrador también puede optar por hacer pública una carpeta mediante la casilla de verificación Carpeta ****pública de la consola Propiedades**[!UICONTROL  de la]** carpeta. Todos los usuarios pueden ver una carpeta pública.

* Independientemente de las funciones de usuario y los privilegios, cuando los usuarios inician sesión en Brand Portal, verán todas las carpetas públicas y las carpetas que se hayan compartido directamente con ellos o con un grupo al que pertenezcan. Las carpetas privadas o las carpetas compartidas con otros usuarios no son visibles para todos los usuarios.

### Uso compartido de carpetas con grupos de usuarios en Brand Portal {#sharing-folders-with-user-groups-on-brand-portal}

Los derechos de acceso a los recursos de una carpeta dependen de los derechos de acceso de su carpeta principal, independientemente de la configuración de las carpetas secundarias. Este comportamiento se rige por [las ACL](https://helpx.adobe.com/experience-manager/6-5/sites/administering/using/security.html#PermissionsinAEM) en AEM, ya que las carpetas secundarias heredan las ACL de sus carpetas principales. Por ejemplo, si una carpeta A contiene la carpeta B que contiene la carpeta C, un grupo de usuarios (o usuarios) con derechos de acceso en la carpeta A también tendrá los mismos derechos de acceso en la carpeta B y la carpeta C. Si la carpeta B es la carpeta secundaria de A, heredará sus ACL y si la carpeta C es la carpeta secundaria de B, heredará las ACL.

Del mismo modo, los grupos de usuarios (o usuarios) que tienen permisos para acceder únicamente a la carpeta B tienen los mismos permisos de acceso en la carpeta C pero no en la carpeta A. Por lo tanto, se recomienda que las organizaciones organicen su contenido de manera que la mayoría de los recursos expuestos se coloquen en la carpeta de niños y se restrinja el acceso a la carpeta raíz desde los niños hasta los archivos secundarios.

### Public folder publish {#public-folder-publish}

A menos que se seleccione la opción Publicación **[!UICONTROL de carpetas]**públicas al configurar la replicación de Brand Portal, los usuarios no administradores (como editores y visores) no tendrán acceso a los recursos publicados desde Recursos AEM a Brand Portal.

![](assets/assetbpreplication.png)

Si la opción Publicación **[!UICONTROL de carpetas]**públicas está desactivada, los administradores deben compartir específicamente estos recursos con usuarios no administradores que utilicen la función de uso compartido.

>[!NOTE]
>
>La opción para activar Publicación **[!UICONTROL de carpetas]**públicas está disponible en AEM 6.3.2.1 y versiones posteriores.

## Acceso a carpetas compartidas {#access-to-shared-folders}

La siguiente matriz analiza los derechos y derechos de acceso para compartir o dejar de compartir recursos para diversas funciones de usuario:

|  | Acceso a todas las carpetas publicadas desde Recursos AEM en Brand Portal | Acceso a carpetas compartidas | Compartir/dejar de compartir derechos de carpeta |
|---------------|-----------|-----------|------------|
| Administrador | Sí | Sí | Sí |
| Editor | No* | Sí, solo si se comparten con ellos o con el grupo al que pertenecen | Sí, solo para las carpetas compartidas con ellos o con el grupo al que pertenecen |
| Visor | No* | Sí, solo si se comparten con ellos o con el grupo al que pertenecen | No |
| Usuario invitado | No* | Sí, solo si se comparten con ellos o con el grupo al que pertenecen | No |

**De forma predeterminada, la opción Publicación **[!UICONTROL de carpetas]**públicas está desactivada al configurar la replicación de Brand Portal con AEM Author. Si la opción está activada, todas las carpetas publicadas en Brand Portal estarán accesibles a todos los usuarios (también a los usuarios no administradores) de forma predeterminada.*

### Acceso de usuario no administrador a carpetas compartidas {#non-admin-user-access-to-shared-folders}

Los usuarios no administradores solo pueden acceder a las carpetas compartidas con ellos en Brand Portal. Sin embargo, el modo en que se muestran estas carpetas en el portal cuando inician sesión depende de la configuración de **[!UICONTROL Habilitar jerarquía]**de carpetas.

**Si la configuración está deshabilitada**

Los usuarios no administradores ven todas las carpetas compartidas con ellos en la página de aterrizaje al iniciar sesión en el portal de marca.

![](assets/disabled-folder-hierarchy1-1.png)

**Si la configuración está habilitada**

Los usuarios no administradores ven el árbol de carpetas (a partir de la carpeta raíz) y las carpetas compartidas organizadas dentro de sus respectivas carpetas principales al iniciar sesión en Brand Portal.

Estas carpetas principales son las carpetas virtuales y no se pueden realizar acciones en ellas. Puede reconocer estas carpetas virtuales con un icono de candado.

No hay tareas de acción visibles al pasar el ratón por encima o seleccionarlas en la vista **[!UICONTROL de]**tarjeta, a diferencia de las carpetas compartidas.**[!UICONTROL  El botón Información general]** se muestra al seleccionar una carpeta virtual en la Vista **[!UICONTROL de]**columna y en la Vista**[!UICONTROL  de]**lista.

>[!NOTE]
>
>Tenga en cuenta que la miniatura predeterminada de las carpetas virtuales es la imagen en miniatura de la primera carpeta compartida.

![](assets/enabled-hierarchy1-1.png) ![](assets/hierarchy1-nonadmin-1.png) ![](assets/hierarchy-nonadmin-1.png) ![](assets/hierarchy2-nonadmin-1.png)

## Compartir carpetas {#how-to-share-folders}

Para compartir una carpeta con los usuarios de Brand Portal, siga estos pasos:

1. Haga clic en el icono de superposición de la izquierda y elija **[!UICONTROL Navegación]**.

   ![](assets/selectorrail.png)

1. En el lateral de la izquierda, seleccione **[!UICONTROL Archivos]**.

   ![](assets/access_files.png)

1. En la interfaz de Brand Portal, seleccione la carpeta que desee compartir.

   ![](assets/share-folders.png)

1. En la barra de herramientas de la parte superior, seleccione **[!UICONTROL Compartir]**.

   ![](assets/share_icon.png)

   Aparece la consola Propiedades [!UICONTROL de la] carpeta.

   ![](assets/folder_properties.png)

1. En la consola Propiedades **[!UICONTROL de la]**carpeta, especifique el título de la carpeta en el campo Título**[!UICONTROL  de la]** carpeta si no desea que los usuarios vean el nombre predeterminado.
1. En la lista **[!UICONTROL Agregar usuario]**, seleccione los usuarios o grupos con los que desee compartir la carpeta y haga clic en**[!UICONTROL  Agregar]**.
Para compartir la carpeta solo con usuarios invitados y ningún otro usuario, seleccione Usuarios ****anónimos en el menú desplegable**[!UICONTROL  Miembros]** .

   ![](assets/only-anonymous.png)

   >[!NOTE]
   >
   >Para que la carpeta esté disponible para todos los usuarios, independientemente de la pertenencia y función del grupo, haga que se haga pública activando la casilla de verificación Carpeta ****pública.

1. Si es necesario, haga clic en **[!UICONTROL Cambiar miniatura]**para modificar la imagen en miniatura de la carpeta.
1. Haga clic en **[!UICONTROL Guardar]**.
1. Para acceder a la carpeta compartida, inicie sesión en Brand Portal con las credenciales del usuario con el que ha compartido la carpeta. Revise la carpeta compartida en la interfaz.

## Dejar de compartir carpetas {#unshare-the-folders}

Para dejar de compartir una carpeta compartida anteriormente, siga estos pasos:

1. En la interfaz de Brand Portal, seleccione la carpeta que desee dejar de compartir.

   ![](assets/share-folders-1.png)

1. En la barra de herramientas de la parte superior, haga clic en **[!UICONTROL Compartir]**.
1. En la consola Propiedades **[!UICONTROL de la]**carpeta, en**[!UICONTROL  Miembros]**, haga clic en el símbolo **[!UICONTROL x]**situado junto a un usuario para quitarlos de la lista de usuarios con los que ha compartido la carpeta.

   ![](assets/folder_propertiesunshare.png)

1. En el cuadro de mensaje de advertencia, haga clic en **[!UICONTROL Confirmar]**para confirmar que no se comparte.
Haga clic en**[!UICONTROL  Guardar]**.

1. Inicie sesión en Brand Portal con las credenciales del usuario que ha eliminado de la lista compartida. La carpeta ya no está disponible en la interfaz de Brand Portal para el usuario.
