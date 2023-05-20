---
title: Administrar usuarios, grupos y funciones de usuario
seo-title: Manage users, groups, and user roles
description: Los administradores pueden utilizar Adobe Admin Console para crear usuarios y perfiles de producto de Brand Portal y administrar sus funciones mediante la interfaz de usuario de Brand Portal. Este privilegio no está disponible para visores y editores.
seo-description: Administrators can use Adobe Admin Console to create Brand Portal users and product profiles, and manage their roles using the Brand Portal user interface. This privilege is not available to Viewers and Editors.
uuid: 0dc1867c-6d1b-4d0d-a25e-0df207c269b8
content-type: reference
topic-tags: administration
products: SG_EXPERIENCEMANAGER/Brand_Portal
discoiquuid: ba468e80-d077-4af6-b782-238fc557e22b
role: Admin
exl-id: 35b1fd75-f9e4-4145-80bd-84de091f8b2b
source-git-commit: 955cd8afe939ff47e9f08f312505e230e2f38495
workflow-type: tm+mt
source-wordcount: '2185'
ht-degree: 1%

---

# Administrar usuarios, grupos y funciones de usuario {#manage-users-groups-and-user-roles}

Los administradores pueden utilizar Adobe Admin Console para crear Experience Manager Assets usuarios de Brand portal y perfiles de productos, y administrar sus funciones con la interfaz de Brand portal usuario. Este privilegio no está disponible para los visualizadores y editores.

Entrada [[!UICONTROL Admin Console]](https://adminconsole.adobe.com/enterprise/overview), puede ver todos los productos asociados a su organización. Un producto puede ser cualquier solución de Experience Cloud, como Adobe Analytics, Adobe Target o Experience Manager Assets Brand Portal. Debe elegir el producto de AEM Brand Portal y crear perfiles de producto.

<!--
Comment Type: draft

<note type="note">
<p>Product Profiles (formerly known as product configurations*). </p>
<p>* The nomenclature has changed from product configurations to product profiles in the new Adobe Admin Console.</p>
</note>
-->
![](assets/create-user-group.png)

Estos perfiles de producto se sincronizan con la interfaz de usuario de Brand Portal cada 8 horas y son visibles como grupos en Brand Portal. Una vez que añada usuarios y cree perfiles de producto, y agregue usuarios a esos perfiles de producto, puede asignar funciones a usuarios y grupos en Brand Portal.

>[!NOTE]
>
>Para crear grupos en Brand portal, desde Adobe Systems [!UICONTROL  admin Console ] , utilice **[!UICONTROL productos > perfiles]** de producto, en lugar de grupos ]**de**[!UICONTROL  usuarios página >. Perfiles de producto en el Adobe [!UICONTROL Admin Console] se utilizan para crear grupos en Brand Portal.

## añadir una usuario {#add-a-user}

Si es un administrador de productos, utilice Adobe Systems [[!UICONTROL  admin Console ] ](https://adminconsole.adobe.com/enterprise/overview) para crear usuarios y asignarlos a perfiles de producto ( *antes denominados configuraciones* de producto), que se muestran como grupos en Brand portal. Puede utilizar grupos para realizar operaciones masivas, como la administración de función y el uso compartido de recurso.

>[!NOTE]
>
>Nuevo los usuarios que no tienen acceso a Brand portal pueden solicitud acceder desde la pantalla inicio de sesión del portal de marca. Para obtener más información, consulte [Solicitud de acceso a Brand Portal](../using/brand-portal.md#request-access-to-brand-portal). Después de recibir notificaciones de solicitud de acceso en el área de notificación, haga clic en la notificación correspondiente y, a continuación, haga clic en **[!UICONTROL Conceder acceso]**. También puede seguir el vínculo del correo electrónico de solicitud de acceso recibido. A continuación, para agregar un usuario mediante [Adobe [!UICONTROL Admin Console]](https://adminconsole.adobe.com/enterprise/overview), siga los pasos 4-7 del siguiente procedimiento.

>[!NOTE]
>
>Puede iniciar sesión en [Adobe [!UICONTROL Admin Console]](https://adminconsole.adobe.com/enterprise/overview) directamente o desde Brand Portal. Si inicia sesión directamente, siga los pasos 4-7 del procedimiento siguiente para agregar un usuario.

1. AEM En la barra de herramientas de la parte superior, haga clic en el logotipo del Adobe para acceder a las herramientas administrativas.

   ![AEM logotipo de la](assets/aemlogo.png)

1. En el panel de herramientas administrativas, haga clic en **[!UICONTROL Usuarios]**.

   ![Panel de herramientas de administración](assets/admin-tools-panel-5.png)

1. En el [!UICONTROL Funciones del usuario] , haga clic en **[!UICONTROL Administración]** y haga clic en **[!UICONTROL Admin Console de Launch]**.

   ![Roles de usuario para iniciar el Admin Console](assets/launch_admin_console.png)

1. En Admin Console, realice una de las siguientes acciones para crear un nuevo usuario:

   * En la barra de herramientas de la parte superior, haga clic en **[!UICONTROL información general]** . En la [!UICONTROL  información general ] página, haga clic en **[!UICONTROL asignar usuarios]** desde el tarjeta de productos de Brand portal.

   ![Información general de Admin Console](assets/admin_console_overviewadduser.png)

   * En la barra de herramientas de la parte superior, haga clic en **[!UICONTROL Usuarios]**. En el [!UICONTROL Usuarios] página, [!UICONTROL Usuarios] en el carril izquierdo está seleccionado de forma predeterminada. Clic **[!UICONTROL Añadir usuario]**.

   ![Admin Console Agregar usuarios](assets/admin_console_adduseruserpage.png)

1. En el cuadro de diálogo Agregar usuario, escriba el ID de correo electrónico del usuario que desea agregar o seleccione el usuario en la lista de sugerencias que aparecen mientras escribe.

   ![Añadir usuario a Brand Portal](assets/add_user_to_aem_bp.png)

1. Asigne el usuario al menos a un producto perfil (antes denominado configuración del producto) para que el usuario pueda acceder a Brand portal. Seleccione la perfil del producto correspondiente en la **[!UICONTROL Seleccione una perfil para este campo del producto]** .
1. Haga clic en **[!UICONTROL Guardar]**. Se envía una correo electrónico de bienvenida a la usuario recientemente agregada. La usuario invitada puede hacer clic en el vincular en la correo electrónico de bienvenida para acceder a Brand portal. El usuario puede inicio de sesión con el ID de correo electrónico ( [!UICONTROL  Adobe ID ] , [!UICONTROL  Enterprise ID ] o [!UICONTROL  Fedrated ID ] ) configurado en admin Console. Para obtener más información, consulte [Experiencia del primer inicio de sesión](../using/brand-portal-onboarding.md).

   >[!NOTE]
   >
   >Si un usuario no puede iniciar sesión en Brand Portal, el administrador de la organización debe visitar el Adobe [!UICONTROL Admin Console] y compruebe si el usuario está presente y si se ha añadido al menos a un perfil de producto.

   Para obtener información sobre la concesión de privilegios administrativos al usuario, consulte [Proporcionar privilegios de administrador a los usuarios](../using/brand-portal-adding-users.md#provideadministratorprivilegestousers).

## Añadir un perfil de producto {#add-a-product-profile}

Perfiles de producto (anteriormente conocidos como configuraciones de producto) en [!UICONTROL Admin Console] se utilizan para crear grupos en Brand Portal, de modo que pueda realizar operaciones masivas como la administración de funciones y el uso compartido de recursos en Brand Portal. **Brand Portal** es el perfil de producto predeterminado disponible; puede crear más perfiles de producto y agregar usuarios a los nuevos perfiles de producto.

>[!NOTE]
>
>Puede iniciar sesión en [[!UICONTROL Admin Console]](https://adminconsole.adobe.com/enterprise/overview) directamente o desde Brand Portal. Si inicio de sesión [!UICONTROL  admin Console ] directamente, seguir pasos 4-7 en el siguiente procedimiento para añadir un perfil de producto.

1. En la barra de herramientas de AEM de la parte superior, haga clic en el logotipo de Adobe Systems para acceder a las herramientas administrativas.

   ![Logotipo de AEM](assets/aemlogo.png)

1. En el panel Herramientas administrativas, haga clic en **[!UICONTROL usuarios]** .

   ![Panel de herramientas de administración](assets/admin-tools-panel-6.png)

1. En el [!UICONTROL Funciones del usuario] , haga clic en **[!UICONTROL Administración]** y haga clic en **[!UICONTROL Admin Console de Launch]**.

   ![Admin Console de Launch](assets/launch_admin_console.png)

1. En la barra de herramientas de la parte superior, haga clic en **[!UICONTROL productos]** .
1. En el [!UICONTROL  Página de productos ] , [!UICONTROL  perfiles ] de producto se selecciona de forma predeterminada. Haga clic en **[!UICONTROL nuevo perfil]** .

   ![añadir nuevo perfil de producto](assets/admin_console_addproductprofile.png)

1. En el [!UICONTROL Crear un nuevo perfil] , proporcione el nombre para mostrar y la descripción del perfil y elija si quiere notificar a los usuarios por correo electrónico cuando se les añada o elimine del perfil.

   ![Crear perfil de producto](assets/admin_console_addaproductprofilecreatenewprofile.png)

1. Haga clic en **[!UICONTROL Listo]**. El grupo de configuración del producto, por ejemplo **[!UICONTROL Grupo de ventas]**, se añade a Brand Portal.

   ![Perfiles de producto](assets/admin_console_productprofileadded.png)

## Adición de usuarios a un perfil de producto {#add-users-to-a-product-profile}

Para agregar usuarios a un grupo de Brand Portal, agréguelos al perfil de producto correspondiente (anteriormente conocido como configuraciones de producto) en [!UICONTROL Admin Console]. Puede agregar usuarios de forma individual o en lote.

>[!NOTE]
>
>Puede iniciar sesión en [[!UICONTROL Admin Console]](https://adminconsole.adobe.com/enterprise/overview) directamente o desde Brand Portal. Si inicia sesión en Admin Console directamente, siga los pasos 4-7 del procedimiento siguiente para añadir usuarios a un perfil de producto.

1. En la barra de herramientas de la parte superior, haga clic en el logotipo del Experience Manager para acceder a las herramientas administrativas.

   ![AEM Logotipo de](assets/aemlogo.png)

1. En el panel de herramientas administrativas, haga clic en **[!UICONTROL Usuarios]**.

   ![Panel herramientas de administración](assets/admin-tools-panel-7.png)

1. En la [!UICONTROL  Página funciones ] de usuario, haga clic en el pestaña de **[!UICONTROL Administración]** y, a continuación, en **[!UICONTROL Launch admin Console]** .

   ![Iniciar [!DNL Admin Console]](assets/launch_admin_console.png)

1. En la barra de herramientas de la parte superior, haga clic en **[!UICONTROL Productos]**.
1. En el [!UICONTROL Productos] página, [!UICONTROL Perfiles de producto] está seleccionado de forma predeterminada. Abra el perfil de producto al que desee agregar un usuario, por ejemplo, [!UICONTROL Grupo de ventas].

   ![Perfiles de producto](assets/admin_console_productprofileadded.png)

1. Para agregar usuarios individuales al perfil de producto, haga lo siguiente:

   * Haga clic en **[!UICONTROL añadir usuario]** .

   ![Agrupar para asignar un perfil de producto en Brand portal](assets/admin_console_productprofilesalesgroup.png)

   * En el [!UICONTROL  añadir usuario a Sales grupo ] página, escriba el ID correo electrónico del usuario que desea agregar o seleccione el usuario de las sugerencias que aparecen al escribir.

   ![Agregar un usuario a un grupo](assets/admin_console_addusertosalesgroup.png)

   * Haga clic en **[!UICONTROL Guardar]**.



1. Para añadir usuarios en bloque al perfil de producto, haga lo siguiente:

   * Elegir **[!UICONTROL puntos suspensivos (...) > Agregar usuarios mediante CSV]**.

   ![Adición de usuarios por lotes](assets/admin_console_addbulkusers.png)

   * En el **[!UICONTROL Agregar usuarios mediante CSV]** , descargue una plantilla CSV o arrastre y suelte un archivo CSV.

   ![Adición de usuarios por csv](assets/admin_console_addbulkuserscsv.png)

   * Haga clic en **[!UICONTROL Cargar]**.
   Si agregó usuarios al perfil de producto predeterminado, es decir, a Brand Portal, se enviará un correo electrónico de bienvenida al ID de correo electrónico de los usuarios que agregó. Los usuarios invitados pueden acceder a Brand Portal haciendo clic en el vínculo del correo electrónico de bienvenida e iniciando sesión con un [!UICONTROL Adobe ID]. Para obtener más información, consulte [Experiencia del primer inicio de sesión](../using/brand-portal-onboarding.md).

   Los usuarios añadidos a un perfil de producto personalizado o nuevo no reciben notificaciones por correo electrónico.

## Proporcionar privilegios de administrador a usuarios {#provide-administrator-privileges-to-users}

Puede proporcionar al administrador del sistema o el privilegio administrador del producto a un usuario de Brand portal. No proporcione otros derechos administrativos disponibles en [!UICONTROL Admin Console], como administrador de perfiles de producto, administrador de grupos de usuarios y administrador de asistencia. Para obtener más información sobre estas funciones, consulte [Funciones administrativas](https://helpx.adobe.com/enterprise/using/admin-roles.html).

>[!NOTE]
>
>Puede iniciar sesión en [[!UICONTROL Admin Console]](https://adminconsole.adobe.com/enterprise/overview) directamente o desde Brand Portal. Si inicia sesión en [!UICONTROL Admin Console] Siga directamente los pasos 4-8 del siguiente procedimiento para añadir un usuario a un perfil de producto.

1. AEM En la barra de herramientas de la parte superior, haga clic en el logotipo del Adobe para acceder a las herramientas administrativas.

   ![Logotipo de AEM](assets/aemlogo.png)

1. En el panel de herramientas administrativas, haga clic en **[!UICONTROL Usuarios]**.

   ![Panel de herramientas de administración](assets/admin-tools-panel-8.png)

1. En el [!UICONTROL Funciones del usuario] , haga clic en **[!UICONTROL Administración]** y haga clic en **[!UICONTROL Admin Console de Launch]**.

   ![Admin Console de Launch](assets/launch_admin_console.png)

1. En la barra de herramientas de la parte superior, haga clic en **[!UICONTROL Usuarios]**.
1. En el [!UICONTROL Usuarios] página, [!UICONTROL Usuarios] en el carril izquierdo está seleccionado de forma predeterminada. Haga clic en el nombre de usuario del usuario al que desea otorgar privilegios de administrador.

   ![Agregar usuarios al Admin Console](assets/admin_console_adduseruserpage.png)

1. En la página de perfil de usuario, busque **[!UICONTROL Derechos administrativos]** en la parte inferior y elija **[!UICONTROL puntos suspensivos (...) > Editar derechos de administrador]**.
   ![Derechos de administrador en Admin Console](assets/admin_console_editadminrights.png)

1. En el [!UICONTROL Editar administrador] , seleccione Administrador del sistema o Administrador de productos.

   ![Editar los derechos de administración en Admin Console](assets/admin_console_editadminrightsselection.png)

   >[!NOTE]
   >
   >Brand portal solo admite funciones de administrador del sistema y administrador del producto.
   >
   >Adobe Systems recomienda evitar el uso del administrador del sistema función porque otorga privilegios de administrador en toda la organización para todos los productos de una organización. Por ejemplo, un administrador del sistema de una organización que incluye tres marketing nube productos tiene el conjunto completo de privilegios para los tres productos. Solo el administrador del sistema puede configurar Experience Manager Assets para que activos pueda publicarse de Experience Manager Assets en Brand portal. Para obtener más información, consulte [Configuración de Experience Manager Assets con Brand Portal](../using/configure-aem-assets-with-brand-portal.md).
   >
   >Por el contrario, la función Administrador de productos concede privilegios de administrador solo para un producto específico. Si desea aplicar un control de acceso más granular dentro de Brand Portal, utilice la función Administrador de productos y seleccione el producto como Brand Portal.

   >[!NOTE]
   >
   >Brand Portal no admite privilegios de administrador de perfiles de producto (anteriormente conocido como administrador de configuración). Evite asignar derechos de administrador de perfil de producto a un usuario.

1. Revise la selección de tipo admin y haga clic en **[!UICONTROL Guardar]**.

   >[!NOTE]
   >
   >Para revocar privilegios de administrador para una usuario, realice los cambios correspondientes en la **[!UICONTROL página Administración]** de editar y, a continuación, haga clic en **[!UICONTROL Guardar]** .


## Administrar funciones de usuario {#manage-user-roles}

Un administrador puede modificar las funciones de los usuarios en Brand Portal.

Además de la función Administrador, Brand Portal admite las siguientes funciones:

* [!UICONTROL Visor]: los usuarios con esta función pueden ver los archivos y carpetas que un administrador comparte con ellos. Los visualizadores también pueden buscar y descargar recursos. Sin embargo, los visualizadores no pueden compartir contenido (archivos, carpetas, [!UICONTROL colecciones]) con otros usuarios.
* [!UICONTROL Editor]: los usuarios con esta función tienen todos los privilegios de un visualizador. Además, los editores pueden compartir contenido (carpetas, [!UICONTROL colecciones], vínculos) con otros usuarios.

1. AEM En la barra de herramientas de la parte superior, haga clic en el logotipo del Adobe para acceder a las herramientas administrativas.

   ![Logotipo de AEM](assets/aemlogo.png)

1. En el panel de herramientas administrativas, haga clic en **[!UICONTROL Usuarios]**.

   ![Panel de herramientas de administración](assets/admin-tools-panel-9.png)

1. En el [!UICONTROL Funciones del usuario] página, la [!UICONTROL Usuarios] está seleccionada de forma predeterminada. Para el usuario cuya función desee cambiar, seleccione **[!UICONTROL Editor]** o **[!UICONTROL Visor]** desde el **[!UICONTROL Rol]** menú desplegable.

   ![Modificar las funciones de los usuarios](assets/modify_user_role.png)

   Para modificar la función de varios usuarios simultáneamente, seleccione los usuarios y elija el función correspondiente en la **[!UICONTROL lista desplegable función]** .

   >[!NOTE]
   >
   >El [!UICONTROL Rol] La lista de usuarios administradores está desactivada. No puede seleccionar estos usuarios para modificar sus funciones.


   >[!NOTE]
   >
   >La función de usuario también se deshabilita si el usuario es miembro del grupo Editor. Para revocar los privilegios de edición al usuario, elimínelo del grupo Editor o cambie la función de todo el grupo a Visor.


1. Haga clic en **[!UICONTROL Guardar]**. La función se modifica para el usuario correspondiente. Si ha seleccionado varios usuarios, los roles de todos los usuarios se modifican simultáneamente.

   >[!NOTE]
   >
   >Los cambios en usuario permisos solo se reflejan en las **[!UICONTROL funciones]** de usuario página después de que los usuarios vuelvan a Inicio de sesión en Brand portal.

## Administración de funciones y privilegios de grupo {#manage-group-roles-and-privileges}

Un administrador puede asociar privilegios específicos con una [ grupo ](../using/brand-portal-adding-users.md#main-pars-title-278567577) de usuarios en Brand portal. Los **[!UICONTROL grupos]** pestaña de las **[!UICONTROL funciones]** de usuario página permiten a los administradores:

* Asignar funciones a grupos de usuario
* Restrinja a los grupos de usuarios a descargar representaciones originales de archivos de imagen (.jpeg, .tiff, .png, .bmp, .gif, .pjpeg, x-portable-anymap, x-portable-bitmap, x-portable-graymap, x-portable-pixmap, x-rgb, x-xbitmap, x-xpixmap, x-icon, image/photoshop, image/x-photoshop, .psd, image/vnd.adobe.photoshop) desde Brand Portal.

>[!NOTE]
>
>En el caso de los recursos compartidos como vínculo, el permiso para acceder a las representaciones originales de los archivos de imagen se aplicará en función de los permisos del usuario que comparta los recursos.

Para modificar la función y el derecho de acceso a las representaciones originales para miembros de grupo específicos, siga estos pasos:

1. En el **[!UICONTROL Funciones del usuario]** , vaya a la página **[!UICONTROL Grupos]** pestaña.
1. Seleccione los grupos cuyos roles desea cambiar.
1. Seleccione la función adecuada en el **[!UICONTROL Rol]** lista desplegable.

   Para permitir que los miembros de un grupo tengan acceso a las representaciones originales de archivos de imagen (.jpeg, .tiff, .png, .bmp, .gif, .pjpeg, x-portable-anymap, x-portable-bitmap, x-portable-graymap, x-portable-pixmap, x-rgb, x-xbitmap, x-xpixmap, x-icon, image/photoshop, image/x-photoshop, .psd, image/vnd.adobe.photoshop) que descarguen del portal o del vínculo compartido, mantenga **[!UICONTROL Acceso al original]** opción seleccionada para ese grupo. De forma predeterminada, **[!UICONTROL se selecciona acceso a la opción original]** para todos los usuarios. Para evitar que un grupo de usuarios acceda a las representaciones originales, anule la selección de la opción correspondiente a ese grupo.

   ![Funciones del grupo de usuarios](assets/access-original-rend.png)

   >[!NOTE]
   >
   >Si se agrega un usuario a varios grupos y uno de estos grupos tiene restricciones, estas se aplicarán a ese usuario.
   >
   >Además, las restricciones para acceder a las representaciones originales de archivos de imagen no se aplican a los administradores aunque sean miembros de grupos restringidos.


1. Haga clic en **[!UICONTROL Guardar]**. La función se ha modificado para los grupos correspondientes.

   >[!NOTE]
   >
   >La Asociación usuario a grupo, o la miembros del grupo de un usuario, se sincroniza con Brand portal cada 8 horas. Los cambios en las funciones de usuario o grupo son efectivos después de que se ejecute el siguiente trabajo de sincronizar.
