---
title: Acceso de invitado a Brand Portal
seo-title: Guest Access to Brand Portal
description: Permita el acceso de invitados y ahorre el esfuerzo de incorporar numerosos usuarios sin autenticación.
seo-description: Allow guest access and save the effort to onboard numerous users without authentication.
uuid: edb4378d-1710-44a2-97a6-594d99f62fff
contentOwner: VG
topic-tags: introduction
content-type: reference
products: SG_EXPERIENCEMANAGER/Brand_Portal
discoiquuid: b9e9fe7b-0373-42d1-851b-7c76b47657c2
exl-id: ecce0a45-abae-41c4-9ea7-5dfdcf19e5ea
source-git-commit: 0670b8d372fd2dc5bdb1d0a928601e3e09a6dcf9
workflow-type: tm+mt
source-wordcount: '1026'
ht-degree: 0%

---

# Acceso de invitado a Brand Portal {#guest-access-to-brand-portal}

Experience Manager Assets Brand Portal permite el acceso de invitados al portal. Un usuario invitado no necesita credenciales para entrar al portal y tiene acceso a los activos públicos (y colecciones) del portal. Los usuarios en la sesión de invitado pueden añadir recursos a lightbox (colección privada) y descargarlos hasta que la sesión dure o a menos que el usuario invitado elija [[!UICONTROL Finalizar sesión]](#exit-guest-session). Una sesión de usuario invitado permanece activa durante 15 minutos.

La funcionalidad de acceso de invitado permite a las organizaciones [compartir rápidamente los recursos aprobados](../using/brand-portal-sharing-folders.md#how-to-share-folders) con la audiencia a escala sin tener que incorporarla. Brand Portal 6.4.2 y versiones posteriores están equipadas para atender a varios usuarios invitados simultáneos, lo que representa el 10 % de la cuota total de usuarios por organización. Al permitir el acceso de invitados, se ahorra tiempo para administrar e incorporar puntuaciones de usuarios con funcionalidades limitadas en Brand Portal.\
Las organizaciones pueden habilitar (o deshabilitar) el acceso de invitados en la cuenta de Brand Portal de la organización mediante **[!UICONTROL Permitir el acceso de invitados]** opción de **[!UICONTROL Acceso]** configuración en el panel herramientas administrativas.

<!--
Comment Type: annotation
Last Modified By: mgulati
Last Modified Date: 2018-08-17T10:42:59.879-0400
Removed the first para: "AEM Assets Brand Portal allows public users to enter the portal anonymously and have restricted access to the allowed public resources as guests. Organization users with guest role need not seek access and authentication from administrators."
-->

![](assets/enable-guest-access.png)

## Comenzar sesión de invitado {#begin-guest-session}

Para introducir Brand Portal de forma anónima, seleccione **[!UICONTROL Haga clic aquí]** correspondiente a **[!UICONTROL ¿Acceso de invitado?]** en la pantalla de bienvenida de Brand Portal. Introduzca la comprobación de seguridad captcha para conceder acceso y utilizar Brand Portal.

![](assets/bp-login-screen.png)

## Duración de sesión de invitado {#guest-session-duration}

Una sesión de usuario invitado permanece activa durante 15 minutos.
Esto significa que el estado del **[!UICONTROL Lightbox]** se conserva durante 15 minutos a partir de la hora de inicio de la sesión y, después, la sesión de invitado actual se reinicia para que se pierda el estado de Lightbox.

Por ejemplo, un usuario invitado inicia sesión en Brand Portal a las 15:00 horas y agrega recursos a **[!UICONTROL Lightbox]** para descargar a las 15:05 horas. Si el usuario no descarga la **[!UICONTROL Lightbox]** (o sus recursos) antes de las 15:15 horas (en los 15 minutos siguientes al inicio de sesión), el usuario debe reiniciar la sesión. El **[!UICONTROL Lightbox]** está vacío, lo que significa que los recursos cargados ya no están disponibles si se perdió la sesión.

## Sesiones de invitado simultáneas permitidas {#concurrent-guest-sessions-allowed}

El número de sesiones de invitado simultáneas está limitado al 10 % de la cuota total de usuarios por organización. Significa que para una organización con una cuota de usuario de 200, un máximo de 20 usuarios invitados pueden trabajar al mismo tiempo. Se deniega el acceso al usuario número 21 y solo puede acceder como invitado si finaliza la sesión de cualquiera de los 20 usuarios invitados activos.

>[!NOTE]
>
>Brand Portal no envía notificaciones si el número de usuarios con licencia supera el valor contratado (cuota). Además, no restringe ninguna actividad de los usuarios con licencia.

## Interacción del usuario invitado con Brand Portal {#guest-user-interaction-with-brand-portal}

### Navegación de IU de invitado

Al entrar en Brand Portal como invitado, los usuarios pueden ver todas las [recursos y carpetas compartidos](../using/brand-portal-sharing-folders.md#sharefolders) de manera pública o con usuarios invitados exclusivamente. Esta vista es la vista solo de contenido, que muestra los recursos en cualquiera de los diseños de tarjeta, lista o columna.

![](assets/disabled-folder-hierarchy1.png)

Sin embargo, los usuarios invitados ven el árbol de carpetas (a partir de la carpeta raíz) y las carpetas compartidas organizadas dentro de sus respectivas carpetas principales al iniciar sesión en Brand Portal, si los administradores han habilitado [Habilitar la jerarquía de carpetas](../using/brand-portal-general-configuration.md#main-pars-header-1621071021) configuración.

Estas carpetas principales son las carpetas virtuales y no se pueden realizar acciones en ellas. Puede reconocer estas carpetas virtuales con un icono de candado.

No hay tareas de acción visibles al pasar el ratón por encima o seleccionarlas en **[!UICONTROL Vista de tarjeta]**, a diferencia de las carpetas compartidas. **[!UICONTROL Información general]** se muestra al seleccionar una carpeta virtual en **[!UICONTROL Vista de columna]** y **[!UICONTROL Vista de lista]**.

>[!NOTE]
>
>La miniatura predeterminada de las carpetas virtuales es la imagen en miniatura de la primera carpeta compartida.

![](assets/enabled-hierarchy1.png) ![](assets/hierarchy1-nonadmin.png) ![](assets/hierarchy-nonadmin.png) ![](assets/hierarchy2-nonadmin.png)

**[!UICONTROL Configuración de vista]** permite a los usuarios invitados ajustar el tamaño de las tarjetas en **[!UICONTROL Vista de tarjeta]** o columnas para mostrar en **[!UICONTROL Vista de lista]**.

![](assets/nav-guest-user.png)

El **[!UICONTROL Árbol de contenido]** permite desplazarse por la jerarquía de recursos.

![](assets/guest-login-ui.png)

Brand Portal proporciona **[!UICONTROL Información general]** opción para que los usuarios invitados la vean **[!UICONTROL Propiedades del recurso]** de recursos o carpetas seleccionados. El **[!UICONTROL Información general]** La opción está visible:

* En la barra de herramientas de la parte superior, al seleccionar un recurso o una carpeta.
* En la lista desplegable, seleccione el Selector de carril.

Al seleccionar la variable **[!UICONTROL Información general]** opción mientras hay un recurso o una carpeta seleccionados, los usuarios pueden ver el título, la ruta y la hora de creación del recurso. Mientras que en la página de detalles de recursos se selecciona **[!UICONTROL Información general]** La opción permite a los usuarios ver los metadatos del recurso.

![](assets/overview-option-1.png)

![](assets/overview-rail-selector-1.png)

**[!UICONTROL Navegación]** en el carril izquierdo permite navegar de archivos a colecciones y volver a la sesión de invitado para que los usuarios puedan navegar por los recursos de archivos o colecciones.

**[!UICONTROL Filtrar]** permite a los usuarios invitados filtrar archivos y carpetas de recursos mediante predicados de búsqueda establecidos por el administrador.

### Funcionalidades de usuario invitado

Los usuarios invitados pueden acceder a recursos públicos en Brand Portal y también tienen algunas restricciones, tal como se explica más adelante.

**Los usuarios invitados pueden**:

* Acceda a todas las carpetas públicas y colecciones destinadas a todos los usuarios de Brand Portal.
* Examine miembros, páginas de detalles y obtenga una vista completa de los recursos de los miembros de todas las carpetas y colecciones públicas.
* Busque recursos en carpetas y colecciones públicas.
* Añadir recursos a la colección Lightbox. Estos cambios en la colección persisten durante la sesión.
* Descargue recursos directamente o a través de la colección Lightbox.

**Los usuarios invitados no pueden**:

* Cree colecciones y búsquedas guardadas, o compártalas más.
* Acceder a la configuración de carpetas y colecciones.
* Compartir recursos como vínculos.

### Descargar recursos en la sesión de invitado

Los usuarios invitados pueden descargar directamente recursos compartidos de forma pública o exclusiva con usuarios invitados en Brand Portal. Los usuarios invitados también pueden agregar recursos a **[!UICONTROL Lightbox]** (colección pública) y descargue el **[!UICONTROL Lightbox]** antes de que caduque su sesión.

Para descargar recursos y colecciones, utilice el icono de descarga de:

* Miniaturas de acciones rápidas, que aparecen al pasar el ratón por encima del recurso o la colección
* La barra de herramientas de la parte superior, que aparece al seleccionar el recurso o la colección

![](assets/download-on-guest.png)

Seleccionar **[!UICONTROL Habilitar la aceleración de descarga]** el [!UICONTROL Descargar] El cuadro de diálogo permite [mejorar el rendimiento de descarga](../using/accelerated-download.md).

## Salir de la sesión de invitado {#exit-guest-session}

Para salir de una sesión de invitado, utilice **[!UICONTROL Finalizar sesión]** en las opciones disponibles en el encabezado. Sin embargo, si la pestaña del explorador utilizada para la sesión de invitado está inactiva, la sesión caducará automáticamente tras dos horas de inactividad.

![](assets/end-guest-session.png)

## Monitorización de actividades de usuarios invitados {#monitoring-guest-user-activities}

Los administradores pueden monitorizar la interacción de los usuarios invitados con Brand Portal. Los informes generados en Brand Portal pueden proporcionar perspectivas clave sobre las actividades de los usuarios invitados. Por ejemplo, **[!UICONTROL Descargar]** Este informe se puede utilizar para hacer un seguimiento del recuento de recursos descargados por el usuario invitado. **[!UICONTROL Inicios de sesión de usuario]** Este informe puede informar cuándo inició sesión el usuario invitado por última vez en el portal y la frecuencia de inicios de sesión en una duración especificada.
