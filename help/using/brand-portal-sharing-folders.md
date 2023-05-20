---
title: Compartir carpetas
seo-title: Share folders
description: Brand Portal no admite la ingesta de recurso para que activos se publique en Brand portal desde una Experience Manager Assets Autor preconfigurado. Activos publicados no son accesibles para los usuarios que no son administradores de Brand portal, a menos que se configuran al configurar la replicación con Experience Manager instancia, y deben compartirse con ellos.
seo-description: Brand Portal does not support asset ingestion so assets must be published to Brand Portal from a pre-configured Experience Manager Assets Author instance. Published assets are not accessible to non-admin users of Brand Portal, unless configured while configuring replication with Experience Manager instance, and need to be shared with them.
uuid: 340d0a49-b708-4f0e-9fb8-99c824942f34
content-type: reference
topic-tags: sharing
products: SG_EXPERIENCEMANAGER/Brand_Portal
discoiquuid: 2332c16f-40be-4673-8cc6-2360d5b74116
exl-id: d28cf927-60e8-437e-9cba-92f7e19020e7
source-git-commit: 4caa4263bd74b51af7504295161c421524e51f0c
workflow-type: tm+mt
source-wordcount: '1109'
ht-degree: 2%

---

# Compartir carpetas en Brand portal {#share-folders}

Assets deben publicarse en Brand portal desde una Experience Manager Autor instancia preconfigurado, ya que el portal de marca no admite la ingesta de recurso.

## Carpeta compartir flujo de trabajo en Brand portal {#folder-sharing-workflow-in-brand-portal}

A continuación se describe la flujo de trabajo de uso compartido de carpetas y el acceso usuario:

* De forma predeterminada, todas las carpetas publicadas desde Experience Manager Assets en Brand portal solo son visibles para el administrador de Brand portal, a menos que se marquen como públicas al configurar la duplicación.
* El administrador utiliza la **[!UICONTROL consola de propiedades]** de carpeta para compartir una carpeta con usuarios o grupos selectivos. Solo los usuarios o grupos con los que se comparte la carpeta pueden ver la carpeta después de iniciar sesión en Brand portal. La carpeta no es visible para otros usuarios.
* El administrador también puede optar por convertir una carpeta en pública mediante la **[!UICONTROL casilla de verificación pública carpeta]** de la **[!UICONTROL consola carpeta propiedades]** . Una carpeta pública es visible para todos los usuarios.

* Independientemente de las funciones y los privilegios de los usuarios, cuando estos inician sesión en Brand Portal, ven todas las carpetas públicas y las que se comparten directamente con ellos o con un grupo al que pertenecen. Las carpetas privadas o las carpetas compartidas con otros usuarios no son visibles para todos los usuarios.

### Compartir carpetas con grupos de usuarios en Brand Portal {#sharing-folders-with-user-groups-on-brand-portal}

Los derechos de acceso a los recursos de una carpeta dependen de los derechos de acceso de su carpeta principal, independientemente de la configuración de las carpetas secundarias. Este comportamiento se rige por [ACL](https://experienceleague.adobe.com/docs/experience-manager-65/administering/security/security.html?lang=es) AEM en la práctica, las carpetas secundarias heredan las ACL de sus carpetas principales. Por ejemplo, si una carpeta A contiene la carpeta B que contiene la carpeta C, una grupo de usuarios (o usuarios) con derechos de acceso en la carpeta A también tienen los mismos derechos de acceso en la carpeta B y en la carpeta C. Carpeta B es la carpeta secundaria de A hereda sus ACL y la carpeta C es la carpeta secundaria de B hereda sus ACL.

Del mismo modo, usuario grupos (o usuarios) que tienen permisos para acceder únicamente a la carpeta B tienen los mismos permisos de acceso en la carpeta C pero no en la carpeta A. Por lo tanto, se recomienda que las organizaciones organicen sus contenido de forma que la mayoría de las activos expuestas se encuentren en la carpeta de elementos secundarios y que se pueda restringir el acceso de elementos secundarios a la carpeta raíz.

### publicar de carpetas públicas {#public-folder-publish}

A menos que se seleccione la opción pública Carpeta Publish ]**al configurar la**[!UICONTROL  replicación de Brand portal, los usuarios que no son administradores (como editores y visores) no tienen acceso a activos publicados de recursos AEM en el portal de marca.

![](assets/assetbpreplication.png)

Si la **[!UICONTROL opción pública Carpeta Publish]** está deshabilitada, los administradores deben compartir estas activos con usuarios que no sean administradores mediante la capacidad de compartir.

>[!NOTE]
>
>La opción de habilitar **[!UICONTROL la carpeta pública Publish]** está disponible en AEM 6.3.2.1.

## Acceso a carpetas compartidas {#access-to-shared-folders}

La siguiente matriz analiza los derechos de acceso y los derechos para compartir/anular uso compartido activos para diversas funciones de usuario:

|  | Acceso a todas las carpetas publicadas desde Recursos AEM a Brand portal | Acceso a carpetas compartidas | Derechos de carpetas compartidas/anular uso compartido |
|---------------|-----------|-----------|------------|
| Administrador | Sí | Sí | Sí |
| Editor | No* | Sí, solo si se comparten con ellos o con los grupo a los que pertenecen. | Sí, solo para las carpetas compartidas con ellas o con la grupo a la que pertenecen. |
| Visor | No* | Sí, solo si se comparte con ellos o con el grupo al que pertenecen | No |
| Usuario invitado | No* | Sí, solo si se comparten con ellos o con los grupo a los que pertenecen. | No |

>[!NOTE]
>
>De forma predeterminada, la opción pública Carpeta Publish ]**está deshabilitada al configurar la**[!UICONTROL  replicación de Brand Portal con AEM autor. Si la opción está activada, las carpetas publicadas en Brand portal serán accesibles para todos los usuarios (también usuarios que no son administradores) de forma predeterminada.

### Acceso a carpetas compartidas que no son administradores usuario {#non-admin-user-access-to-shared-folders}

Los usuarios que no sean administradores solo pueden acceder a las carpetas compartidas con ellas en Brand portal. No obstante, el modo en que se muestran estas carpetas en el portal cuando inician sesión depende de la configuración de habilitar Carpeta configuración de **[!UICONTROL jerarquía]** .

**Si la configuración está desactivada**

Los usuarios que no son administradores ven todas las carpetas compartidas con ellas en página de aterrizaje, en registro en el portal de marca.

![](assets/disabled-folder-hierarchy1-1.png)

**Si la configuración está habilitada**

Los usuarios no administradores ven el árbol de carpetas (a partir de la carpeta raíz) y las carpetas compartidas organizadas dentro de sus respectivas carpetas principales al iniciar sesión en Brand Portal.

Estas carpetas principales son las carpetas virtuales y no se pueden realizar acciones en ellas. Puede reconocer estas carpetas virtuales con un icono de candado.

No hay tareas de acción visibles al pasar el ratón por encima o seleccionarlas en **[!UICONTROL Vista de tarjeta]**, a diferencia de las carpetas compartidas. **[!UICONTROL Información general]** se muestra al seleccionar una carpeta virtual en **[!UICONTROL Vista de columna]** y **[!UICONTROL Vista de lista]**.

>[!NOTE]
>
>Tenga en cuenta que la miniatura predeterminada de las carpetas virtuales es la imagen en miniatura de la primera carpeta compartida.

![](assets/enabled-hierarchy1-1.png) ![](assets/hierarchy1-nonadmin-1.png) ![](assets/hierarchy-nonadmin-1.png) ![](assets/hierarchy2-nonadmin-1.png)

## Compartir carpetas {#how-to-share-folders}

Para compartir una carpeta con usuarios de Brand portal, seguir estos pasos:

1. Haga clic en el icono superposición de la izquierda y seleccione **[!UICONTROL navegación]** .

   ![](assets/selectorrail.png)

1. En el siderail de la izquierda, seleccione **[!UICONTROL archivos]** .

   ![](assets/access_files.png)

1. En la interfaz de Brand portal, seleccione la carpeta que desee compartir.

   ![](assets/share-folders.png)

1. En la barra de herramientas de la parte superior, seleccione **[!UICONTROL compartir]** .

   ![](assets/share_icon.png)

   Se abre la consola de Propiedades ] de [!UICONTROL  carpeta.

   ![](assets/folder_properties.png)

1. En la **[!UICONTROL consola propiedades]** de carpeta, especifique el título de la carpeta en el **[!UICONTROL campo carpeta título]** si no desea que el nombre predeterminado se muestre a los usuarios.
1. En el **[!UICONTROL lista de usuario]** añadir, seleccione los usuarios o grupos con los que desee compartir la carpeta y haga clic en **[!UICONTROL añadir]** .
Para compartir la carpeta solo con usuarios invitados y sin otros usuarios, seleccione **[!UICONTROL usuarios]** anónimos en la **[!UICONTROL lista desplegable miembros]** .

   ![](assets/only-anonymous.png)

   >[!NOTE]
   >
   >Para hacer que la carpeta esté disponible para todos los usuarios independientemente de su miembros del grupo y función, haga pública la casilla de **[!UICONTROL verificación pública carpeta]** .

1. Si es necesario, haga clic en **[!UICONTROL cambiar miniatura]** para modificar la imagen en miniatura de la carpeta.
1. Haga clic en **[!UICONTROL Guardar]**.

1. Para acceder a la carpeta compartida, inicie sesión en Brand portal con las credenciales de la usuario donde compartió la carpeta. Revise la carpeta compartida en la interfaz.

## Dejar de compartir carpetas {#unshare-the-folders}

Para anular uso compartido una carpeta compartida anteriormente, seguir estos pasos:

1. En la interfaz de Brand portal, seleccione la carpeta que desee anular uso compartido.

   ![](assets/share-folders-1.png)

1. En la barra de herramientas de la parte superior, haga clic en **[!UICONTROL Compartir]**.
1. En el **[!UICONTROL Propiedades de carpeta]** consola, en **[!UICONTROL Miembros]**, haga clic en **[!UICONTROL x]** símbolo situado junto a un usuario para quitarlo de la lista de usuarios con los que compartió la carpeta.

   ![](assets/folder_propertiesunshare.png)

1. En el cuadro de mensaje de advertencia, haga clic en **[!UICONTROL Confirmar]** para confirmar que no se comparte.
Haga clic en **[!UICONTROL Guardar]**.

1. Inicie sesión en Brand Portal con las credenciales del usuario que eliminó de la lista compartida. La carpeta ya no está disponible en la interfaz de Brand Portal para el usuario.
