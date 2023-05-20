---
title: Acceso de invitado a Brand Portal
seo-title: Guest Access to Brand Portal
description: Permitir el acceso de invitados y ahorrar el esfuerzo para incorporar varios usuarios sin autenticación.
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

Experience Manager Assets Brand portal permite el acceso de invitados al portal. Una usuario de invitado no necesita credenciales para entrar al portal y tiene acceso a los activos públicos (y colecciones) del portal. Los usuarios en la sesión de invitado pueden añadir recursos a lightbox (colección privada) y descargar lo mismo hasta que dure su sesión, que es de 2 horas desde el principio de la sesión a menos que el usuario invitado elija [[!UICONTROL Finalizar sesión]](#exit-guest-session).

El acceso de invitados funcionalidad permite a las organizaciones [ compartir rápidamente activos ](../using/brand-portal-sharing-folders.md#how-to-share-folders) aprobados con la audiencia prevista a escala, sin necesidad de incorporarlos. Brand portal 6.4.2 está preparado para servir a varios usuarios invitados simultáneos, que es el 10% del total de usuario cuota por organización. Permitir el acceso de invitados ahorra tiempo a administrar y a las puntuaciones de los usuarios tablero con funcionalidades limitadas en Brand portal.\
Las organizaciones pueden habilitar (o deshabilitar) el acceso de invitados en Brand portal cuenta de la organización mediante **[!UICONTROL la opción Permitir acceso]** de invitado de **[!UICONTROL configuración de acceso]** en el panel Herramientas administrativas.

<!--
Comment Type: annotation
Last Modified By: mgulati
Last Modified Date: 2018-08-17T10:42:59.879-0400
Removed the first para: "AEM Assets Brand Portal allows public users to enter the portal anonymously and have restricted access to the allowed public resources as guests. Organization users with guest role need not seek access and authentication from administrators."
-->

![](assets/enable-guest-access.png)

## Iniciar sesión de invitado {#begin-guest-session}

Para especificar el portal de marca de forma anónima, seleccione **[!UICONTROL haga clic aquí]** correspondiente al acceso de **[!UICONTROL invitado?]** pantalla de bienvenida del portal de marca. Introduzca la comprobación de seguridad captcha para conceder acceso y utilizar Brand Portal.

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

### Navegación IU de invitados

Al introducir el portal de marca como invitado, los usuarios pueden ver todos los [ activos y carpetas compartidos ](../using/brand-portal-sharing-folders.md#sharefolders) públicamente o con usuarios invitados exclusivamente. Esta vista es la contenido solo vista, que muestra activos en cualquiera de las distribuciones de tarjeta, lista o columna.

![](assets/disabled-folder-hierarchy1.png)

Sin embargo, los usuarios invitados ven el árbol de carpetas (a partir de la carpeta raíz) y las carpetas compartidas organizadas dentro de sus respectivas carpetas principales en registro en el portal de marca, si los administradores han habilitado [ la configuración de jerarquía ](../using/brand-portal-general-configuration.md#main-pars-header-1621071021) de carpeta.

Estas carpetas principales son las carpetas virtuales y no se pueden realizar acciones en ellas. Puede reconocer estas carpetas virtuales con un icono de candado.

No hay tareas de acción visibles al pasar el ratón por encima o seleccionarlas en **[!UICONTROL Vista de tarjeta]**, a diferencia de las carpetas compartidas. **[!UICONTROL Información general]** botón se muestra en la selección de una carpeta virtual en ver ]**de**[!UICONTROL  columna y **[!UICONTROL lista Ver]** .

>[!NOTE]
>
>La miniatura predeterminada de las carpetas virtuales es la imagen en miniatura de la primera carpeta compartida.

![](assets/enabled-hierarchy1.png) ![](assets/hierarchy1-nonadmin.png) ![](assets/hierarchy-nonadmin.png) ![](assets/hierarchy2-nonadmin.png)

**[!UICONTROL Ver opción Configuración]** permite a los usuarios invitados ajustar los tamaños de tarjeta en **[!UICONTROL las columnas ver]** o de la tarjeta para que se muestren en **[!UICONTROL la lista Ver]** .

![](assets/nav-guest-user.png)

El árbol ]**de**[!UICONTROL  contenido permite desplazarse por activos jerarquía.

![](assets/guest-login-ui.png)

Brand portal ofrece **[!UICONTROL una opción de Resumen]** a los usuarios invitados a vista **[!UICONTROL propiedades]** de recursos de activos/carpetas seleccionadas. La **[!UICONTROL opción Resumen]** es visible:

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
* Añadir activos en caja de luz colección. Estos cambios en la colección persisten durante la sesión.
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

Los administradores pueden monitor interacción usuario invitado con el portal de marca. Los informes generados en Brand portal pueden proporcionar información clave sobre las actividades de usuario de huésped. Por ejemplo, **[!UICONTROL se puede utilizar descargar]** Informe para rastrear el recuento de activos descargado por la usuario de invitado. **[!UICONTROL El informe de inicios de sesión]** de usuario puede informar del momento en el que el invitado usuario la última vez que inició sesión en el portal y frecuencia de inicio de sesión en una duración determinada.
