---
title: Acceso de invitado a Brand Portal
seo-title: Acceso de invitado a Brand Portal
description: Permita el acceso de los invitados y ahorre esfuerzos para integrar a numerosos usuarios que no necesitan autenticarse.
seo-description: Permita el acceso de los invitados y ahorre esfuerzos para integrar a numerosos usuarios que no necesitan autenticarse.
uuid: edb4378d-1710-44a2-97a6-594d99f62fff
contentOwner: mgulati
topic-tags: introduction
content-type: reference
products: SG_EXPERIENCEMANAGER/Brand_Portal
discoiquuid: b9e9fe7b-0373-42d1-851b-7c76b47657c2
translation-type: tm+mt
source-git-commit: 1a8658a3ced4fd211a1c1606a80bb51920ca8be1
workflow-type: tm+mt
source-wordcount: '1029'
ht-degree: 1%

---


# Acceso de invitado a Brand Portal {#guest-access-to-brand-portal}

AEM portal de marca permite a los invitados acceder al portal. Un usuario invitado no necesita credenciales para entrar en el portal y tiene acceso a los recursos públicos (y colecciones) del portal. Los usuarios de la sesión de invitados pueden agregar recursos a su caja de luz (colección privada) y descargar el mismo hasta que dure la sesión, es decir, 2 horas desde el comienzo de la sesión, a menos que el usuario invitado elija [[!UICONTROL Finalizar sesión]](#exit-guest-session).

La funcionalidad de acceso de invitados permite a las organizaciones [compartir rápidamente los activos aprobados](../using/brand-portal-sharing-folders.md#how-to-share-folders) con la audiencia prevista a escala sin tener que incorporarlos. A partir de la versión 6.4.2, Brand Portal está equipado para servir a varios usuarios invitados simultáneos, lo que representa el 10 % de la cuota total de usuarios por organización. Permitir el acceso de los invitados ahorra tiempo para administrar y agregar puntuaciones de usuarios que necesitan usar funcionalidades limitadas en Brand Portal.\
Las organizaciones pueden habilitar (o deshabilitar) el acceso de invitados en la cuenta de Brand Portal de la organización mediante la opción **[!UICONTROL Permitir acceso de invitados]** de la configuración de **[!UICONTROL Access]** del panel de herramientas administrativas.

<!--
Comment Type: annotation
Last Modified By: mgulati
Last Modified Date: 2018-08-17T10:42:59.879-0400
Removed the first para: "AEM Assets Brand Portal allows public users to enter the portal anonymously and have restricted access to the allowed public resources as guests. Organization users with guest role need not seek access and authentication from administrators."
-->

![](assets/enable-guest-access.png)

## Iniciar sesión de invitado {#begin-guest-session}

Para ingresar a Brand Portal de forma anónima, seleccione **[!UICONTROL Haga clic aquí]** correspondiente a **[!UICONTROL Acceso de invitado?]** en la pantalla de bienvenida de Brand Portal. Introduzca la comprobación de seguridad catcha para conceder acceso a la utilización del portal de marca.

![](assets/bp-login-screen.png)

## Duración de la sesión de invitado {#guest-session-duration}


Una sesión de usuario invitado permanece activa durante 15 minutos.
Esto significa que el estado del **[!UICONTROL Lightbox]** se conserva durante 15 minutos desde el inicio de sesión y, después, se reinicia la sesión de invitado actual para que se pierda el estado del Lightbox.

Por ejemplo, un usuario invitado inicia sesión en Brand Portal a las 15.00 horas y agrega recursos a **[!UICONTROL Lightbox]** para descargarlos a las 15.05 horas. Si el usuario no descarga la colección **[!UICONTROL Lightbox]** (o sus recursos) antes de las 15:15 horas (en los 15 minutos posteriores al inicio de sesión), tendrá que reiniciar la sesión. El **[!UICONTROL Lightbox]** estará vacío, lo que significa que los recursos cargados ya no estarán disponibles si se perdió la sesión.

## Sesiones de invitados simultáneas permitidas {#concurrent-guest-sessions-allowed}

El número de sesiones de invitados simultáneas está limitado al 10 % de la cuota total de usuarios por organización. Esto significa que para una organización con una cuota de usuario de 200, un máximo de 20 usuarios invitados pueden trabajar al mismo tiempo. Al usuario número 21 se le deniega el acceso y solo puede acceder como invitado si finaliza la sesión de cualquiera de los 20 usuarios invitados activos.

## Interacción del usuario invitado con Brand Portal {#guest-user-interaction-with-brand-portal}

### Navegación de la interfaz de usuario del invitado

Al entrar en Brand Portal como invitado, los usuarios pueden ver todos los [recursos y carpetas compartidos](../using/brand-portal-sharing-folders.md#sharefolders) públicamente o con usuarios invitados exclusivamente. Esta vista es la vista de contenido único, que muestra los recursos en cualquiera de los diseños de tarjeta, lista o columna.

![](assets/disabled-folder-hierarchy1.png)

Sin embargo, los usuarios invitados ven el árbol de carpetas (a partir de la carpeta raíz) y las carpetas compartidas organizadas dentro de sus respectivas carpetas principales al iniciar sesión en Brand Portal, si los administradores han habilitado la configuración [Habilitar jerarquía de carpetas](../using/brand-portal-general-configuration.md#main-pars-header-1621071021).

Estas carpetas principales son las carpetas virtuales y no se pueden realizar acciones en ellas. Puede reconocer estas carpetas virtuales con un icono de candado.

No hay tareas de acción visibles al pasar el ratón por encima o seleccionarlas en **[!UICONTROL Vista de tarjeta]**, a diferencia de las carpetas compartidas. **[!UICONTROL El botón]** Información general se muestra al seleccionar una carpeta virtual en la Vista **[!UICONTROL de]** vista de  **[!UICONTROL columna y]** Lista.

>[!NOTE]
>
>La miniatura predeterminada de las carpetas virtuales es la imagen en miniatura de la primera carpeta compartida.

![](assets/enabled-hierarchy1.png) ![](assets/hierarchy1-nonadmin.png) ![](assets/hierarchy-nonadmin.png) ![](assets/hierarchy2-nonadmin.png)

**[!UICONTROL La opción]** Configuración de vistas permite a los usuarios invitados ajustar el tamaño de las tarjetas en las columnas  **[!UICONTROL del]** visor de tarjetas para que se muestren en la Vista **[!UICONTROL de]** Listas.

![](assets/nav-guest-user.png)

El **[!UICONTROL árbol de contenido]** le permite moverse por la jerarquía de recursos.

![](assets/guest-login-ui.png)

Brand Portal ofrece a los usuarios invitados la opción **[!UICONTROL Información general]** para la vista **[!UICONTROL Propiedades del recurso]** de los recursos/carpetas seleccionados. La opción **[!UICONTROL Overview]** está visible:

* En la barra de herramientas de la parte superior, seleccione un recurso o una carpeta.
* En la lista desplegable al seleccionar el Selector de raíl.
Al seleccionar la opción **[!UICONTROL Información general]** mientras se selecciona un recurso o carpeta, los usuarios pueden ver el título, la ruta y la hora de creación de recursos. Mientras que, en la página de detalles del recurso, si selecciona la opción **[!UICONTROL Información general]**, los usuarios pueden ver los metadatos del recurso.

![](assets/overview-option-1.png)

![](assets/overview-rail-selector-1.png)<br />

**[!UICONTROL La opción]** Navegación en el carril izquierdo permite desplazarse de archivos a colecciones y volver a la sesión de invitado para que los usuarios puedan navegar por los recursos de archivos o colecciones.

**** Filteroption permite a los usuarios invitados filtrar archivos y carpetas de recursos mediante predicados de búsqueda establecidos por el administrador.

### Funciones de usuario invitado

Los usuarios invitados pueden acceder a los recursos públicos de Brand Portal y también tienen pocas restricciones, como se explica más adelante.

**Los usuarios invitados pueden**:

* Acceda a todas las carpetas públicas y colecciones destinadas a todos los usuarios de Brand Portal.
* Examinar los miembros, la página de detalles y la vista de recursos completa de los miembros de todas las carpetas y colecciones públicas.
* Buscar recursos en carpetas y colecciones públicas.
* Añada los recursos en una colección de Lightbox. Estos cambios en la colección persisten durante la sesión.
* Descargue recursos directamente o a través de una colección de Lightbox.

**Los usuarios invitados no pueden**:

* Cree colecciones y búsquedas guardadas, o compártalas más.
* Acceda a la configuración de carpetas y colecciones.
* Compartir recursos como vínculos.

### Descargar recursos en la sesión de invitados

Los usuarios invitados pueden descargar directamente recursos compartidos pública o exclusivamente con usuarios invitados en Brand Portal. Los usuarios invitados también pueden agregar recursos a **[!UICONTROL Lightbox]** (colección pública) y descargar la colección **[!UICONTROL Lightbox]** antes de que caduque la sesión.

Para descargar recursos y colecciones, utilice el icono de descarga de:

* Miniaturas de acción rápida, que aparecen al pasar el ratón sobre el recurso o la colección
* La barra de herramientas de la parte superior, que aparece al seleccionar el recurso o la colección

![](assets/download-on-guest.png)

Si selecciona **[!UICONTROL Habilitar la aceleración de descarga]** en el cuadro de diálogo [!UICONTROL Descargar], podrá [mejorar el rendimiento de descarga](../using/accelerated-download.md).

## Salir de la sesión de invitado {#exit-guest-session}

Para salir de una sesión de invitado, utilice **[!UICONTROL Finalizar sesión]** desde las opciones disponibles en el encabezado. Sin embargo, si la ficha del explorador utilizada para la sesión de invitado está inactiva, la sesión caduca automáticamente tras dos horas de inactividad.

![](assets/end-guest-session.png)

## Monitoreo de actividades de usuarios invitados {#monitoring-guest-user-activities}

Los administradores pueden supervisar la interacción del usuario invitado con Brand Portal. Los informes generados en Brand Portal pueden proporcionar información clave sobre las actividades de los usuarios invitados. Por ejemplo: el informe **[!UICONTROL Descargar]** puede utilizarse para rastrear el recuento de recursos descargados por el usuario invitado. **[!UICONTROL El informe de]** inicios de sesión del usuario puede informar en qué momento el usuario invitado inició sesión por última vez en el portal y la frecuencia de inicios de sesión en un período de tiempo especificado.
