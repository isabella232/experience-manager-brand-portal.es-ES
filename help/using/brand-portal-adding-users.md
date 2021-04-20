---
title: Administrar usuarios, grupos y funciones de usuario
seo-title: Administrar usuarios, grupos y funciones de usuario
description: Los administradores pueden usar Adobe Admin Console para crear usuarios y perfiles de producto de AEM Assets Brand Portal y administrar sus funciones mediante la interfaz de usuario de Brand Portal. Este privilegio no está disponible para los visualizadores y editores.
seo-description: Los administradores pueden usar Adobe Admin Console para crear usuarios y perfiles de producto de AEM Assets Brand Portal y administrar sus funciones mediante la interfaz de usuario de Brand Portal. Este privilegio no está disponible para los visualizadores y editores.
uuid: 0dc1867c-6d1b-4d0d-a25e-0df207c269b8
content-type: reference
topic-tags: administration
products: SG_EXPERIENCEMANAGER/Brand_Portal
discoiquuid: ba468e80-d077-4af6-b782-238fc557e22b
role: Administrator
translation-type: tm+mt
source-git-commit: 263653916e4bc183827c197c3beb137c9e59ccb1
workflow-type: tm+mt
source-wordcount: '2210'
ht-degree: 0%

---


# Administrar usuarios, grupos y funciones de usuario {#manage-users-groups-and-user-roles}

Los administradores pueden usar Adobe Admin Console para crear usuarios y perfiles de producto de AEM Assets Brand Portal y administrar sus funciones mediante la interfaz de usuario de Brand Portal. Este privilegio no está disponible para los visualizadores y editores.

En [[!UICONTROL Admin Console]](http://adminconsole.adobe.com/enterprise/overview), puede ver todos los productos asociados con su organización. Un producto puede ser cualquier solución de Experience Cloud, como Adobe Analytics, Adobe Target o AEM Brand Portal. Debe elegir el producto AEM Brand Portal y crear perfiles de producto.

<!--
Comment Type: draft

<note type="note">
<p>Product Profiles (formerly known as product configurations*). </p>
<p>* The nomenclature has changed from product configurations to product profiles in the new Adobe Admin Console.</p>
</note>
-->
![](assets/create-user-group.png)

Estos perfiles de producto se sincronizan con la interfaz de usuario de Brand Portal cada 8 horas y se pueden ver como grupos en Brand Portal. Una vez que agregue usuarios y cree perfiles de producto, y agregue usuarios a esos perfiles de producto, puede asignar funciones a usuarios y grupos en Brand Portal.

>[!NOTE]
>
>Para crear grupos en Brand Portal, desde el Adobe [!UICONTROL Admin Console], utilice **[!UICONTROL Productos > Perfiles de producto]**, en lugar de **[!UICONTROL Página de usuario > Grupos de usuarios]**. Los perfiles de producto del Adobe [!UICONTROL Admin Console] se utilizan para crear grupos en Brand Portal.

## Agregar un usuario {#add-a-user}

Si es administrador de productos, utilice el Adobe [[!UICONTROL Admin Console]](http://adminconsole.adobe.com/enterprise/overview) para crear usuarios y asignarlos a perfiles de producto (*anteriormente conocidos como configuraciones de producto*), que se muestran como grupos en Brand Portal. Puede utilizar grupos para realizar operaciones masivas, como la administración de funciones y el uso compartido de recursos.

>[!NOTE]
>
>Los nuevos usuarios que no tengan acceso a Brand Portal pueden solicitar acceso desde la pantalla de inicio de sesión de Brand Portal. Para obtener más información, consulte [Solicitud de acceso a Brand Portal](../using/brand-portal.md#request-access-to-brand-portal). Después de recibir notificaciones de solicitud de acceso en el área de notificación, haga clic en la notificación correspondiente y, a continuación, haga clic en **[!UICONTROL Conceder acceso]**. Como alternativa, siga el vínculo en el correo electrónico de solicitud de acceso recibido. A continuación, para agregar un usuario a través del [Adobe [!UICONTROL Admin Console]](http://adminconsole.adobe.com/enterprise/overview), siga los pasos 4 a 7 del procedimiento que se muestra a continuación.

>[!NOTE]
>
>Puede iniciar sesión en [Adobe [!UICONTROL Admin Console]](http://adminconsole.adobe.com/enterprise/overview) directamente o desde Brand Portal. Si inicia sesión directamente, siga los pasos 4-7 del procedimiento que se muestra a continuación para agregar un usuario.

1. En la barra de herramientas AEM de la parte superior, haga clic en el logotipo de Adobe para acceder a las herramientas administrativas.

   ![Logotipo de AEM](assets/aemlogo.png)

1. En el panel de herramientas administrativas, haga clic en **[!UICONTROL Usuarios]**.

   ![Panel de herramientas de administración](assets/admin-tools-panel-5.png)

1. En la página [!UICONTROL Funciones de usuario], haga clic en la pestaña **[!UICONTROL Administración]** y, a continuación, haga clic en **[!UICONTROL Iniciar Admin Console]**.

   ![Funciones de usuario para iniciar el Admin Console](assets/launch_admin_console.png)

1. En Admin Console, realice una de las siguientes acciones para crear un nuevo usuario:

   * En la barra de herramientas de la parte superior, haga clic en **[!UICONTROL Información general]**. En la página [!UICONTROL Información general], haga clic en **[!UICONTROL Asignar usuarios]** en la tarjeta de producto de Brand Portal.

   ![Información general del Admin Console](assets/admin_console_overviewadduser.png)

   * En la barra de herramientas de la parte superior, haga clic en **[!UICONTROL Usuarios]**. En la página [!UICONTROL Users], [!UICONTROL Users] en el carril izquierdo está seleccionado de forma predeterminada. Haga clic en **[!UICONTROL Agregar usuario]**.

   ![Admin Console Agregar usuarios](assets/admin_console_adduseruserpage.png)

1. En el cuadro de diálogo agregar usuario, escriba el ID de correo electrónico del usuario que desea agregar o selecciónelo en la lista de sugerencias que aparecen al escribir.

   ![Agregar usuario a Brand Portal](assets/add_user_to_aem_bp.png)

1. Asigne el usuario al menos a un perfil de producto (anteriormente conocido como configuración de producto) para que el usuario pueda acceder a Brand Portal. Seleccione el perfil de producto adecuado en el campo **[!UICONTROL Seleccione un perfil para este producto]**.
1. Haga clic en **[!UICONTROL Guardar]**. Se envía un correo electrónico de bienvenida al usuario que ha añadido. El usuario invitado puede acceder a Brand Portal haciendo clic en el vínculo del correo electrónico de bienvenida e iniciando sesión utilizando un [!UICONTROL Adobe ID]. Para obtener más información, consulte [Experiencia de inicio de sesión por primera vez](../using/brand-portal-onboarding.md).

   >[!NOTE]
   >
   >Si un usuario no puede iniciar sesión en Brand Portal, el administrador de la organización debe visitar el Adobe [!UICONTROL Admin Console] y comprobar si el usuario está presente y se ha agregado al menos a un perfil de producto.

   Para obtener información sobre la concesión de privilegios administrativos al usuario, consulte [Proporcionar privilegios de administrador a los usuarios](../using/brand-portal-adding-users.md#provideadministratorprivilegestousers).

## Añadir un perfil de producto {#add-a-product-profile}

Los perfiles de producto (anteriormente conocidos como configuraciones de producto) en [!UICONTROL Admin Console] se utilizan para crear grupos en Brand Portal, de modo que pueda realizar operaciones masivas como la administración de funciones y el uso compartido de recursos en Brand Portal. **Brand** Portal es el perfil de producto predeterminado disponible; puede crear más perfiles de producto y agregar usuarios a los nuevos perfiles de producto.

>[!NOTE]
>
>Puede iniciar sesión en [[!UICONTROL Admin Console]](http://adminconsole.adobe.com/enterprise/overview) directamente o desde Brand Portal. Si inicia sesión directamente en [!UICONTROL Admin Console], siga los pasos 4 a 7 del procedimiento siguiente para agregar un perfil de producto.

1. En la barra de herramientas AEM de la parte superior, haga clic en el logotipo de Adobe para acceder a las herramientas administrativas.

   ![Logotipo AEM](assets/aemlogo.png)

1. En el panel de herramientas administrativas, haga clic en **[!UICONTROL Usuarios]**.

   ![Panel de herramientas de administración](assets/admin-tools-panel-6.png)

1. En la página [!UICONTROL Funciones de usuario], haga clic en la pestaña **[!UICONTROL Administración]** y, a continuación, haga clic en **[!UICONTROL Iniciar Admin Console]**.

   ![Admin Console de Launch](assets/launch_admin_console.png)

1. En la barra de herramientas de la parte superior, haga clic en **[!UICONTROL Productos]**.
1. En la página [!UICONTROL Products], [!UICONTROL Product Profiles] está seleccionado de forma predeterminada. Haga clic en **[!UICONTROL Nuevo perfil]**.

   ![Añadir nuevo perfil de producto](assets/admin_console_addproductprofile.png)

1. En la página [!UICONTROL Crear un nuevo perfil], proporcione el nombre del perfil, el nombre para mostrar, la descripción del perfil y elija si desea notificar por correo electrónico a los usuarios cuando se agreguen o eliminen del perfil.

   ![Crear perfil de producto](assets/admin_console_addaproductprofilecreatenewprofile.png)

1. Haga clic en **[!UICONTROL Listo]**. El grupo de configuración de producto, por ejemplo **[!UICONTROL Sales group]**, se agrega a Brand Portal.

   ![Perfiles de producto](assets/admin_console_productprofileadded.png)

## Agregar usuarios a un perfil de producto {#add-users-to-a-product-profile}

Para agregar usuarios a un grupo de Brand Portal, agréguelos al perfil de producto correspondiente (anteriormente conocido como configuraciones de producto) en [!UICONTROL Admin Console]. Puede agregar usuarios de forma individual o en masa.

>[!NOTE]
>
>Puede iniciar sesión en [[!UICONTROL Admin Console]](http://adminconsole.adobe.com/enterprise/overview) directamente o desde Brand Portal. Si inicia sesión directamente en el Admin Console, siga los pasos 4 a 7 del procedimiento que se muestra a continuación para agregar usuarios a un perfil de producto.

1. En la barra de herramientas AEM de la parte superior, haga clic en el logotipo de Adobe para acceder a las herramientas administrativas.

   ![Logotipo AEM](assets/aemlogo.png)

1. En el panel de herramientas administrativas, haga clic en **[!UICONTROL Usuarios]**.

   ![Panel de herramientas de administración](assets/admin-tools-panel-7.png)

1. En la página [!UICONTROL Funciones de usuario], haga clic en la pestaña **[!UICONTROL Administración]** y, a continuación, haga clic en **[!UICONTROL Iniciar Admin Console]**.

   ![Iniciar [!DNL Admin Console]](assets/launch_admin_console.png)

1. En la barra de herramientas de la parte superior, haga clic en **[!UICONTROL Productos]**.
1. En la página [!UICONTROL Products], [!UICONTROL Product Profiles] está seleccionado de forma predeterminada. Abra el perfil de producto al que desee agregar un usuario, por ejemplo, [!UICONTROL Grupo de ventas].

   ![Perfiles de producto](assets/admin_console_productprofileadded.png)

1. Para agregar usuarios individuales al perfil del producto, haga lo siguiente:

   * Haga clic en **[!UICONTROL Agregar usuario]**.

   ![Grupo para asignar el perfil de producto en Brand Portal](assets/admin_console_productprofilesalesgroup.png)

   * En la página [!UICONTROL Agregar usuario al grupo de ventas], escriba el ID de correo electrónico del usuario que desea agregar o seleccione el usuario en la lista de sugerencias que aparecen a medida que escribe.

   ![Agregar un usuario a un grupo](assets/admin_console_addusertosalesgroup.png)

   * Haga clic en **[!UICONTROL Guardar]**.



1. Para agregar usuarios masivos al perfil del producto, haga lo siguiente:

   * Seleccione **[!UICONTROL puntos suspensivos (...) > Agregar usuarios mediante CSV]**.

   ![Agregar usuarios de forma masiva](assets/admin_console_addbulkusers.png)

   * En la página **[!UICONTROL Agregar usuarios mediante CSV]**, descargue una plantilla CSV o arrastre y suelte un archivo CSV.

   ![Agregar usuarios por csv](assets/admin_console_addbulkuserscsv.png)

   * Haga clic en **[!UICONTROL Cargar]**.
   Si agregó usuarios al perfil de producto predeterminado, es decir, a Brand Portal, se envía un correo electrónico de bienvenida al ID de correo electrónico de los usuarios agregados. Los usuarios invitados pueden acceder a Brand Portal haciendo clic en el vínculo del correo electrónico de bienvenida e iniciando sesión utilizando un [!UICONTROL Adobe ID]. Para obtener más información, consulte [Experiencia de inicio de sesión por primera vez](../using/brand-portal-onboarding.md).

   Los usuarios añadidos a un perfil de producto personalizado o nuevo no reciben notificaciones por correo electrónico.

## Proporcionar privilegios de administrador a los usuarios {#provide-administrator-privileges-to-users}

Puede proporcionar el privilegio de administrador del sistema o administrador del producto a un usuario de Brand Portal. No proporcione otros derechos administrativos disponibles en [!UICONTROL Admin Console], como administrador de perfiles de producto, administrador de grupos de usuarios y administrador de asistencia. Para obtener más información sobre estas funciones, consulte [Funciones administrativas](https://helpx.adobe.com/enterprise/using/admin-roles.html).

>[!NOTE]
>
>Puede iniciar sesión en [[!UICONTROL Admin Console]](https://adminconsole.adobe.com/enterprise/overview) directamente o desde Brand Portal. Si inicia sesión directamente en [!UICONTROL Admin Console], siga los pasos 4 a 8 del procedimiento que se muestra a continuación para agregar un usuario a un perfil de producto.

1. En la barra de herramientas AEM de la parte superior, haga clic en el logotipo de Adobe para acceder a las herramientas administrativas.

   ![AEMLogo](assets/aemlogo.png)

1. En el panel de herramientas administrativas, haga clic en **[!UICONTROL Usuarios]**.

   ![Panel de herramientas de administración](assets/admin-tools-panel-8.png)

1. En la página [!UICONTROL Funciones de usuario], haga clic en la pestaña **[!UICONTROL Administración]** y, a continuación, haga clic en **[!UICONTROL Iniciar Admin Console]**.

   ![Admin Console de Launch](assets/launch_admin_console.png)

1. En la barra de herramientas de la parte superior, haga clic en **[!UICONTROL Usuarios]**.
1. En la página [!UICONTROL Users], [!UICONTROL Users] en el carril izquierdo está seleccionado de forma predeterminada. Haga clic en el nombre de usuario del usuario al que desea otorgar privilegios de administrador.

   ![Agregar usuarios en el Admin Console](assets/admin_console_adduseruserpage.png)

1. En la página de perfil del usuario, busque la sección **[!UICONTROL Derechos administrativos]** en la parte inferior y elija **[!UICONTROL puntos suspensivos (...) > Editar derechos de administrador]**.
   ![Derechos de administrador en el Admin Console](assets/admin_console_editadminrights.png)

1. En la página [!UICONTROL Editar administrador], seleccione Administrador del sistema o Administrador del producto.

   ![Editar derechos de administrador en Admin Console](assets/admin_console_editadminrightsselection.png)

   >[!NOTE]
   >
   >Brand Portal solo admite las funciones de administrador del sistema y administrador de productos.
   >
   >Adobe recomienda evitar el uso de la función de administrador del sistema porque otorga privilegios de administrador en toda la organización para todos los productos de una organización. Por ejemplo, un administrador del sistema de una organización que incluya tres productos de marketing cloud tiene todo el conjunto de privilegios para los tres productos. Solo los administradores del sistema pueden configurar AEM Assets para que los recursos se puedan publicar desde AEM Assets en Brand Portal. Para obtener más información, consulte [Configuración de AEM Assets con Brand Portal](../using/configure-aem-assets-with-brand-portal.md).
   >
   >Por el contrario, la función Administrador de productos concede privilegios de administrador para un producto específico. Si desea aplicar un control de acceso más granular en Brand Portal, utilice la función de administrador de productos y seleccione el producto como Brand Portal.

   >[!NOTE]
   >
   >Brand Portal no admite privilegios de administrador de perfiles de producto (anteriormente conocido como administrador de configuración). Evite asignar derechos de administrador de perfiles de producto a un usuario.

1. Revise la selección de tipo de administrador y haga clic en **[!UICONTROL Guardar]**.

   >[!NOTE]
   >
   >Para revocar los privilegios de administrador para un usuario, realice los cambios correspondientes en la página **[!UICONTROL Editar administrador]** y, a continuación, haga clic en **[!UICONTROL Guardar]**.


## Administrar funciones de usuario {#manage-user-roles}

Un administrador puede modificar las funciones de los usuarios en Brand Portal.

Además de la función de administrador, Brand Portal admite las siguientes funciones:

* [!UICONTROL Visor]: Los usuarios con esta función pueden ver los archivos y carpetas que un administrador comparte con ellos. Los visualizadores también pueden buscar y descargar recursos. Sin embargo, los visualizadores no pueden compartir contenido (archivos, carpetas, [!UICONTROL colecciones]) con otros usuarios.
* [!UICONTROL Editor]: Los usuarios con esta función tienen todos los privilegios de un visualizador. Además, los editores pueden compartir contenido (carpetas, [!UICONTROL colecciones], vínculos) con otros usuarios.

1. En la barra de herramientas AEM de la parte superior, haga clic en el logotipo de Adobe para acceder a las herramientas administrativas.

   ![AEMLogo](assets/aemlogo.png)

1. En el panel de herramientas administrativas, haga clic en **[!UICONTROL Usuarios]**.

   ![Panel de herramientas de administración](assets/admin-tools-panel-9.png)

1. En la página [!UICONTROL Funciones de usuario], la pestaña [!UICONTROL Usuarios] está seleccionada de forma predeterminada. Para el usuario cuya función desea cambiar, seleccione **[!UICONTROL Editor]** o **[!UICONTROL Visor]** en la lista desplegable **[!UICONTROL Función]**.

   ![Modificación de las funciones de los usuarios](assets/modify_user_role.png)

   Para modificar la función de varios usuarios simultáneamente, seleccione los usuarios y elija la función adecuada en la lista desplegable **[!UICONTROL Función]**.

   >[!NOTE]
   >
   >La lista [!UICONTROL Función] para usuarios administradores está deshabilitada. No puede seleccionar a estos usuarios para modificar sus funciones.


   >[!NOTE]
   >
   >La función de usuario también está deshabilitada si el usuario es miembro del grupo Editor. Para revocar los privilegios de edición del usuario, elimine el usuario del grupo Editor o cambie la función de todo el grupo a Visor.


1. Haga clic en **[!UICONTROL Guardar]**. La función se modifica para el usuario correspondiente. Si ha seleccionado varios usuarios, las funciones de todos los usuarios se modifican simultáneamente.

   >[!NOTE]
   >
   >Los cambios en los permisos de usuario se reflejan en la página **[!UICONTROL Funciones de usuario]** solo después de que los usuarios vuelvan a iniciar sesión en Brand Portal.

## Administrar roles y privilegios de grupo {#manage-group-roles-and-privileges}

Un administrador puede asociar privilegios específicos con un [grupo](../using/brand-portal-adding-users.md#main-pars-title-278567577) de usuarios en Brand Portal. La pestaña **[!UICONTROL Grupos]** de la página **[!UICONTROL Funciones de usuario]** permite a los administradores:

* Asignación de funciones a grupos de usuarios
* Restringir grupos de usuarios para descargar representaciones originales de archivos de imagen (.jpeg, .tiff, .png, .bmp, .gif, .pjpeg, x-portable-anymap, x-portable-bitmap, x-portable-graymap, x-portable-pixmap, x-rgb, x-xbitmap, x-xpixmap, x-icon, image/photoshop, image/x photoshop, .psd, image/vnd.adobe.photoshop) de Brand Portal.

>[!NOTE]
>
>Para los recursos compartidos como vínculo, el permiso para acceder a las representaciones originales de los archivos de imagen se aplicará en función de los permisos del usuario que comparte los recursos.

Para modificar la función y el derecho de acceso a las representaciones originales de miembros específicos del grupo, siga estos pasos:

1. En la página **[!UICONTROL Funciones de usuario]**, vaya a la pestaña **[!UICONTROL Grupos]**.
1. Seleccione los grupos para los que desee cambiar las funciones.
1. Seleccione la función adecuada en la lista desplegable **[!UICONTROL Función]**.

   Para permitir que los miembros de un grupo tengan acceso a las representaciones originales de archivos de imagen (.jpeg, .tiff, .png, .bmp, .gif, .pjpeg, x-portable-anymap, x-portable-bitmap, x-portable-graymap, x-portable-pixmap, x-rgb, x-xbitmap, x-xxxmap, x-icon, image/photoshop imagen/x-photoshop, .psd, image/vnd.adobe.photoshop) que descargan del portal o enlace compartido, mantenga seleccionada la opción **[!UICONTROL Acceso al original]** para ese grupo. De forma predeterminada, la opción **[!UICONTROL Access to Original]** está seleccionada para todos los usuarios. Para evitar que un grupo de usuarios acceda a las representaciones originales, anule la selección de la opción correspondiente a ese grupo.

   ![Funciones de grupo de usuarios](assets/access-original-rend.png)

   >[!NOTE]
   >
   >Si un usuario se agrega a varios grupos y uno de estos grupos tiene restricciones, las restricciones se aplicarán a ese usuario.
   >
   >Además, las restricciones para acceder a las representaciones originales de los archivos de imagen no se aplican a los administradores aunque sean miembros de grupos restringidos.


1. Haga clic en **[!UICONTROL Guardar]**. La función se modifica para los grupos correspondientes.

   >[!NOTE]
   >
   >La asociación de usuario a grupo, o la pertenencia a grupo de un usuario, se sincroniza con Brand Portal cada 8 horas. Los cambios en las funciones de usuario o grupo se aplican después de ejecutar el siguiente trabajo de sincronización.

