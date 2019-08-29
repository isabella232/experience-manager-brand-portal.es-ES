---
title: Novedades de AEM Assets Brand Portal
seo-title: Novedades de AEM Assets Brand Portal
description: Eche un vistazo a las nuevas funciones y mejoras de 6.4.4.
seo-description: Eche un vistazo a las nuevas funciones y mejoras de 6.4.4.
uuid: 2 c 59 d 738-9 b 53-4 f 25-a 205-13 bf 75 c 80 b 77
contentOwner: bdhar
products: SG_ EXPERIENCEMANAGER/Brand_ Portal
content-type: referencia
topic-tags: introducción
discoiquuid: fec 32 ca 3-142 b -4 a 11-9 b 92-5113 fc 27277 a
translation-type: tm+mt
source-git-commit: cbb64eb8a79480a1ccedbe5131a38ddf6eaec88d

---


# Novedades de AEM Assets Brand Portal {#what-s-new-in-aem-assets-brand-portal}

Adobe Experience Manager (AEM) Assets Brand Portal le ayuda a adquirir, controlar y distribuir fácilmente recursos creativos aprobados a usuarios externos y a usuarios internos de la empresa entre dispositivos. Ayuda a mejorar la eficacia del uso compartido de recursos, acelera el tiempo de comercialización de los recursos y reduce el riesgo de acceso no autorizado y no autorizado. Adobe está trabajando para mejorar la experiencia general de Brand Portal. Este es un paso nuevo en las nuevas funciones y mejoras.

## ¿Qué ha cambiado en 6.4.4? {#what-is-changing-in}

Brand Portal 6.4.4 se centra en las mejoras de la búsqueda de texto y las solicitudes principales de los clientes. Consulte las últimas [Notas de la versión de Brand Portal](brand-portal-release-notes.md).

### Mejoras de búsqueda {#search-enhancements}

Brand Portal 6.4.4 y posteriores admite la búsqueda parcial de texto en predicado de propiedad en el panel de filtrado. Para permitir la búsqueda parcial de texto necesita habilitar **la búsqueda parcial** en Predicado de propiedad en el formulario de búsqueda.

Continúe leyendo para obtener más información sobre la búsqueda de texto parcial y la búsqueda comodín.

#### Búsqueda parcial de frases {#partial-phrase-search}

Ahora puede buscar recursos especificando solamente una parte (una palabra o dos) de la frase buscada en el panel de filtrado.

**La búsqueda**de frases parciales es
útil cuando no está seguro de la combinación exacta de palabras que se producen en la frase de búsqueda.

Por ejemplo, si el formulario de búsqueda en Brand Portal utiliza Predicado de propiedad para buscar parcialmente el título de recursos, especificando el término **camp** devuelve todos los recursos con la palabra camp en la frase de título.

![](assets/partialphrasesearch.png)

#### Búsqueda comodín {#wildcard-search}

Brand Portal permite utilizar el asterisco (*) en la consulta de búsqueda junto con una parte de la palabra en la frase de búsqueda.

**Caso
de uso** Si no está seguro de las palabras exactas que se producen en la frase de búsqueda, puede utilizar una búsqueda comodín para rellenar los huecos en la consulta de búsqueda.

Por ejemplo, si se especifica **una escalada *** , se devuelven todos los recursos que tengan palabras que comienzan con los caracteres **en** la frase de título si el formulario de búsqueda en Brand Portal utiliza Predicado de propiedad para la búsqueda parcial del título de recursos.

![](assets/wildcard-prop.png)

De manera similar, especifique:

* *** sube** devuelve todos los recursos que tienen palabras que terminan con caracteres **escalada** en la frase del título.

* *** escalada *** devuelve todos los recursos que tienen palabras que comprenden los caracteres **en** la frase de título.

>[!NOTE]
>
>Al seleccionar **la casilla de verificación Búsqueda** parcial **, Ignorar caso** está seleccionado de forma predeterminada.

[![](https://helpx.adobe.com/content/dam/help/en/experience-manager/brand-portal/images/see-the-guide.png)](../using/brand-portal-searching.md#facetedsearchbyapplyingfilterstosearch)

## ¿Qué ha cambiado en 6.4.3? {#what-changed-in}

Brand Portal 6.4.3 se centra en— proporcionar a organizaciones un alias alternativo además de su ID de inquilino en la URL de acceso de Brand Portal, la nueva configuración de jerarquía de carpetas, mejoras en la compatibilidad con vídeo, publicación programada desde la instancia de AEM Author a Brand Portal, mejoras operativas— y atiende a solicitudes de clientes.

### Navegación por jerarquía de carpetas para usuarios que no son administradores

Ahora los administradores pueden configurar cómo se muestran las carpetas a usuarios no administradores (editores, usuarios invitados y usuarios invitados) al iniciar sesión. [Habilite la configuración de jerarquía](../using/brand-portal-general-configuration.md) de carpetas en Configuración **general**, en el panel de herramientas de administración. Si la configuración es:

* **habilitada**, el árbol de carpetas que empieza desde la carpeta raíz es visible para usuarios no administradores. De este modo, se les otorga una experiencia de navegación similar a la de los administradores.
* **desactivadas**, solo se muestran las carpetas compartidas en la página de aterrizaje.

![](assets/enable-folder-hierarchy.png)**El caso de uso**

La funcionalidad [Habilitar jerarquía](../using/brand-portal-general-configuration.md) de carpetas (cuando está habilitada) le ayuda a diferenciar las carpetas con los mismos nombres compartidos de jerarquías diferentes. Al iniciar sesión, los usuarios no administradores ven las carpetas principales (y antecesoras) virtuales de las carpetas compartidas.![](assets/disabled-folder-hierarchy1-2.png)![](assets/enabled-hierarchy1-2.png)
 

Las carpetas compartidas se organizan dentro de los directorios respectivos de carpetas virtuales. Puede reconocer estas carpetas virtuales con un icono de candado.

Tenga en cuenta que la miniatura predeterminada de las carpetas virtuales es la imagen en miniatura de la primera carpeta compartida.

![](assets/hierarchy1-nonadmin-2.png)

[![](https://helpx.adobe.com/content/dam/help/en/experience-manager/brand-portal/images/see-the-guide.png)](../using/brand-portal-general-configuration.md)

### Buscar en una ruta o una ruta de carpeta específica

**Predicado de explorador** de rutas se introduce en el formulario de búsqueda para permitir la búsqueda de recursos en un directorio específico. La ruta de búsqueda predeterminada de predicado de búsqueda para el navegador de rutas es */content/dam/mac/ &lt; id-id &gt;/*, que se puede configurar editando el formulario de búsqueda predeterminado.

* Los usuarios administradores pueden utilizar el navegador de rutas para navegar a cualquier directorio de carpetas en Brand Portal.
* Los usuarios no administradores pueden utilizar el navegador de rutas para navegar únicamente a las carpetas (y volver a las carpetas principales) compartidas con ellos.
Por ejemplo, */content/dam/mac/ &lt; tenant-id &gt;/foldera/folderb/folderc* se comparte con un usuario no administrador. El usuario puede buscar recursos dentro de folderc mediante el navegador de rutas. Este usuario también puede navegar a folderb y a foldera (ya que son antecesores de folderc que se comparten con el usuario).

![](assets/edit-search-form.png)

**El caso de uso**

Ahora puede restringir la búsqueda de recursos dentro de una carpeta específica a la que ha navegado, en lugar de comenzar en la carpeta raíz.

Tenga en cuenta que la búsqueda bajo estas carpetas devuelve resultados únicamente de los recursos que se han compartido con el usuario.

![](assets/filter-panel.png)

[![](https://helpx.adobe.com/content/dam/help/en/experience-manager/brand-portal/images/see-the-guide.png)](../using/brand-portal-search-facets.md#listofsearchpredicates)

### Compatibilidad con representaciones de vídeo de Dynamic Media

Los usuarios cuya instancia de AEM Author se encuentra en el modo híbrido Dynamic Media pueden obtener una vista previa y descargar las representaciones de Dynamic Media, además de los archivos de vídeo originales.

Para permitir la vista previa y la descarga de representaciones de medios dinámicos en cuentas de usuario específicas, los administradores deben especificar **la Configuración de Dynamic Media** (URL de servicio de vídeo (URL-Gateway) y el ID de registro para recuperar el vídeo dinámico) en la configuración **de vídeo** desde el panel de herramientas de administración.

**El caso**
de uso de los vídeos de Dynamic Media se puede previsualizar en:

* Página de detalles del recurso
* Vista de tarjeta del recurso
* Página de vista previa del vínculo compartido

Las codificaciones de vídeo de Dynamic Media se pueden descargar de:

* Portal de marca
* Vínculo compartido

![](assets/edit-dynamic-media-config.png)

[![](https://helpx.adobe.com/content/dam/help/en/experience-manager/brand-portal/images/see-the-guide.png)](../using/brand-portal.md#tenantaliasforportalurl)

### Publicación programada en Brand Portal

Los recursos (y carpetas) de publicación de [AEM (6.4.2.0) de](https://helpx.adobe.com/experience-manager/6-4/release-notes/sp-release-notes.html#main-pars_header_9658011) creación de instancias a Brand Portal se pueden programar para una fecha y hora posteriores.

Del mismo modo, los recursos publicados pueden eliminarse del portal más adelante (hora), mediante la programación del flujo de trabajo Cancelar publicación del portal de marca.

![](assets/schedule-publish.png)
![](assets/publishlater-workflow.png)

[![](https://helpx.adobe.com/content/dam/help/en/experience-manager/brand-portal/images/see-the-guide.png)](../using/brand-portal.md#tenantaliasforportalurl)

### Alias de inquilino configurable en URL

Las organizaciones pueden obtener su URL de portal personalizada, con un prefijo alternativo en la URL. Para obtener un alias para el nombre del inquilino en su URL de portal existente, las organizaciones deben ponerse en contacto con la asistencia de Adobe.

Tenga en cuenta que solo se puede personalizar el prefijo de la URL de Brand Portal y no toda la dirección URL.\
Por ejemplo, una organización con dominio existente **geomettrix.brand-portal.adobe.com** puede obtener **geomettrixinc.brand-portal.adobe.com** creado on request.

Sin embargo, la instancia de AEM Author solo se puede [configurar](https://helpx.adobe.com/experience-manager/6-5/assets/using/brand-portal-configuring-integration.html) con la URL de ID de inquilino y no con la URL (alternativa) del alias del inquilino.

**El caso
de uso** Organizaciones puede satisfacer sus necesidades de marca mediante la personalización de la dirección URL del portal, en lugar de mantenerse atascada a la dirección URL proporcionada por Adobe.

[![](https://helpx.adobe.com/content/dam/help/en/experience-manager/brand-portal/images/see-the-guide.png)](../using/brand-portal.md#tenantaliasforportalurl)

### Descargar mejoras de experiencia

La versión ofrece una experiencia de descarga simplificada con un número reducido de clics y advertencias, en:

* para descargar solo las representaciones (y no los recursos originales).
* descargar los recursos cuando se restringe el acceso a las representaciones originales.

## ¿Qué ha cambiado en 6.4.2? {#what-changed-in-1}

Brand Portal 6.4.2 incorpora una serie de capacidades para tratar las necesidades de distribución de recursos de las organizaciones y ayudarle a llegar a un gran número de usuarios distribuidos globalmente mediante el acceso de invitado y la óptima experiencia con descargas aceleradas. Brand Portal también proporciona un mayor control a las organizaciones mediante nuevas configuraciones para administradores, informes recién añadidos y catálogos a solicitudes de clientes.

### Acceso de invitados

![](assets/bp-login-screen-1.png)

Portal de marca AEM permite el acceso de los invitados al portal. Un usuario invitado no necesita credenciales para ingresar al portal y puede acceder y descargar todas las carpetas y colecciones públicas. Los usuarios invitados pueden agregar recursos a su lightbox (colección privada) y descargarlos. También pueden ver la búsqueda de etiquetas inteligentes y los predicados de búsqueda establecidos por los administradores. La sesión de invitado no permite a los usuarios crear colecciones ni guardarlas ni compartirlas, acceder a la configuración de carpetas y colecciones ni compartir recursos como vínculos.

En una organización, se permiten varias sesiones de invitados simultáneas, que se limitan al 10% de la cuota total de usuarios por organización.

Una sesión de invitado permanece activa durante dos horas. Por lo tanto, el estado de la caja de luz también se conserva hasta dos horas desde la hora de inicio de la sesión. Después de dos horas, la sesión del invitado tiene que reiniciarse, por lo que se pierde el estado de la caja de iluminación.

### Descargas aceleradas

Los usuarios de Brand Portal pueden aprovechar las descargas rápidas de IBM Aspera Connect para obtener velocidades de hasta 25 veces más rápido y disfrutar de una experiencia de descarga perfecta independientemente de su ubicación en todo el mundo. Para descargar los recursos más rápidamente desde Brand Portal o el vínculo compartido, los usuarios deben seleccionar **la opción Activar aceleración** de descarga en el cuadro de diálogo de descarga, siempre que la aceleración de descarga esté habilitada en su organización.

![](assets/donload-assets-dialog-2.png)

Para habilitar la descarga acelerada basada en IBM Aspera para la organización, los administradores **habilitan** la opción Activar aceleración de descarga (que está deshabilitada de forma predeterminada) desde [Configuración general](brand-portal-general-configuration.md#allow-download-acceleration) en el panel de herramientas administrativas. Para obtener más información sobre los requisitos previos y los pasos para la resolución de problemas de descarga más rápida de Brand Portal y los vínculos compartidos, consulte [Guía para acelerar las descargas desde Brand Portal](../using/accelerated-download.md#main-pars-header).

### Informe Inicios de sesión de usuarios

Se ha introducido un nuevo informe para rastrear inicios de sesión de usuario. El informe Inicios **de sesión** de usuario puede ser de utilidad para permitir a las organizaciones auditar y llevar una comprobación a los administradores delegados y a otros usuarios de Brand Portal.

Los registros de informes muestran nombres, ID de correo electrónico, personas (administrador, visor, editor, invitado), grupos, último inicio de sesión, estado de actividad e inicio de sesión de cada usuario desde la implementación de Brand Portal 6.4.2 hasta el momento de generación de informes. Los administradores pueden exportar el informe como. csv. Junto con otros informes, los informes Inicios de sesión de usuario permiten a las organizaciones monitorear más estrechamente las interacciones de los usuarios con los recursos de marca aprobados, garantizando así la conformidad con las oficinas de cumplimiento corporativas.

![](assets/user-logins-1.png)

### Acceso a representaciones originales

Los administradores pueden restringir el acceso de los usuarios a los archivos de imagen originales (.jpeg. tiff. png. bmp. gif. pjpeg, x-portable-anymap, x-portable-anymap, x-portable-de-mapmap, x-portátil, x-xbitmap, x-xpixmap, x-xpixmap, x-xpixmap, x-xpixmap, x-xpixmap, x-xpixmap, x-xpixmap, x-xpixmap, x-xpixmap, x-xpixmap, x-xpixmap, x-xpixmap, x-xpixmap, x-xpixmap, x-xpixmap, x-xpixmap, x-xpixmap, x-xpixmap, x-xpixmap, x-xpixmap, x-xpixmap, x-xpixmap, x-xpixmap, x-xpixmap, x-xpixmap, x-xpixmap, x-xpixmap, x-xpixmap, x-xpixmap, x-x@-@ icono, image/photoshop, image/x-photoshop. psd, image/vnd. adobe. photoshop) y proporcionan acceso a las representaciones de baja resolución que descargan de Brand Portal o del vínculo compartido. Este acceso se puede controlar en el nivel de grupo de usuarios desde la ficha Grupos de la página Funciones de usuario en el panel Herramientas de administración.

![](assets/access-original-rend-1.png)

* De forma predeterminada, todos los usuarios pueden descargar representaciones originales, ya que el acceso al original está habilitado para todos.
* Los administradores deben anular la selección de las casillas correspondientes para evitar que un grupo de usuarios acceda a representaciones originales.
* Si un usuario es miembro de varios grupos, pero sólo uno de los grupos tiene restricciones, las restricciones se aplican a ese usuario.
* Las restricciones no se aplican a los administradores, aunque sean miembros de grupos restringidos.
* Los permisos del usuario que comparte recursos como vínculo se aplican a los usuarios que descargan recursos mediante vínculos compartidos.

### Ruta de jerarquía de carpetas en las vistas de tarjeta y lista

Las tarjetas de carpetas, en Vista de tarjeta, ahora muestran información de jerarquía de carpetas para usuarios no administradores (Editor, Visor y Usuario invitado). Esta funcionalidad permite que los usuarios conozcan la ubicación de las carpetas, en relación con la jerarquía principal.

La información de jerarquía de carpetas es especialmente útil para diferenciar las carpetas con nombres similares a otras carpetas compartidas desde una jerarquía de carpetas diferente. Si los usuarios no administradores no conocen la estructura de carpetas de los recursos compartidos, los recursos /folders con nombres similares parecen confusos.

* Las rutas mostradas en las tarjetas respectivas se truncan para ajustarse a los tamaños de la tarjeta. Sin embargo, los usuarios pueden ver la ruta completa como información sobre herramientas al pasar el ratón por encima de la ruta truncada.

![](assets/folder-hierarchy1-1.png)

Vista de lista muestra la ruta de carpeta de los recursos de una columna a todos los usuarios de Brand Portal.

![](assets/list-view-1.png)

### Opción de información general para ver propiedades de recursos

Brand Portal proporciona la opción Información general a usuarios no administradores (editores, usuarios invitados, usuarios invitados) para ver propiedades de recursos de carpetas o recursos seleccionados. La opción Información general está visible:

1. En la barra de herramientas situada en la parte superior de la selección de un recurso o carpeta.
2. En la lista desplegable de selección del Selector de raíl.

Al seleccionar la opción Información general mientras se selecciona un recurso o carpeta, los usuarios pueden ver el título, la ruta y la hora de creación de recursos. En cambio, en la página de detalles del recurso, la opción Información general permite que los usuarios vean metadatos del recurso.

![](assets/overview-option-2.png)

![](assets/overview-rail-selector-2.png)

## Nuevas configuraciones

Se agregan seis nuevas configuraciones para que los administradores habiliten/deshabiliten las siguientes funcionalidades en inquilinos específicos:

* Permitir el acceso de invitados
* Permitir que los usuarios soliciten acceso a Brand Portal
* Permitir que los administradores eliminen recursos de Brand Portal
* Permitir la creación de colecciones públicas
* Permitir la creación de colecciones inteligentes públicas
* Permitir aceleración de descarga

Las configuraciones anteriores están disponibles en Acceso y Configuración general en el panel Herramientas administrativas.

![](assets/access-configs-1.png)
![](assets/general-configs-1.png)
![](assets/admin-tools-panel-13.png)

### Interfaz de usuario de Adobe. io para configurar integraciones oauth

A partir de Brand Portal 6.4.2, se utiliza la interfaz Adobe. io [https://legacy-oauth.cloud.adobe.io/](https://legacy-oauth.cloud.adobe.io/) para crear aplicaciones JWT, lo que permite configurar integraciones oauth para permitir la integración de AEM Assets con Brand Portal. Anteriormente, la interfaz de usuario para configurar las integraciones de oauth se alojaba en [https://marketing.adobe.com/developer/](https://marketing.adobe.com/developer/). Para obtener más información sobre la integración de Recursos AEM con Brand Portal para publicar recursos y colecciones en Brand Portal, consulte [Configurar la integración de AEM Assets con Brand Portal](https://helpx.adobe.com/in/experience-manager/6-4/assets/using/brand-portal-configuring-integration.html).

## Mejoras de búsqueda

Los administradores pueden hacer que la propiedad predica sin distinción de mayúsculas y minúsculas mediante el predicado de propiedad actualizado, que tiene una comprobación de Ignorar caso. Esta opción está disponible para predicado de propiedad de predicado de propiedad y de varios valores.\
Sin embargo, la búsqueda sin distinción de mayúsculas y minúsculas es comparativamente más lenta que la búsqueda predeterminada de predicado de propiedad. Si hay demasiados predicados que no distinguen mayúsculas y minúsculas en el filtro de búsqueda, la búsqueda puede ralentizarse. Por lo tanto, es aconsejable utilizar la búsqueda sin distinción de mayúsculas y minúsculas.

## Qué cambió en 6.4.1 {#what-changed-in-2}

Brand Portal 6.4.1 es una versión de actualización de plataforma que incorpora varias funciones nuevas y mejoras esenciales como las mejoras de navegación, búsqueda y rendimiento para ofrecer experiencias de cliente que cumplen con los requisitos.

### Mejoras de exploración

* Nuevo carril de árbol de contenido para navegar rápidamente por una jerarquía de recursos.

![](assets/contenttree-2.png)

* Se han introducido nuevos métodos abreviados de teclado, por ejemplo _(p)_ para la navegación a páginas de propiedades, _(e)_ para Editar y _(ctrl + c)_ para operaciones de copia.
* Se ha mejorado el desplazamiento y la experiencia de carga diferida en la vista de tarjeta y de lista para examinar un gran número de recursos.
* Vista de tarjeta mejorada con compatibilidad con tarjetas de distintos tamaños según la configuración de la vista.

![](assets/cardviewsettings-1.png)

* La vista de tarjeta ahora muestra la marca de fecha y hora al pasar el ratón por encima de la etiqueta de fecha.

* Vista de columna mejorada con **Más detalles** en la instantánea de recursos, que le permite desplazarse a la página de detalles de un recurso.

![](assets/columnmoredetail.png)

* La vista de lista muestra ahora los nombres de archivo de los recursos en la primera columna de forma predeterminada, además de la configuración regional, el tipo de recurso, las dimensiones, el tamaño, la clasificación y la información de publicación. La nueva **configuración** de vista se puede utilizar para configurar la cantidad de detalle que se mostrará en la vista de lista.

* Se ha mejorado la experiencia de detalles del recurso con capacidad para desplazarse hacia delante y hacia atrás entre los recursos utilizando nuevos botones de navegación y ver el recuento de recursos.

![](assets/navbtn.png)

* Nueva capacidad para obtener una vista previa de los archivos de audio, cargados desde AEM, en la página de detalles del recurso.
* Nueva funcionalidad Recursos relacionados proporcionada en las propiedades de Recursos. Los recursos relacionados con otros recursos fuente/derivados en AEM y publicados en Brand Portal ahora tienen su relación intacta en Brand Portal, con vínculos a los activos relacionados en la página de propiedades.
* Se ha introducido una nueva configuración para restringir la creación de colecciones públicas a los usuarios no administradores. Las organizaciones pueden trabajar con el equipo de asistencia de Adobe para configurar esta capacidad en cuentas específicas.

### Mejoras de búsqueda

* Capacidad introducida para volver a la misma posición en los resultados de búsqueda, después de navegar a un elemento de búsqueda, sin volver a ejecutar la consulta de búsqueda.
* Se ha proporcionado un nuevo recuento de resultados de búsqueda para mostrar el número de resultados de búsqueda.
* Se ha mejorado el filtro de búsqueda de tipo de archivo con la capacidad de filtrar los resultados de búsqueda según tipos MIME detallados como.jpg. png y. psd comparados con las versiones anteriores, Documentos y Multimedia.
* Filtros de búsqueda mejorados para colecciones, con marcas de hora precisas en lugar de la funcionalidad del deslizador de tiempo anterior.
* Se han introducido nuevos filtros de tipo de acceso para buscar las colecciones públicas o no públicas.

![](assets/accesstypefilter.png)

### Optimizaciones de descarga

* Un solo archivo grande se descarga directamente, sin la creación del archivo zip, mejorando así la velocidad y el rendimiento.
* El límite de descarga Zip para la función de compartir vínculos ha aumentado a 5 GB, desde 1 GB.

* Ahora los usuarios pueden descargar solo los archivos originales y los originales, así como evitar las representaciones integradas, al descargar recursos de Brand Portal o a través de la función de vínculos compartidos.

![](assets/excludeautorendition.png)

### Mejoras de rendimiento

* Mejora hasta el 100% en la velocidad de descarga de recursos.
* Mejora hasta un 40% en la respuesta de búsqueda de recursos.
* Mejora hasta un 40% en el rendimiento de navegación.

**Nota**: Las mejoras mencionadas son según las pruebas realizadas en el laboratorio.

### Capacidades mejoradas de generación de informes

**Se ha introducido un informe**
de uso compartido de vínculos nuevo para proporcionar información sobre los vínculos compartidos. El informe Compartir vínculos enumera todas las URL, a los recursos, compartidas con usuarios internos y externos en toda la organización en el intervalo de tiempo especificado. También informa cuándo se compartió el vínculo, quién y cuándo caduca.

![](assets/navigatereport.png)

**Se modificó el punto de entrada para acceder al informe**Uso del informe
Uso ahora se consolidan con otros informes y ahora se pueden ver desde la consola Informes de recursos. Para acceder a la consola Informes de recursos, vaya a **Crear/Administrar informes** desde el panel Herramientas administrativas.

![](assets/accessassetreport.png)

**Una experiencia de usuario mejorada con la**interfaz de informes de informes
en Brand Portal es más intuitiva e incluye mayor control para las organizaciones. Además de crear varios informes, los administradores ahora pueden volver a visitar los informes generados y descargarlos o eliminarlos, ya que estos informes se guardan en Brand Portal.

Cada uno de los informes que se crean puede personalizarse añadiendo o quitando columnas predeterminadas. Además, se pueden agregar columnas personalizadas a los informes de descarga, caducidad y publicación para controlar su grado de granularidad.

### Herramientas de administración mejoradas

Se ha mejorado el selector de propiedades en las herramientas de administración para metadatos, búsquedas e informes con Tipo-ahead y capacidad de exploración para simplificar la experiencia de administración.

### Otras mejoras

* Los recursos publicados en Brand Portal desde AEM 6.3.2.1 y 6.4 ahora pueden estar disponibles públicamente para usuarios generales de Brand Portal, marcando la casilla de verificación Publicación pública en el cuadro de diálogo de replicación de AEM Assets Brand Portal.

![](assets/public-folder-publish.png)

* Los administradores reciben notificaciones a través de los correos electrónicos de solicitud de acceso, aparte de las notificaciones en el área de notificación de Brand Portal, si alguien ha solicitado acceso al portal de marca.

## ¿Qué ha cambiado en 6.3.2? {#what-changed-in-3}

Brand Portal 6.3.2 incluye funcionalidad nueva y mejorada orientada a las principales solicitudes de los clientes y mejoras generales de rendimiento.

### Solicitar acceso a Brand Portal {#request-access-to-brand-portal}

Ahora los usuarios pueden solicitar acceso a Brand Portal con la nueva función**** need access available on the login screen of Brand Portal.

![](assets/bplogin_request_access.png)

Según si los usuarios tienen un Adobe ID o necesitan crear un Adobe ID, los usuarios pueden seguir el flujo de trabajo adecuado para enviar una solicitud. Los administradores de productos de Brand Portal reciben estas solicitudes en su área de notificación y otorgan acceso a través de Admin Console de Adobe.

Para obtener más información, consulte [Solicitar acceso a Brand Portal](../using/brand-portal.md#requestaccesstobrandportal).

### Mejora en el informe descargado de recursos {#enhancement-in-the-assets-downloaded-report}

El informe descargado de recursos ahora incluye el recuento de descargas de recursos por usuario dentro de la fecha y el intervalo de tiempo especificados. Los usuarios pueden descargar este informe en formato. csv y compilar datos como el recuento total de descargas de un recurso con licencia.

![](assets/reports_download_downloaded_by.png)

Para obtener más información, consulte los pasos 3 y 6 en [Crear y administrar informes adicionales](../using/brand-portal-reports.md#createandmanageadditionalreports).

### Notificación de mantenimiento de Brand Portal {#brand-portal-maintenance-notification}

Brand Portal ahora muestra una pancarta de notificación unos días antes de la próxima actividad de mantenimiento. Una notificación de muestra:

![](assets/bp_maintenance_notification-1.png)

Para obtener más información, consulte [Notificación de mantenimiento de Brand Portal](https://helpx.adobe.com/experience-manager/brand-portal/using/brand-portal.html#BrandPortalmaintenancenotification).

### Mejora de los recursos con licencia compartidos mediante la función de compartir vínculos {#enhancement-for-licensed-assets-shared-using-the-link-share-feature}

Al descargar recursos con licencia mediante la función de compartir vínculos, ahora se le solicita que acepte el acuerdo de licencia de esos recursos.

![](assets/copyright_management.png)

Para obtener más información, consulte el paso 12 en [Compartir recursos como vínculo](../using/brand-portal-link-share.md#shareassetsasalink).

### Mejora del selector de usuarios {#user-picker-enhancement}

El rendimiento del selector de usuarios ahora se ha mejorado para adaptarse a las necesidades de los clientes con una gran base de usuarios.

### Cambios en la marca de Experience Cloud {#experience-cloud-branding-changes}

Brand Portal ahora sigue la nueva marca de Adobe Experience Cloud.

![](assets/bp_solution_switcher.png)

## Qué cambió en 6.3.1 {#what-changed-in-4}

Brand Portal 6.3.1 incluye funciones nuevas y mejoradas orientadas a alinear Brand Portal con AEM.

### Interfaz de usuario actualizada {#upgraded-user-interface}

Para alinear la experiencia del usuario de Brand Portal con AEM, Adobe está migrando a la interfaz de usuario de Coral 3. Este cambio mejora el uso general, incluso la navegación y la apariencia.

#### Experiencia de navegación mejorada {#enhanced-navigational-experience}

* Acceso rápido a herramientas administrativas a través del nuevo logotipo de Adobe:

![](assets/aemlogo-3.png)

* Navegación del producto mediante una superposición:

![](assets/overlay_navigation.png)

* Navegación rápida a carpetas principales:

![](assets/navigationparentfolders.png)

* Búsqueda rápida y navegación al contenido y las herramientas necesarios:

![](assets/omnisearchicon.png)

### Experiencia de navegación mejorada {#enhanced-browsing-experience}

* Nueva vista de columna para navegar por carpetas anidadas:

![](assets/millercolumnnavigation.png) ![](assets/multi-columnview.png)

* En la lista de recursos de una carpeta, el recurso más reciente se carga en la parte superior.

### Experiencia de búsqueda mejorada {#enhanced-search-experience}

* La nueva función de búsqueda Omni facilita el acceso rápido a contenido, capacidad o etiquetas relevantes mediante sugerencias automáticas a medida que escribe palabras clave de búsqueda. La búsqueda Omni está disponible en todas las funciones de búsqueda.

![](assets/omnisearch_whatsnew.png)

* También puede agregar filtros de búsqueda a la búsqueda Omni para reducir y acelerar la búsqueda.

![](assets/omnisearch_withfilters.png)

* La nueva búsqueda basada en clasificaciones de recursos permite buscar recursos con clasificaciones, si se publican desde Recursos AEM.
* La nueva función de búsqueda multivalor acepta varias palabras clave con el operador Y para descubrir recursos más rápidamente.
* La nueva función de ampliación de búsqueda permite mejorar la relevancia de búsqueda para que los recursos específicos aparezcan en la parte superior de los resultados de búsqueda.
* La nueva función de búsqueda basada en rutas le permite proporcionar la ruta a una carpeta anidada para poder buscar recursos en esa carpeta.

#### Nueva búsqueda inteligente basada en etiquetas {#new-smart-tags-based-search}

Si las imágenes con etiquetas inteligentes se publican desde AEM Assets a Brand Portal, puede buscar estas imágenes en Brand Portal utilizando los nombres de etiquetas inteligentes como palabras clave de búsqueda. Esta función solo está disponible para archivos.

### Experiencia de descarga mejorada {#enhanced-downloading-experience}

Después de descargar una carpeta anidada, puede conservar la jerarquía original de carpetas. Los recursos dentro de una carpeta anidada se pueden descargar en una sola carpeta en oposición a carpetas independientes.

### Rendimiento mejorado {#improved-performance}

Las mejoras en las funciones de exploración, búsqueda y descarga mejoran significativamente el rendimiento de Brand Portal.

### Nueva administración de derechos digitales para recursos {#new-digital-rights-management-for-assets}

Los administradores pueden establecer la fecha y hora de caducidad de los recursos antes de compartirlos. Una vez que el recurso caduca, es visible para los editores y editores, pero no se puede descargar. Cuando caduca un recurso, los administradores reciben una notificación.

### Clasificación de recursos mejorada {#enhanced-asset-sorting}

La ordenación de recursos en una carpeta de la vista de lista ya no está restringida al número de recursos que se muestran en la primera página. Se ordenan todos los recursos de una carpeta, independientemente de si se enumeran o no en la primera página.

### Informes mejorados {#reporting-capabilities}

Los administradores pueden crear y administrar tres tipos de informes: recursos descargados, caducados y publicados. También hay disponible la capacidad para configurar las columnas en un informe y exportar los informes al formato CSV.

![](assets/newreport.png)

### Metadatos adicionales {#additional-metadata}

Brand Portal 6.3.1 presenta metadatos adicionales, que se encuentran a la par con AEM Assets 6.3. Puede utilizar el formulario Editor de esquemas para controlar los metadatos que deberían estar visibles en la página Propiedades de recursos. Los metadatos de los recursos no son visibles para los usuarios externos que comparten el vínculo, que solo pueden previsualizar y descargar recursos con la URL compartida del vínculo.

![](assets/additionsinmetadata.png)

### Capacidades adicionales para administradores {#additional-capabilities-for-administrators}

* Antes de finalizar las personalizaciones al papel tapiz de pantalla de inicio de sesión, los administradores pueden obtener una vista previa de los cambios.

![](assets/wallpaperpreview.png)

* Cuando un administrador agrega usuarios nuevos, no es necesario que acepte invitaciones para añadirlos a Brand Portal, sino que se agregan automáticamente.

### Nuevas funciones de publicación en AEM Assets 6.3 {#new-publishing-capabilities-in-aem-assets}

* Los administradores de AEM pueden publicar un esquema de metadatos de AEM Assets a Brand Portal con AEM 6.3 SP 1-CFP 1 (6.3.1.1), que estará disponible en el 4 de septiembre de 2017.

![](assets/publish_metadataschemaaemassets.png)

* Los administradores de AEM pueden publicar todas las etiquetas de AEM Assets en Brand Portal con AEM 6.2 SP 1-CFP 7 y AEM 6.3 SP 1-CFP 1 (6.3.1.1).

![](assets/publish_tags_aemassets.png)

* Desde Recursos AEM, puede publicar recursos y colecciones que tengan etiquetas, incluidas etiquetas inteligentes. A continuación, puede buscar estos recursos o colecciones utilizando estas etiquetas como palabras clave de búsqueda en Brand Portal.

## Frequently asked questions {#frequently-asked-questions}

**Qus. ¿Perderé acceso a cualquier recurso, característica o configuraciones que haya creado?****Ans.** Todas las características y configuraciones existentes permanecen intactas. Los usuarios finales no se ven afectados y su contenido permanece intacto.

**Noches. ¿Cuándo se desplaza a la nueva versión de Brand Portal?****Ans.** Brand Portal 6.4.4 se publicó en febrero de 2019. Se espera que la versión de Next Brand Portal se publique en el tercer trimestre de 2019.

>[!NOTE]
>
>La programación de versiones es tentativa y sujeta a cambios. Póngase en contacto con su administrador de cuentas de Adobe o con Asistencia al cliente para obtener el programa actualizado de lanzamiento.

**Noches. ¿Se verán afectados mis usuarios?****Ans.** Este cambio es exclusivamente dentro de Brand Portal, por lo que no afecta a los usuarios finales.

**Noches. ¿Se requiere alguna acción por mi parte?****Ans.** El administrador no requiere ninguna acción. Cuando obtenga acceso al nuevo portal de marca, consulte la documentación para ver todas las campanas y los silbidos.

**Noches. ¿Con quién puedo ponerme en contacto con preguntas?****Ans.** Póngase en contacto con su administrador de cuentas de Adobe o con Asistencia al cliente.
