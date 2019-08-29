---
title: Administrar usuarios, grupos y funciones de usuario
seo-title: Administrar usuarios, grupos y funciones de usuario
description: Los administradores pueden utilizar Adobe Admin Console para crear usuarios y perfiles de producto de AEM Assets Brand Portal y administrar sus funciones mediante la interfaz de usuario de Brand Portal. Este privilegio no está disponible para los editores y editores.
seo-description: Los administradores pueden utilizar Adobe Admin Console para crear usuarios y perfiles de producto de AEM Assets Brand Portal y administrar sus funciones mediante la interfaz de usuario de Brand Portal. Este privilegio no está disponible para los editores y editores.
uuid: 0 dc 1867 c -6 d 1 b -4 d 0 d-a 25 e -0 df 207 c 269 b 8
content-type: referencia
topic-tags: administración
products: SG_ EXPERIENCEMANAGER/Brand_ Portal
discoiquuid: ba 468 e 80-d 077-4 af 6-b 782-238 fc 557 e 22 b
translation-type: tm+mt
source-git-commit: 32c3cdb8e3fafd74cfb36e6bcfe0811e7152b2d0

---


# Administrar usuarios, grupos y funciones de usuario {#manage-users-groups-and-user-roles}

Los administradores pueden utilizar [!DNL Adobe Admin Console] para crear [!DNL AEM Assets Brand Portal] usuarios y perfiles de producto, y administrar sus funciones mediante la interfaz de usuario de Brand Portal. Este privilegio no está disponible para los editores y editores.

En [Admin Console](http://adminconsole.adobe.com/enterprise/overview), puede ver todos los productos asociados con su organización. Un producto podría ser cualquier [!DNL Experience Cloud] solución, [!DNL Adobe Analytics][!DNL Adobe Target]como, o [!DNL AEM Brand Portal]. Debe elegir el producto AEM Brand Portal y crear perfiles de producto.

<!--
Comment Type: draft

<note type="note">
<p>Product Profiles (formerly known as product configurations*). </p>
<p>* The nomenclature has changed from product configurations to product profiles in the new Adobe Admin Console.</p>
</note>
-->
![](assets/create-user-group.png)

Estos perfiles de producto se sincronizan con la interfaz [!DNL Brand Portal] de usuario cada 8 horas y son visibles como grupos en [!DNL Brand Portal]. Una vez que agregue usuarios y cree perfiles de producto, y agregue usuarios a esos perfiles de producto, puede asignar funciones a usuarios y grupos en [!DNL Brand Portal].

>[!NOTE]
>
>Para crear grupos en [!DNL Brand Portal], utilice [!DNL Adobe Admin Console]la página **Productos** &gt; Perfiles **de producto**, en lugar de la página **Usuario** &gt; Grupos **de usuarios**. Los perfiles de producto en [!DNL Adobe Admin Console] se utilizan para crear grupos en [!DNL Brand Portal].

## Agregar un usuario {#add-a-user}

Si es administrador de productos, utilice [[! DNL Adobe Admin Console]](http://adminconsole.adobe.com/enterprise/overview) para crear usuarios y asignarlos a perfiles de producto (*anteriormente conocidos como configuraciones de producto*), que se muestran como grupos en [!DNL Brand Portal]. Puede utilizar grupos para realizar operaciones masivas como administración de funciones y uso compartido de recursos.

>[!NOTE]
Usuarios nuevos que no tienen acceso para [!DNL Brand Portal] solicitar acceso desde la pantalla de inicio de sesión. [!DNL Brand Portal] Para obtener más información, consulte [Solicitar acceso a [! DNL Brand Portal]](../using/brand-portal.md#request-access-to-brand-portal). Después de recibir las notificaciones de solicitud de acceso en su área de notificación, haga clic en la notificación pertinente y, a continuación, haga clic **en Conceder acceso**. También puede seguir el vínculo del correo electrónico de solicitud de acceso recibido. A continuación, para agregar un usuario a través [de [! DNL Adobe Admin Console]](http://adminconsole.adobe.com/enterprise/overview), siga los pasos 4-7 en el procedimiento siguiente.

>[!NOTE]
Puede iniciar sesión en [[! DNL Adobe Admin Console]](http://adminconsole.adobe.com/enterprise/overview) directamente o desde [!DNL Brand Portal]. Si inicia sesión directamente, siga los pasos 4-7 en el procedimiento siguiente para agregar un usuario.

1. En la [!DNL AEM] barra de herramientas de la parte superior, haga clic en el logotipo de Adobe para acceder a las herramientas administrativas.

   ![Logotipo de AEM](assets/aemlogo.png)

2. En el panel de herramientas administrativas, haga clic **en Usuarios**.

   ![Panel de herramientas de administración](assets/admin-tools-panel-5.png)

3. En la página **Funciones** de usuario, haga clic en la ficha **Administración** y, a continuación, en **Iniciar Admin Console**.

   ![Funciones de usuario para iniciar Admin Console](assets/launch_admin_console.png)

4. En Admin Console, realice una de las siguientes acciones para crear un nuevo usuario:

   * En la barra de herramientas de la parte superior, haga clic **en Información general**. En la página **Información general** , haga clic **en Asignar usuarios** de la tarjeta **[!DNL AEM Brand Portal]** de producto.
   ![Información general de la Consola de administración](assets/admin_console_overviewadduser.png)

   * En la barra de herramientas de la parte superior, haga clic **en Usuarios**. En la página **Usuarios** , **los usuarios** del carril izquierdo se seleccionan de forma predeterminada. Haga clic **en Agregar usuario**.
   ![Admin Console Add Users](assets/admin_console_adduseruserpage.png)

5. En el cuadro de diálogo Agregar usuario, escriba el ID de correo electrónico del usuario que desee agregar o seleccione el usuario de la lista de sugerencias que aparecen mientras escribe.

   ![Agregar usuario a Brand Portal](assets/add_user_to_aem_bp.png)

6. Asigne al usuario a un perfil de producto como mínimo (anteriormente conocido como configuraciones de producto) para que el usuario pueda acceder a Brand Portal. Seleccione el perfil de producto adecuado en el **campo Seleccione un perfil para este** campo de producto.
7. Haga clic en **Guardar.** Se envía un correo electrónico de bienvenida al usuario que ha agregado. Para acceder [!DNL Brand Portal] al usuario invitado, haga clic en el vínculo del correo electrónico de bienvenida e inicie sesión con [!UICONTROL un Adobe ID]. Para obtener más información, consulte [Primera experiencia de inicio de sesión](../using/brand-portal-onboarding.md).

   >[!NOTE]
   Si un usuario no puede iniciar sesión, [!DNL Brand Portal]el administrador de la organización debe visitar Adobe [!UICONTROL Admin Console] y comprobar si el usuario está presente y se ha agregado al menos un perfil de producto.

   Para obtener información sobre la concesión de privilegios administrativos al usuario, consulte [Proporcionar privilegios de administrador a los usuarios](../using/brand-portal-adding-users.md#provideadministratorprivilegestousers).

## Agregar un perfil de producto {#add-a-product-profile}

Los perfiles de producto (anteriormente conocidos como configuraciones de producto) en [!UICONTROL la Consola] de administración se utilizan para crear grupos en [!DNL Brand Portal] los que se pueden realizar operaciones masivas como administración de roles y uso compartido de recursos en [!DNL Brand Portal]. **[!DNL Brand Portal]** es el perfil de producto predeterminado disponible; Puede crear más perfiles de producto y agregar usuarios a los nuevos perfiles de producto.

>[!NOTE]
Puede iniciar sesión en [[! UICONTROL Admin Console]](http://adminconsole.adobe.com/enterprise/overview) directamente o desde [!DNL Brand Portal]. Si inicia sesión en [!UICONTROL Admin Console] directamente, siga los pasos 4-7 en el procedimiento siguiente para agregar un perfil de producto.

1. En la [!DNL AEM] barra de herramientas de la parte superior, haga clic en el logotipo de Adobe para acceder a las herramientas administrativas.

   ![[!DNL AEM] Logotipo](assets/aemlogo.png)

2. En el panel de herramientas administrativas, haga clic **en Usuarios**.

   ![Panel de herramientas de administración](assets/admin-tools-panel-6.png)

3. En la página **Funciones** de usuario, haga clic en la ficha **Administración** y, a continuación, en **Iniciar Admin Console**.

   ![Iniciar Admin Console](assets/launch_admin_console.png)

4. En la barra de herramientas de la parte superior, haga clic **en Productos**.
5. En la página **Productos** , los perfiles **de producto** se seleccionan de forma predeterminada. Haga clic **en Nuevo perfil**.

   ![Agregar nuevo perfil de producto](assets/admin_console_addproductprofile.png)

6. En **la** página Crear un nuevo perfil, proporcione el nombre del perfil, el nombre para mostrar, la descripción del perfil y elija si desea notificar a los usuarios por correo electrónico cuando se añadan o eliminen del perfil.

   ![Crear perfil de producto](assets/admin_console_addaproductprofilecreatenewprofile.png)

7. Haga clic en **Finalizado**. El grupo de configuración de productos, por ejemplo, el grupo **Ventas**, se agrega a Brand Portal.

   ![Perfiles de producto](assets/admin_console_productprofileadded.png)

## Agregar usuarios a un perfil de producto {#add-users-to-a-product-profile}

Para agregar usuarios a [!DNL Brand Portal] un grupo, agréguelos al perfil de producto correspondiente (anteriormente conocido como configuraciones de producto) en la Consola [!UICONTROL de administración]. Puede agregar usuarios de forma individual o de forma masiva.

>[!NOTE]
Puede iniciar sesión en [[! DNL Admin Console]](http://adminconsole.adobe.com/enterprise/overview) directamente o desde [!DNL Brand Portal]. Si inicia sesión en Admin Console directamente, siga los pasos 4-7 en el procedimiento siguiente para agregar usuarios a un perfil de producto.

1. En la [!DNL AEM] barra de herramientas de la parte superior, haga clic en el logotipo de Adobe para acceder a las herramientas administrativas.

   ![[!DNL AEM] Logotipo](assets/aemlogo.png)

2. En el panel de herramientas administrativas, haga clic **en Usuarios**.

   ![Panel de herramientas de administración](assets/admin-tools-panel-7.png)

3. En la página **Funciones** de usuario, haga clic en la ficha **Administración** y, a continuación, en **Iniciar Admin Console**.

   ![Iniciar [!DNL Admin Console]](assets/launch_admin_console.png)

4. En la barra de herramientas de la parte superior, haga clic **en Productos**.
5. En la página **Productos** , los perfiles **de producto** se seleccionan de forma predeterminada. Abra el perfil de producto al que desee agregar un usuario, por ejemplo, el grupo **Ventas**.

   ![Perfiles de producto](assets/admin_console_productprofileadded.png)

6. Para agregar usuarios individuales al perfil de producto, haga lo siguiente:

   * Haga clic **en Agregar usuario**.
   ![Agrupar el perfil de producto en [!DNL Brand Portal]](assets/admin_console_productprofilesalesgroup.png)

   * En la página de grupo **Agregar usuario** a ventas, escriba el ID de correo electrónico del usuario que desee agregar o seleccione el usuario de la lista de sugerencias que aparecen mientras escribe.
   ![Agregar usuario a un grupo](assets/admin_console_addusertosalesgroup.png)

   * Haga clic en **Guardar**.



7. Para agregar usuarios masivos al perfil de producto, haga lo siguiente:

   * Elija elipsis(...)****&gt; **Agregar usuarios por CSV**.
   ![Agregar usuarios de forma masiva](assets/admin_console_addbulkusers.png)

   * En **la** página Agregar usuarios por CSV, descargue una plantilla CSV o arrastre y suelte un archivo CSV.
   ![Agregar usuarios por csv](assets/admin_console_addbulkuserscsv.png)

   * Click **Upload**.
   Si ha agregado usuarios al perfil de producto predeterminado, es decir [!DNL Brand Portal], se envía un correo electrónico de bienvenida al ID de correo electrónico de los usuarios que ha agregado. Los usuarios invitados pueden acceder [!DNL Brand Portal] al vínculo haciendo clic en el vínculo del correo electrónico de bienvenida e iniciando sesión con [!UICONTROL un Adobe ID]. Para obtener más información, consulte [Primera experiencia de inicio de sesión](../using/brand-portal-onboarding.md).

   Los usuarios agregados a un perfil de producto personalizado o nuevo no reciben notificaciones por correo electrónico.

## Proporcionar privilegios de administrador a los usuarios {#provide-administrator-privileges-to-users}

Puede proporcionar al administrador del sistema o al administrador del producto privilegios de administrador de [!DNL Brand Portal] producto. No proporcione otros derechos administrativos disponibles en la Consola [!UICONTROL de administración], como administrador de perfiles de producto, administrador de grupos de usuarios y administrador de asistencia. Para obtener más información sobre estas funciones, consulte [Funciones administrativas](https://helpx.adobe.com/enterprise/using/admin-roles.html).

>[!NOTE]
Puede iniciar sesión en [[! UICONTROL Admin Console]](https://adminconsole.adobe.com/enterprise/overview) directamente o desde [!DNL Brand Portal]. Si inicia sesión en [!UICONTROL Admin Console] directamente, siga los pasos 4-8 en el procedimiento siguiente para agregar un usuario a un perfil de producto.

1. En la [!DNL AEM] barra de herramientas de la parte superior, haga clic en el logotipo de Adobe para acceder a las herramientas administrativas.

   ![Aemlogo](assets/aemlogo.png)

2. En el panel de herramientas administrativas, haga clic **en Usuarios**.

   ![Panel de herramientas de administración](assets/admin-tools-panel-8.png)

3. En la página **Funciones** de usuario, haga clic en la ficha **Administración** y, a continuación, en **Iniciar Admin Console**.

   ![Iniciar Admin Console](assets/launch_admin_console.png)

4. En la barra de herramientas de la parte superior, haga clic **en Usuarios**.
5. En la página **Usuarios** , **los usuarios** del carril izquierdo se seleccionan de forma predeterminada. Haga clic en el nombre de usuario del usuario al que desee otorgar privilegios de administrador.

   ![Agregar usuarios en Admin Console](assets/admin_console_adduseruserpage.png)

6. En la página de perfil de usuario, busque **la sección Derechos** administrativos en la parte inferior y seleccione elipsis(...)****&gt; **Editar derechos de administrador**.
   ![Derechos de administrador en Admin Console](assets/admin_console_editadminrights.png)

7. En **la** página Editar administrador, seleccione Administrador del sistema o Administrador de productos.

   ![Editar derechos de administrador en Admin Console](assets/admin_console_editadminrightsselection.png)

   >[!NOTE]
   [!DNL Brand Portal] solo admite funciones de administrador del sistema y administrador de productos.
   [!DNL Adobe] recomienda evitar el uso de la función Administrador de sistemas, ya que concede privilegios de administrador en toda la organización para todos los productos de una organización. Por ejemplo, un administrador de sistemas de una organización que incluye tres productos de Marketing Cloud tiene el conjunto completo de privilegios para los tres productos. Solo un administrador de sistemas puede configurar [!DNL AEM] Recursos para que los recursos se puedan publicar desde [!DNL AEM] Recursos. [!DNL Brand Portal] Para obtener más información, consulte [Configuración de la integración de AEM Assets con [! DNL Brand Portal]](https://helpx.adobe.com/experience-manager/6-5/assets/using/brand-portal-configuring-integration.html).
   Por el contrario, la función Administrador de productos concede privilegios de administrador solamente para un producto específico. Si desea exigir un control de acceso más granular, [!DNL Brand Portal]utilice la función Administrador de productos y seleccione el producto como **[!DNL AEM Brand Portal]**.

   >[!NOTE]
   [!DNL Brand Portal] no admite privilegios de administrador de perfil de producto (anteriormente conocido como administrador de configuración). Evite asignar derechos de administrador de perfil de producto a un usuario.

8. Revise la selección de tipo de administrador y haga clic **en Guardar**.

   >[!NOTE]
   Para revocar privilegios de administrador para un usuario, realice los cambios correspondientes en la página **Editar administrador** y, a continuación, haga clic **en Guardar**.

## Administrar funciones de usuario {#manage-user-roles}

Un administrador puede modificar las funciones de los usuarios en [!DNL Brand Portal].

Además de la función de administrador [!DNL Brand Portal] , admite las siguientes funciones:

* **Visor**: Los usuarios con esta función pueden ver los archivos y las carpetas que un administrador comparte con ellos. Los visores también pueden buscar y descargar recursos. Sin embargo, los visores no pueden compartir contenido (archivos, carpetas, [!UICONTROL colecciones]) con otros usuarios.
* **Editor**: Los usuarios con esta función tienen todos los privilegios de un visor. Además, Editores puede compartir contenido (carpetas, [!UICONTROL colecciones], vínculos) con otros usuarios.

1. En la [!DNL AEM] barra de herramientas de la parte superior, haga clic en el logotipo de Adobe para acceder a las herramientas administrativas.

   ![Aemlogo](assets/aemlogo.png)

2. En el panel de herramientas administrativas, haga clic **en Usuarios**.

   ![Panel de herramientas de administración](assets/admin-tools-panel-9.png)

3. En la página **Funciones** de usuario, la ficha **Usuarios** está seleccionada de forma predeterminada. Para el usuario cuya función desea modificar, seleccione **Editor** o **Visor** en la lista desplegable **Función** .

   ![Modificación de funciones de usuarios](assets/modify_user_role.png)

   Para modificar la función de varios usuarios simultáneamente, seleccione los usuarios y elija la función adecuada en la lista desplegable **Función** .

   >[!NOTE]
   La lista **Función** para usuarios de Administrador está deshabilitada. No puede seleccionar a estos usuarios para modificar sus funciones.

   >[!NOTE]
   La función de usuario también está deshabilitada si el usuario es miembro del grupo Editor. Para anular los privilegios de edición del usuario, elimine el usuario del grupo Editor o cambie la función de todo el grupo a Visor.

4. Haga clic en **Guardar.** La función se modifica para el usuario correspondiente. Si seleccionó varios usuarios, las funciones para todos los usuarios se modifican simultáneamente.

   >[!NOTE]
   Los cambios en los permisos de usuario se reflejan en la página Funciones **de usuario** solo después de que los usuarios vuelvan a iniciar sesión en Brand Portal.

## Administrar funciones y privilegios de grupo {#manage-group-roles-and-privileges}

Un administrador puede asociar privilegios específicos con un [grupo](../using/brand-portal-adding-users.md#main-pars-title-278567577) de usuarios en Brand Portal. La ficha **Grupos** de la página **Funciones** de usuario permite a los administradores:

* Asignación de funciones a grupos de usuarios
* Restringir los grupos de usuarios para descargar representaciones originales de archivos de imagen (.jpeg. tiff. png. bmp. gif. pjpeg, x-portable-anymap, x-portable-anymap, x-portable-graymap, x-portable-pixmap, x-rgb, x-xbitmap, x-xpixmap, x-xpixmap xpixmap, x-icon, image/photoshop, image/x-photoshop. psd, image/vnd. adobe. photoshop) desde Brand Portal.

>[!NOTE]
Para los recursos compartidos como vínculo, el permiso para acceder a representaciones originales de archivos de imagen se aplicará según los permisos del usuario que comparte los recursos.

Para modificar la función y el derecho a acceder a las representaciones originales para miembros específicos del grupo, siga estos pasos:

1. En **la página Funciones** de usuario, vaya a **la** ficha Grupos.
2. Seleccione los grupos para los cuales desee cambiar las funciones.
3. Seleccione la función adecuada en la lista desplegable **Función** .

   Para permitir que los miembros de un grupo tengan acceso a representaciones originales de archivos de imagen (.jpeg. tiff. png. bmp. gif. pjpeg, x-portable-anymap, x-portable-anymap, x-portable-de-mapmap, x-portable-pixmap, x-rgb, x-xbitxde x-xbitmap x-xbitmap x-xbitmap x-xbitmap x-xbitmap x-xbitmap x-xbitmap x-xbitxbitmap x-xbitxx x-xbitxx x-xbitxbitmap x-xbitxbitx-xbitxbitmap x-xbitxx x-xbitxbitmap x-xbitxbitx-xbitxbitmap x-xbitxx x-xbitxbitmap x-xbitxbitx x mapa, x-xpixmap, x-icon, image/photoshop, image/x-photoshop. psd, image/vnd. adobe. photoshop) que descargan del portal o del vínculo compartido, mantenga seleccionada la **opción Acceso a original** para ese grupo. De forma predeterminada, **se selecciona la** opción Acceso a original para todos los usuarios. Para evitar que un grupo de usuarios acceda a representaciones originales, anule la selección de la opción correspondiente a dicho grupo.

   ![Funciones de grupos de usuarios](assets/access-original-rend.png)

   >[!NOTE]
   Si un usuario se agrega a varios grupos y alguno de estos grupos tiene restricciones, las restricciones se aplicarán a ese usuario.
   Además, las restricciones para acceder a las representaciones originales de los archivos de imagen no se aplican a los administradores aunque sean miembros de grupos restringidos.

4. Haga clic en **Guardar.** La función se modifica para los grupos correspondientes.

   >[!NOTE]
   La asociación de usuario a grupo, o la pertenencia a grupos de un usuario, se sincronizan con [!DNL Brand Portal] cada 8 horas. Los cambios en las funciones de usuario o grupo son efectivos después de ejecutar el siguiente trabajo de sincronización.
