---
title: Acceso de invitados a Brand Portal
seo-title: Acceso de invitados a Brand Portal
description: Permitir el acceso de los invitados y guardar el esfuerzo por parte de numerosos usuarios que no necesitan autenticarse.
seo-description: Permitir el acceso de los invitados y guardar el esfuerzo por parte de numerosos usuarios que no necesitan autenticarse.
uuid: edb 4378 d -1710-44 a 2-97 a 6-594 d 99 f 62 fff
contentOwner: mgulati
topic-tags: introducción
content-type: referencia
products: SG_ EXPERIENCEMANAGER/Brand_ Portal
discoiquuid: b 9 e 9 fe 7 b -0373-42 d 1-851 b -7 c 76 b 47657 c 2
translation-type: tm+mt
source-git-commit: 770c353b1143d879280df310012ce9d4d30b40c9

---


# Acceso de invitados a Brand Portal {#guest-access-to-brand-portal}

[!DNL AEM Brand portal] permite al invitado acceder al portal. Un usuario invitado no necesita credenciales para entrar en el portal y tiene acceso a los recursos públicos (y colecciones) del portal. Los usuarios de la sesión de invitados pueden agregar recursos a su cuadro de luz (colección privada) y descargarlos hasta que dure la sesión, que es de 2 horas desde el principio de la sesión, a menos que el usuario invitado elija [Finalizar sesión](#exit-guest-session).

La funcionalidad de acceso invitado permite a las organizaciones compartir [rápidamente los recursos](../using/brand-portal-sharing-folders.md#how-to-share-folders) aprobados con la audiencia deseada a escala sin tener que tableros. [!DNL Brand Portal] 6.4.2 a partir de la versión 6.4.2, se proporciona a varios usuarios invitados simultáneos, que es el 10% de la cuota total de usuarios por organización. Permitir el acceso de los invitados ahorra tiempo para administrar y puntuaciones en el tablero de usuarios que necesitan utilizar funciones limitadas en [!DNL Brand Portal].\
Las organizaciones pueden habilitar (o deshabilitar) el acceso de invitados en [!DNL Brand Portal] cuenta de la organización mediante **la opción Permitir acceso** a invitados desde **los ajustes de acceso** en el panel Herramientas administrativas.

<!--
Comment Type: annotation
Last Modified By: mgulati
Last Modified Date: 2018-08-17T10:42:59.879-0400
Removed the first para: "AEM Assets Brand Portal allows public users to enter the portal anonymously and have restricted access to the allowed public resources as guests. Organization users with guest role need not seek access and authentication from administrators."
-->

![](assets/enable-guest-access.png)

## Comenzar sesión invitado {#begin-guest-session}

Para entrar en Brand Portal de forma anónima, seleccione **[!UICONTROL Haga clic aquí]** correspondiente al **[!UICONTROL acceso de invitados?]** en [!DNL Brand Portal] la pantalla de bienvenida. Los usuarios no tienen que buscar el acceso y esperar a que el administrador los autentique para que conceda [!DNL Brand Portal]acceso.

![](assets/bp-login-screen.png)

## Duración de la sesión del invitado {#guest-session-duration}

Una sesión de usuario invitado permanece activa durante 2 horas. Esto significa que el estado de [!UICONTROL la caja de luz] se conserva hasta 1 hora desde la hora de inicio de la sesión, y después de 2 horas la sesión de invitado actual se reinicia para que se pierda el estado de la caja de iluminación.\
Por ejemplo, un usuario invitado inicia sesión en [!DNL Brand Portal] 1500 horas y añade recursos a Lightbox para descargar a las 16:50 horas. Si el usuario no descarga la colección [!UICONTROL Lightbox (] o sus recursos) antes de las 17:00 horas, la [!UICONTROL caja de iluminación] quedará vacía ya que el usuario tendrá que reiniciar la sesión al final de 1 hora (es decir, 1700 horas).

## Sesiones de invitados simultáneas permitidas {#concurrent-guest-sessions-allowed}

El número de sesiones de invitados simultáneas está limitado al 10% de la cuota total de usuarios por organización. Esto significa que para una organización con cuota de usuario de 200, los 20 usuarios invitados máximos pueden trabajar al mismo tiempo. Al usuario XXI se le deniega el acceso y solo podrá acceder como invitado cuando finalice la sesión de cualquiera de los 20 usuarios invitados activos.

## Interacción del usuario invitado con Brand Portal {#guest-user-interaction-with-brand-portal}

### Navegación de IU invitados

Al ingresar [!DNL Brand Portal] como invitado, los usuarios pueden ver todos los [recursos y carpetas compartidos](../using/brand-portal-sharing-folders.md#sharefolders) públicamente o con usuarios invitados exclusivamente. Esta vista es la vista de contenido únicamente, que muestra los recursos en los diseños de tarjetas, listas o columnas.

![](assets/disabled-folder-hierarchy1.png)

Sin embargo, los usuarios invitados ven el árbol de carpetas (empezando por la carpeta raíz) y las carpetas compartidas organizadas en sus respectivas carpetas principales al iniciar sesión en [!DNL Brand Portal], si los administradores han habilitado [la configuración de Habilitar jerarquía](../using/brand-portal-general-configuration.md#main-pars-header-1621071021) de carpetas.

Estas carpetas principales son las carpetas virtuales y no se pueden realizar acciones en ellas. Puede reconocer estas carpetas virtuales con un icono de candado.

No hay tareas de acción visibles al desplazarse o seleccionarlas en Vista de tarjeta, a diferencia de las carpetas compartidas. El botón Información general se muestra al seleccionar una carpeta virtual en Vista de columna y Vista de lista.

>[!NOTE]
>
>Tenga en cuenta que la miniatura predeterminada de las carpetas virtuales es la imagen en miniatura de la primera carpeta compartida.

![](assets/enabled-hierarchy1.png) ![](assets/hierarchy1-nonadmin.png) ![](assets/hierarchy-nonadmin.png) ![](assets/hierarchy2-nonadmin.png)

La opción Configuración de visualización permite a los usuarios invitados ajustar los tamaños de tarjeta en la vista de tarjeta o en las columnas para mostrarlos en la vista de lista.

![](assets/nav-guest-user.png)

El árbol de contenido permite desplazarse por la jerarquía de recursos.

![](assets/guest-login-ui.png)

[!DNL Brand Portal] Proporciona **la opción Información general** a los usuarios invitados para ver las propiedades de recursos de los recursos o carpetas seleccionados. La opción Información general está visible:

1. En la barra de herramientas situada en la parte superior de la selección de un recurso o carpeta.
2. En la lista desplegable de selección del Selector de raíl.

Al seleccionar la opción Información general mientras se selecciona un recurso o carpeta, los usuarios pueden ver el título, la ruta y la hora de creación de recursos. En cambio, en la página de detalles del recurso, la opción Información general permite que los usuarios vean metadatos del recurso.

![](assets/overview-option-1.png)

![](assets/overview-rail-selector-1.png)

**[!UICONTROL La opción de navegación]** en el carril izquierdo permite navegar de los archivos a [!UICONTROL las colecciones] y de volver a la sesión de invitados para que los usuarios puedan explorar los recursos en archivos o [!UICONTROL colecciones].

**La opción Filtro** permite a los usuarios invitados filtrar archivos y carpetas de recursos mediante predicados de búsqueda establecidos por el administrador.

### Capacidades de usuario invitado

Los usuarios invitados pueden acceder a los recursos públicos y [!DNL Brand Portal]también tener pocas restricciones como se analiza más adelante.

Los usuarios invitados pueden:

* acceso a todas las carpetas y [!UICONTROL colecciones públicas] destinadas a todos los [!DNL Brand Portal] usuarios.
* los miembros de examinar, la página de detalles y la vista de recursos completa de los miembros de todas las carpetas y [!UICONTROL colecciones públicas].
* buscar recursos en carpetas y [!UICONTROL colecciones públicas].
* agregar recursos a [!UICONTROL la colección Lightbox]. Durante la sesión, se mantienen estos cambios en [!UICONTROL la colección] .
* descargar recursos directamente o a través [!UICONTROL de colecciones Lightbox].

Los usuarios invitados no pueden:

* crear [!UICONTROL colecciones] y búsquedas guardadas, o compartirlas aún más.
* carpeta de acceso y [!UICONTROL colecciones] .
* compartir recursos como vínculos.

### Descarga de recursos en sesión de invitado

Los usuarios invitados pueden descargar directamente recursos compartidos públicamente o exclusivamente con usuarios invitados. [!DNL Brand Portal] Los usuarios invitados también pueden agregar recursos a [!UICONTROL Lightbox] ( [!UICONTROL colección pública]) y descargar la colección [!UICONTROL de Lightbox] antes de que caduque la sesión.

Para descargar recursos y [!UICONTROL colecciones], utilice el icono de descarga de:

* miniaturas de acción rápida, que aparecen al pasar el ratón sobre el recurso o [!UICONTROL la colección]
* la barra de herramientas situada en la parte superior, que aparece al seleccionar el recurso o [!UICONTROL la colección]

![](assets/download-on-guest.png)

Si selecciona **Activar aceleración de descarga** en el cuadro de diálogo Descargar [, podrá mejorar el rendimiento de descarga](../using/accelerated-download.md).

## Salir de la sesión del invitado {#exit-guest-session}

Para salir de una sesión de invitado, utilice **Finalizar sesión** de las opciones disponibles en el encabezado. Sin embargo, si la ficha del explorador para la sesión de invitado está inactiva, la sesión caducará automáticamente después de dos horas de inactividad.

![](assets/end-guest-session.png)

## Supervisión de actividades de usuarios invitados {#monitoring-guest-user-activities}

Los administradores pueden supervisar la interacción del usuario invitado con [!DNL Brand Portal]el. Los informes generados proporcionan [!DNL Brand Portal] perspectivas clave sobre las actividades de los usuarios invitados. Por ejemplo, **Descargar** informe puede utilizarse para rastrear el recuento de recursos descargados por el usuario invitado. **Informe Inicios** de sesión de usuario puede informar cuando el usuario invitado inició sesión por última vez en el portal y la frecuencia de inicios de sesión en una duración especificada.
