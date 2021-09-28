---
title: Acceso de invitado a Brand Portal
seo-title: Guest Access to Brand Portal
description: Permita el acceso de invitado y ahorre el esfuerzo de incorporar numerosos usuarios sin autenticación.
seo-description: Allow guest access and save the effort to onboard numerous users without authentication.
uuid: edb4378d-1710-44a2-97a6-594d99f62fff
contentOwner: VG
topic-tags: introduction
content-type: reference
products: SG_EXPERIENCEMANAGER/Brand_Portal
discoiquuid: b9e9fe7b-0373-42d1-851b-7c76b47657c2
exl-id: ecce0a45-abae-41c4-9ea7-5dfdcf19e5ea
source-git-commit: 51dc6f9c3b3a59751d7910513279e52906d97b88
workflow-type: tm+mt
source-wordcount: '1026'
ht-degree: 0%

---

# Acceso de invitado a Brand Portal {#guest-access-to-brand-portal}

Experience Manager Assets Brand Portal permite que los invitados accedan al portal. Un usuario invitado no necesita credenciales para entrar al portal y tiene acceso a los recursos públicos (y colecciones) del portal. Los usuarios de la sesión de invitados pueden agregar recursos a lightbox (colección privada) y descargarlos hasta que dure la sesión, que es de 2 horas desde el comienzo de la sesión, a menos que el usuario invitado elija [[!UICONTROL Finalizar sesión]](#exit-guest-session).

La funcionalidad de acceso de invitado permite a las organizaciones [compartir rápidamente los recursos aprobados](../using/brand-portal-sharing-folders.md#how-to-share-folders) con la audiencia deseada a escala sin tener que incorporarlos. A partir de la versión 6.4.2, Brand Portal está equipado para atender a varios usuarios invitados simultáneos, lo que representa el 10% de la cuota total de usuarios por organización. Permitir el acceso de los invitados ahorra tiempo para administrar y incorporar puntuaciones de usuarios con funciones limitadas en Brand Portal.\
Las organizaciones pueden habilitar (o deshabilitar) el acceso de invitados en la cuenta de Brand Portal de la organización mediante la opción **[!UICONTROL Permitir acceso de invitados]** de la configuración **[!UICONTROL Acceso]** del panel de herramientas administrativas.

<!--
Comment Type: annotation
Last Modified By: mgulati
Last Modified Date: 2018-08-17T10:42:59.879-0400
Removed the first para: "AEM Assets Brand Portal allows public users to enter the portal anonymously and have restricted access to the allowed public resources as guests. Organization users with guest role need not seek access and authentication from administrators."
-->

![](assets/enable-guest-access.png)

## Iniciar sesión de invitado {#begin-guest-session}

Para entrar en Brand Portal de forma anónima, seleccione **[!UICONTROL Click here]** correspondiente a **[!UICONTROL Guest Access?]** en la pantalla de bienvenida de Brand Portal. Introduzca la comprobación de seguridad captcha para conceder acceso para utilizar Brand Portal.

![](assets/bp-login-screen.png)

## Duración de la sesión del invitado {#guest-session-duration}


Una sesión de usuario invitado permanece activa durante 15 minutos.
Esto significa que el estado de **[!UICONTROL Lightbox]** se conserva durante 15 minutos desde el inicio de la sesión y, después de eso, la sesión de invitado actual se reinicia para que se pierda el estado de Lightbox.

Por ejemplo, un usuario invitado inicia sesión en Brand Portal a las 15.00 horas y agrega recursos a **[!UICONTROL Lightbox]** para descargarlos a las 15.05 horas. Si el usuario no descarga la colección **[!UICONTROL Lightbox]** (o sus recursos) antes de las 15:15 horas (en los 15 minutos siguientes al inicio de sesión), el usuario debe reiniciar la sesión. El **[!UICONTROL Lightbox]** está vacío, lo que significa que los recursos cargados ya no están disponibles si se perdió la sesión.

## Se permiten sesiones de invitados simultáneos {#concurrent-guest-sessions-allowed}

El número de sesiones de invitados simultáneos está limitado al 10% de la cuota de usuario total por organización. Esto significa que para una organización con una cuota de usuario de 200, un máximo de 20 usuarios invitados pueden trabajar al mismo tiempo. Al usuario 21 se le deniega el acceso y solo puede acceder como invitado si finaliza la sesión de cualquiera de los 20 usuarios invitados activos.

>[!NOTE]
>
>Brand Portal no envía notificaciones si el número de usuarios con licencia supera el valor contratado (cuota). Además, no restringe ninguna actividad de los usuarios con licencia.

## Interacción del usuario invitado con Brand Portal {#guest-user-interaction-with-brand-portal}

### Navegación de IU de invitado

Al entrar en Brand Portal como invitado, los usuarios pueden ver todos los [recursos y carpetas compartidos](../using/brand-portal-sharing-folders.md#sharefolders) públicamente o exclusivamente con usuarios invitados. Esta vista es la vista de solo contenido, que muestra los recursos en cualquiera de los diseños de tarjeta, lista o columna.

![](assets/disabled-folder-hierarchy1.png)

Sin embargo, los usuarios invitados ven el árbol de carpetas (a partir de la carpeta raíz) y las carpetas compartidas organizadas dentro de sus respectivas carpetas principales al iniciar sesión en Brand Portal, si los administradores han habilitado la configuración [Habilitar jerarquía de carpetas](../using/brand-portal-general-configuration.md#main-pars-header-1621071021).

Estas carpetas principales son las carpetas virtuales y no se puede realizar ninguna acción en ellas. Puede reconocer estas carpetas virtuales con un icono de bloqueo.

No hay tareas de acción visibles al pasar el ratón o seleccionarlas en **[!UICONTROL Vista de tarjeta]**, a diferencia de las carpetas compartidas. **** El botón Información general se muestra al seleccionar una carpeta virtual en la vista  **[!UICONTROL de]** columna y la vista de  **[!UICONTROL lista]**.

>[!NOTE]
>
>La miniatura predeterminada de las carpetas virtuales es la imagen en miniatura de la primera carpeta compartida.

![](assets/enabled-hierarchy1.png) ![](assets/hierarchy1-nonadmin.png) ![](assets/hierarchy-nonadmin.png) ![](assets/hierarchy2-nonadmin.png)

**[!UICONTROL La]** opción Ver configuración permite a los usuarios invitados ajustar el tamaño de las tarjetas en las columnas del  **[!UICONTROL visor de]** tarjetas para que se muestren en la vista de  **[!UICONTROL lista]**.

![](assets/nav-guest-user.png)

El **[!UICONTROL árbol de contenido]** le permite moverse por la jerarquía de recursos.

![](assets/guest-login-ui.png)

Brand Portal proporciona la opción **[!UICONTROL Información general]** a los usuarios invitados para ver **[!UICONTROL Propiedades de los recursos]** de los recursos/carpetas seleccionados. La opción **[!UICONTROL Información general]** está visible:

* En la barra de herramientas de la parte superior, seleccione un recurso o una carpeta.
* En la lista desplegable al seleccionar el Selector de carril.

Al seleccionar la opción **[!UICONTROL Información general]** mientras está seleccionado un recurso/carpeta, los usuarios pueden ver el título, la ruta y la hora de creación de los recursos. Mientras que en la página de detalles del recurso, la opción **[!UICONTROL Información general]** permite a los usuarios ver los metadatos del recurso.

![](assets/overview-option-1.png)

![](assets/overview-rail-selector-1.png)

**** La opción de navegación en el carril izquierdo permite navegar de archivos a colecciones y volver a la sesión de invitado para que los usuarios puedan navegar por los recursos en archivos o colecciones.

**** Filteroption permite a los usuarios invitados filtrar archivos de recursos y carpetas utilizando los predicados de búsqueda establecidos por el administrador.

### Capacidades del usuario invitado

Los usuarios invitados pueden acceder a los recursos públicos en Brand Portal y también tienen pocas restricciones, como se explica más adelante.

**Los usuarios invitados pueden**:

* Acceda a todas las carpetas públicas y colecciones destinadas a todos los usuarios de Brand Portal.
* Examine los miembros y la página de detalles, y tenga una vista completa de los recursos de los miembros de todas las carpetas y colecciones públicas.
* Buscar recursos en carpetas públicas y colecciones.
* Agregue recursos a la colección Lightbox. Estos cambios en la colección persisten durante la sesión.
* Descargue recursos directamente o a través de la colección Lightbox.

**Los usuarios invitados no pueden**:

* Cree colecciones y búsquedas guardadas, o compártalas más.
* Acceda a la configuración de carpetas y colecciones.
* Compartir recursos como vínculos.

### Descargar recursos en la sesión de invitado

Los usuarios invitados pueden descargar directamente recursos compartidos pública o exclusivamente con usuarios invitados en Brand Portal. Los usuarios invitados también pueden agregar recursos a **[!UICONTROL Lightbox]** (colección pública) y descargar la colección **[!UICONTROL Lightbox]** antes de que caduque la sesión.

Para descargar recursos y colecciones, utilice el icono de descarga de:

* Miniaturas de acción rápida que aparecen al pasar el ratón por encima del recurso o la colección
* La barra de herramientas de la parte superior, que aparece al seleccionar el recurso o la colección

![](assets/download-on-guest.png)

Al seleccionar **[!UICONTROL Habilitar la aceleración de descarga]** en el cuadro de diálogo [!UICONTROL Descargar] puede [mejorar el rendimiento de descarga](../using/accelerated-download.md).

## Salir de la sesión de invitado {#exit-guest-session}

Para salir de una sesión de invitado, utilice **[!UICONTROL Finalizar sesión]** desde las opciones disponibles en el encabezado. Sin embargo, si la pestaña del explorador utilizada para la sesión del invitado está inactiva, la sesión caducará automáticamente tras dos horas de inactividad.

![](assets/end-guest-session.png)

## Supervisión de las actividades de los usuarios invitados {#monitoring-guest-user-activities}

Los administradores pueden supervisar la interacción del usuario invitado con Brand Portal. Los informes generados en Brand Portal pueden proporcionar perspectivas clave sobre las actividades de los usuarios invitados. Por ejemplo, el informe **[!UICONTROL Download]** se puede utilizar para rastrear el recuento de recursos descargados por el usuario invitado. **[!UICONTROL El informe de]** inicios de sesión del usuario puede informar cuándo el usuario invitado inició sesión por última vez en el portal y la frecuencia de inicios de sesión en un período de tiempo especificado.
