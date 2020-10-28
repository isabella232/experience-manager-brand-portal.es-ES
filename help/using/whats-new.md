---
title: Novedades de AEM Assets Brand Portal
seo-title: Novedades de AEM Assets Brand Portal
description: Eche un vistazo a las nuevas funciones y mejoras de 2020.10.0.
seo-description: Eche un vistazo a las nuevas funciones y mejoras de 2020.10.0.
uuid: 2c59d738-9b53-4f25-a205-13bf75c80b77
products: SG_EXPERIENCEMANAGER/Brand_Portal
content-type: reference
contentOwner: Vishabh Gupta
topic-tags: introduction
discoiquuid: fec32ca3-142b-4a11-9b92-5113fc27277a
translation-type: tm+mt
source-git-commit: 1d57e3ec19f1ffc944e2547989b2627988cd19c1
workflow-type: tm+mt
source-wordcount: '5479'
ht-degree: 1%

---


# Novedades de AEM Assets Brand Portal {#what-s-new-in-aem-assets-brand-portal}

Adobe Experience Manager (AEM) Assets Brand Portal le ayuda a adquirir, controlar y distribuir de forma segura recursos creativos aprobados a partes externas y usuarios empresariales internos entre dispositivos. Ayuda a mejorar la eficiencia del uso compartido de activos, acelera el tiempo de comercialización de los activos y reduce el riesgo de incumplimiento y acceso no autorizado. Adobe está trabajando para mejorar la experiencia general de Brand Portal. A continuación, podrá echar un vistazo a las nuevas funciones y mejoras.

## Qué cambió en 2020.10.0 {#what-changed-in-oct-2020}

Brand Portal 2020.10.0 es una versión mejorada que se centra en simplificar la experiencia de descarga de recursos e incluye correcciones críticas. La mejora incluye un flujo de trabajo nuevo y mejorado para la descarga de recursos, opciones adicionales para excluir representaciones, descarga directa desde el panel **[!UICONTROL Representaciones]** , configuración para permitir derechos de acceso y descarga para grupos específicos de usuarios, y navegación sencilla hacia los archivos, colecciones y vínculos compartidos desde todas las páginas de Brand Portal. Consulte las últimas notas de la versión [de Brand Portal](brand-portal-release-notes.md).


### Experiencia de descarga simplificada {#download-dialog}

Anteriormente, el cuadro de diálogo **[!UICONTROL Descargar]** aparecía con varias opciones, como crear una carpeta independiente para cada recurso, enviar un recurso por correo electrónico, seleccionar el recurso original, las representaciones personalizadas, las representaciones dinámicas, excluir las representaciones del sistema y habilitar la aceleración de la descarga, que eran ambiguas para los usuarios nuevos o no técnicos, especialmente cuando se seleccionaban varios recursos o carpetas para la descarga. Además, el usuario no pudo ver todas las representaciones de recursos ni excluir una representación personalizada o dinámica específica.

El nuevo cuadro de diálogo **[!UICONTROL Descargar]** generaliza el proceso de selección y filtrado de recursos, lo que facilita a los usuarios de Brand Portal la toma de decisiones eficaces mientras descargan las representaciones de recursos. Lista todos los recursos seleccionados y sus representaciones en función de la configuración de [**[!UICONTROL descarga]**](brand-portal-download-assets.md) y la configuración de **[!UICONTROL descarga]** .

>[!NOTE]
>
>Ahora todos los usuarios tendrán habilitada la descarga **** rápida de forma predeterminada y requiere que [IBM Aspera Connect 3.9.9](https://www.ibm.com/support/knowledgecenter/SSXMX3_3.9.9/kc/connect_welcome.html) esté instalada en la extensión de su explorador antes de descargar los recursos de Brand Portal.

<!--
If any of the **[!UICONTROL Custom Rendition]** or **[!UICONTROL System Rendition]** is enabled in the [**[!UICONTROL Download]**](brand-portal-download-assets.md) configuration and **[!UICONTROL Download]** settings are enabled for the group users, the new **[!UICONTROL Download]** dialog appears with all the renditions of the selected assets or folders containing assets in a list view. 
-->

En el cuadro de diálogo **[!UICONTROL Descargar]** , los usuarios pueden:

* Vista todas las representaciones disponibles de cualquier recurso en la lista de descarga.
* Excluya las representaciones de los recursos que no sean necesarias para la descarga.
* Aplique el mismo conjunto de representaciones a todos los tipos de recursos similares con un solo clic.
* Aplique un conjunto diferente de representaciones para distintos tipos de recursos.
* Crear una carpeta independiente para cada recurso.
* Descargue los recursos seleccionados y sus representaciones.

El flujo de trabajo de descarga se mantiene constante para los recursos independientes, varios recursos, carpetas que contienen recursos, recursos con licencia o sin licencia y la descarga de recursos mediante el vínculo compartido. Consulte [los pasos para descargar recursos desde Brand Portal](https://docs.adobe.com/content/help/en/experience-manager-brand-portal/using/download/brand-portal-download-assets.html#download-assets).

![download-dialog](assets/download-dialog-box.png)

### Navegación rápida  {#quick-navigation}

Anteriormente, la opción de vista de **[!UICONTROL archivos]**, **[!UICONTROL colecciones]** y vínculos **** compartidos estaba oculta y requería varios clics cada vez que el usuario deseaba cambiar a otra vista.

En Brand Portal 2020.10.0, los usuarios pueden navegar a **[!UICONTROL Archivos]**, **[!UICONTROL colecciones]** y vínculos **** compartidos desde todas las páginas de Brand Portal con un solo clic mediante los vínculos de navegación rápida.

![collection-navigation](assets/collection-navigation.png)

### Panel de representación mejorado {#rendition-panel}

Anteriormente, los usuarios solo podían realizar la vista del recurso original y sus representaciones en el panel **[!UICONTROL Representaciones]** si alguna de las representaciones **** personalizadas o **[!UICONTROL del sistema]** estaba habilitada en la configuración de **[!UICONTROL descarga]** . Además, los usuarios tuvieron que descargar todas las representaciones de recursos, ya que no había ningún filtro para excluir representaciones personalizadas o dinámicas específicas que no eran necesarias.

<!--
Earlier, if any of the custom or system renditions was enabled in the **[!UICONTROL Download]** settings, an additional **[!UICONTROL Download]** dialog appeared on clicking the **[!UICONTROL Download]** button wherein the user had to manually select the set of renditions (original asset, custom renditions, dynamic renditions) to download.
There was no filter to exclude specific custom or dynamic renditions which were not required for download.
-->

En Brand Portal 2020.10.0, los usuarios pueden excluir representaciones específicas y [descargar directamente las representaciones seleccionadas del panel](brand-portal-download-assets.md#download-assets-from-asset-details-page) Representaciones de la página de detalles de recursos sin tener que abrir el cuadro de diálogo **[!UICONTROL Descargar]** .


<!-- 
In Brand Portal 2020.10.0, direct download and exclude renditions features are introduced in the **[!UICONTROL Renditions]** panel on the asset details page. All the renditions (original asset, custom renditions, dynamic renditions) under the rendition panel are now associated with a check box and are enabled by default. 

The user can clear the check boxes to exclude the renditions which are not required for download. And can click on the **[!UICONTROL Download]** button in the **[!UICONTROL Renditions]** panel to directly download the selected set of renditions in a zip folder without having to open the **[!UICONTROL Download]** dialog.
-->

![renditions-panel](assets/renditions-panel.png)


### Configurar permisos de descarga {#download-permissions}

Además de las configuraciones de **[!UICONTROL descarga]** existentes, los administradores de Brand Portal también pueden configurar permisos para que distintos grupos de usuarios realicen vistas y (o) descarguen el recurso original y sus representaciones desde la página de detalles del recurso.

Inicie sesión como administrador en el inquilino de Brand Portal y vaya a **[!UICONTROL Herramientas]** > **[!UICONTROL Usuarios]**.

En la página Funciones **[!UICONTROL de]** usuario, vaya a la ficha **[!UICONTROL Grupos]** para configurar la vista y (o) los permisos de descarga para los grupos de usuarios

Anteriormente, la configuración solo estaba disponible para evitar que los usuarios del grupo descargaran el recurso original.

La ficha **[!UICONTROL Grupos]** de la página Funciones **[!UICONTROL de]** usuario permite a los administradores configurar las opciones de vista y descarga:

* Si están activadas las opciones **[!UICONTROL Descargar representaciones originales]** y **[!UICONTROL Descargar representaciones]** , los usuarios del grupo seleccionado pueden realizar vistas y descargar los recursos originales y sus representaciones.
* Si ambas opciones de configuración están desactivadas, los usuarios solo pueden realizar la vista de los recursos originales. Las representaciones de recursos no son visibles para los usuarios en la página de detalles de recursos.
* Si solo está activada la opción **[!UICONTROL Descargar original]** , los usuarios pueden realizar la vista y descargar solo los recursos originales desde la página de detalles del recurso.
* Si solo está activada la opción **[!UICONTROL Descargar representaciones]** , los usuarios pueden realizar la vista del recurso original pero no pueden descargarlo. Sin embargo, el usuario puede realizar vistas y descargar las representaciones de recursos.

Consulte [Configuración de la descarga](https://docs.adobe.com/content/help/en/experience-manager-brand-portal/using/download/brand-portal-download-assets.html#configure-download-permissions)de recursos.

![vista-descarga-permiso](assets/download-permissions.png)

>[!NOTE]
>
>Si se agrega un usuario a varios grupos y uno de ellos tiene restricciones, las restricciones se aplicarán al usuario.


<!--
>Restrictions to access the original asset and their renditions do not apply to administrators even if they are members of restricted groups.
 >
 >The users can always download assets and their renditions from the repository using a `curl` request even if the download configurations are turned-off.
 >
-->

## Qué cambió en 6.4.7 {#what-changed-in-647}

La versión 6.4.7 de Brand Portal incorpora el visor de Documento, mejora la experiencia de descarga de recursos e incluye correcciones importantes. Consulte las últimas notas de la versión [de Brand Portal](brand-portal-release-notes.md).

<!--
Brand Portal 6.4.7 release brings in the Document Viewer, leverages the Brand Portal administrators to configure asset download, and centers top customer requests. See latest [Brand Portal Release Notes](brand-portal-release-notes.md).
-->

### Visor de documento {#doc-viewer}

El visor de Documento mejora la visualización de archivos PDF. Proporciona una experiencia similar a la de Adobe Document Cloud mientras ve los archivos PDF en Brand Portal.

Anteriormente, había disponibles opciones limitadas para la vista de los archivos PDF.

Con el visor de Documento, los usuarios de Brand Portal ahora tienen las opciones de vista de páginas, marcadores de vista, búsqueda de texto en la página, acercamiento, alejamiento, navegación a páginas anteriores y siguientes, cambio a página, ajuste a la ventana, ajuste a la pantalla y oculte o muestre la barra de herramientas.

>[!NOTE]
>
>La experiencia de visualización de otros formatos de documentos permanece sin cambios.


![](assets/doc-viewer.png)

### Descargar experiencia {#download-configurations}

El proceso de descarga de recursos se ha rediseñado, lo que ofrece una experiencia de usuario simplificada al [descargar recursos de Brand Portal](brand-portal-download-assets.md).

El flujo de trabajo existente de descarga de recursos de Brand Portal va seguido inevitablemente de la aparición de un cuadro de diálogo de **[!UICONTROL descarga]** con varias opciones de descarga entre las que elegir.

En Brand Portal 6.4.7, los administradores de Brand Portal pueden configurar la configuración de **[!UICONTROL descarga]** de recursos. Las configuraciones disponibles son:
* **[!UICONTROL Descarga rápida]**
* **[!UICONTROL Representaciones personalizadas]**
* **[!UICONTROL Representaciones del sistema]**

El administrador de Brand Portal puede habilitar cualquier combinación para configurar la descarga de recursos.

<!--In Brand Portal 6.4.7, fast download, custom renditions, and system renditions are the three configurations available.-->

* Si se desactivan tanto las representaciones **** personalizadas como las representaciones **[!UICONTROL del sistema]** , las representaciones originales de los recursos se descargan sin ningún cuadro de diálogo adicional que simplifique la experiencia de descarga para los usuarios de Brand Portal.

* Si se ha habilitado cualquiera de las representaciones **** personalizadas o **[!UICONTROL del sistema]** , aparece el cuadro de diálogo **[!UICONTROL Descargar]** y se descarga el recurso original junto con las representaciones de recursos. La activación de la configuración de descarga **** rápida acelera el proceso de descarga.

En función de la configuración, el flujo de trabajo de descarga permanece constante para los recursos independientes, varios recursos, carpetas que contienen recursos, recursos con licencia o sin licencia, y la descarga de recursos mediante un vínculo compartido.

![](assets/download-configuration.png)


## Qué cambió en 6.4.6 {#what-changed-in-646}

En Brand Portal 6.4.6, se cambia el canal de autorización entre AEM Assets y Brand Portal. Brand Portal ahora es compatible con AEM Assets como Cloud Service, AEM Assets 6.3 y versiones posteriores. En AEM Assets 6.3 y versiones posteriores, Brand Portal se configuró anteriormente en la IU clásica mediante OAuth Gateway heredado, que utiliza el intercambio de tokens JWT para obtener un Token de acceso IMS para la autorización. AEM Assets ahora se configura con Brand Portal a través de Adobe Developer Console, que proporciona un distintivo IMS para la autorización del inquilino de Brand Portal.

<!-- The steps to configure integration are different depending on your AEM version, and whether you are configuring for the first-time, or upgrading the existing integration:
-->

<!--
  
   | **AEM Version** |**New Integration** |**Upgrade Integration** |
|---|---|---|
| **AEM 6.5** |[Create new integration](../using/brand-portal-configure-integration-65.md) |[Upgrade existing integration](../using/brand-portal-configure-integration-65.md#upgrade-integration-65) | 
| **AEM 6.4** |[Create new integration](../using/brand-portal-configure-integration-64.md) |[Upgrade existing integration](../using/brand-portal-configure-integration-64.md#upgrade-integration-64) | 
| **AEM 6.3** |[Create new integration](../using/brand-portal-configure-integration-63.md) |[Upgrade existing integration](../using/brand-portal-configure-integration-63.md#upgrade-integration-63) | 
| **AEM 6.2** |Contact Support |Contact Support | 

   -->

Los pasos para configurar AEM Assets con Brand Portal son diferentes en función de la versión de AEM y de si va a realizar la configuración por primera vez o a actualizar las configuraciones existentes:

<!--| **AEM Version** |**New Configuration** |**Upgrade Configuration** |
|---|---|---|
| **AEM 6.5 (6.5.4.0 and above)** |[Create configuration](../using/brand-portal-configure-integration-65.md) |[Upgrade configuration](../using/brand-portal-configure-integration-65.md#upgrade-integration-65) | 
| **AEM 6.4 (6.4.8.0 and above)** |[Create configuration](../using/brand-portal-configure-integration-64.md) |[Upgrade configuration](../using/brand-portal-configure-integration-64.md#upgrade-integration-64) | 
| **AEM 6.3 (6.3.3.8 and above)** |[Create configuration](../using/brand-portal-configure-integration-63.md) |[Upgrade configuration](../using/brand-portal-configure-integration-63.md#upgrade-integration-63) | 
| **AEM 6.2** |Contact Support |Contact Support | 
-->


<!-- AEM Assets configuration with Brand Portal on Adobe I/O is supported on:
* AEM 6.5.4.0 and above
* AEM 6.4.8.0 and above
* AEM 6.3.3.8 and above -->

| **Versión de AEM** | **Nueva configuración** | **Configuración de actualización** |
|---|---|---|
| **AEM Assets as a Cloud Service** | [Crear configuración](https://docs.adobe.com/content/help/en/experience-manager-cloud-service/assets/brand-portal/configure-aem-assets-with-brand-portal.html) | - |
| **AEM 6.5 (6.5.4.0 y posterior)** | [Crear configuración](https://docs.adobe.com/content/help/en/experience-manager-65/assets/brandportal/configure-aem-assets-with-brand-portal.html) | [Configuración de actualización](https://docs.adobe.com/content/help/en/experience-manager-65/assets/brandportal/configure-aem-assets-with-brand-portal.html#upgrade-integration-65) |
| **AEM 6.4 (6.4.8.0 y posterior)** | [Crear configuración](https://docs.adobe.com/content/help/en/experience-manager-64/assets/brandportal/configure-aem-assets-with-brand-portal.html) | [Configuración de actualización](https://docs.adobe.com/content/help/en/experience-manager-64/assets/brandportal/configure-aem-assets-with-brand-portal.html#upgrade-integration-64) |
| **AEM 6.3 (6.3.3.8 y posterior)** | [Crear configuración](https://helpx.adobe.com/experience-manager/6-3/assets/using/brand-portal-configuring-integration.html) | [Configuración de actualización](https://helpx.adobe.com/experience-manager/6-3/assets/using/brand-portal-configuring-integration.html#Upgradeconfiguration) |
| **AEM 6.2** | Comuníquese con la asistencia técnica | Comuníquese con la asistencia técnica |

>[!NOTE]
>
>Se recomienda actualizar la instancia de AEM a Service Pack más reciente.

Consulte las últimas notas de la versión [de Brand Portal](brand-portal-release-notes.md).

Consulte las preguntas más frecuentes sobre [Brand Portal](brand-portal-faqs.md).

## Qué cambió en 6.4.5 {#what-changed-in-645}


Brand Portal 6.4.5 es una versión de funciones que se centra en proporcionar a los usuarios de Brand Portal (agencias/equipos externos) la capacidad de cargar contenido en Brand Portal y publicarlo en AEM Assets, sin la necesidad de acceder al entorno de creación. Esta función se denomina **[Asset Sourcing en Brand Portal](brand-portal-asset-sourcing.md)** y mejorará las experiencias de los clientes al proporcionar un mecanismo bidireccional para que los usuarios contribuyan y compartan recursos con otros usuarios de Brand Portal distribuidos globalmente.

### Origen de recursos en Brand Portal {#asset-sourcing-in-bp}

La fuente de recursos permite a los usuarios de AEM (administradores/usuarios no administradores) crear nuevas carpetas con una propiedad de contribución **de** recursos adicional, lo que garantiza que la nueva carpeta creada esté abierta al envío de recursos por parte de los usuarios de Brand Portal. Esto desencadena automáticamente un flujo de trabajo que crea dos subcarpetas adicionales, llamadas NUEVO y COMPARTIDO, dentro de la carpeta **Contribution** recién creada.

A continuación, el usuario AEM define el requisito [cargando un resumen](brand-portal-configure-contribution-folder-properties.md) sobre los tipos de recursos que deben agregarse a la carpeta de contribución, así como [cargando recursos](brand-portal-upload-baseline-assets.md)de línea de base a la carpeta **COMPARTIDO** para garantizar que los usuarios de BP tengan la información de referencia que necesitan. A continuación, el administrador puede otorgar a los usuarios activos de Brand Portal acceso a la carpeta de contribución antes de publicar la carpeta de **contribución** recién creada en Brand Portal.


Una vez que el usuario haya terminado de añadir contenido en la carpeta **NEW** , podrá volver a publicar la carpeta de contribución en el entorno de creación de AEM. Tenga en cuenta que la importación puede tardar unos minutos en completarse y reflejar el contenido recién publicado en AEM Assets.

Además, todas las funcionalidades existentes permanecen sin cambios. Los usuarios de Brand Portal pueden realizar vistas, búsquedas y descargas de recursos desde la carpeta de contribución, así como desde las demás carpetas permitidas. Además, los administradores pueden compartir la carpeta de contribución, modificar las propiedades y añadir recursos a las colecciones.

>[!NOTE]
>
>La fuente de recursos en Brand Portal es compatible con AEM 6.5.2.0 y versiones posteriores.
>
>La función no se admite en versiones anteriores: AEM 6.3 y AEM 6.4.

### Carga de recursos en la carpeta de contribución {#upload-assets-in-bp}

Los usuarios de Brand Portal con los permisos adecuados pueden [descargar los requisitos](brand-portal-download-asset-requirements.md) de recursos para comprender la necesidad de contribución y cargar varios recursos o carpetas que contengan varios recursos en la carpeta de contribución. Sin embargo, tenga en cuenta que los usuarios de Brand Portal solo pueden cargar recursos en la subcarpeta **NEW** . La carpeta **SHARED** está pensada para la distribución de requisitos y recursos de línea de base. Consulte [Carga de recursos en la carpeta de contribución](brand-portal-upload-assets-to-contribution-folder.md)

![](assets/upload-asset6.png)

![](assets/upload-asset4.png)


### Publicar carpeta de contribución en AEM Assets {#publish-assets-to-aem}

Una vez completada la carga en la carpeta **NEW** , los usuarios de Brand Portal pueden publicar la carpeta de contribución en AEM. Puede tardar unos minutos en importar y reflejar el contenido o los recursos publicados en AEM Assets. Consulte [Publicación de la carpeta de contribución en AEM Assets](brand-portal-publish-contribution-folder-to-aem-assets.md)


![](assets/upload-asset5.png)

## Qué cambió en 6.4.4 {#what-changed-in-644}

La versión 6.4.4 de Brand Portal se centra en las mejoras en la búsqueda de texto y en las principales solicitudes de los clientes. Consulte las últimas notas de la versión [de Brand Portal](brand-portal-release-notes.md).

### Mejoras de búsqueda

A partir de la versión 6.4.4 de Brand Portal, se admite la búsqueda de texto parcial en el predicado de propiedades en el panel de filtrado. Para permitir la búsqueda de texto parcial, debe habilitar la búsqueda **parcial** en el predicado de propiedades en el formulario de búsqueda.

Continúe leyendo para obtener más información sobre la búsqueda de texto parcial y la búsqueda con comodines.

#### Búsqueda de frase parcial {#partial-phrase-search}

Ahora puede buscar recursos especificando solo una parte (es decir, una palabra o dos) de la frase buscada en el panel de filtrado.

**Caso** de uso La búsqueda parcial de frases resulta útil cuando no está seguro de la combinación exacta de palabras que se producen en la frase buscada.

Por ejemplo, si el formulario de búsqueda en Brand Portal utiliza Property Predicate para la búsqueda parcial del título de los recursos, al especificar el término **camp** se devuelven todos los recursos con la palabra camp en su frase de título.

![](assets/partialphrasesearch.png)

#### Búsqueda de comodines {#wildcard-search}

El portal de marcas permite utilizar el asterisco (*) en la consulta de búsqueda junto con una parte de la palabra de la frase buscada.

**Caso** de uso Si no está seguro de las palabras exactas que se producen en la frase buscada, puede utilizar una búsqueda comodín para llenar los espacios en la consulta de búsqueda.

Por ejemplo, si se especifica **escalar*** , se devuelven todos los recursos con palabras que comienzan con los caracteres **escalar** en la frase de título si el formulario de búsqueda en Brand Portal utiliza Predicado de propiedades para la búsqueda parcial del título de los recursos.

![](assets/wildcard-prop.png)

Del mismo modo, especificando:

* ***escalar** devuelve todos los recursos que tienen palabras que finalizan con caracteres **escalados** en la frase de título.

* ***escalar*** devuelve todos los recursos que tienen palabras que comprenden los caracteres que **suben** en la frase de título.

>[!NOTE]
>
>Al seleccionar la casilla de verificación Búsqueda **** parcial, se selecciona **Omitir caso** de forma predeterminada.

[![](https://helpx.adobe.com/content/dam/help/en/experience-manager/brand-portal/images/see-the-guide.png)](../using/brand-portal-searching.md#facetedsearchbyapplyingfilterstosearch)

## Qué cambió en 6.4.3 {#what-changed-in}

La versión de Brand Portal 6.4.3 se centra en: proporcionar a las organizaciones un alias alternativo además de su ID de inquilino en la URL de acceso a Brand Portal, nueva configuración de jerarquía de carpetas, mejoras en la compatibilidad con vídeo, publicación programada de la instancia de AEM Author en Brand Portal, mejoras operativas — y atiende las solicitudes de los clientes.

### Navegación de jerarquía de carpetas para usuarios que no son administradores

Los administradores ahora pueden configurar cómo se muestran las carpetas a los usuarios no administradores (editores, visores y usuarios invitados) al iniciar sesión. [Habilitar la configuración de jerarquía](../using/brand-portal-general-configuration.md) de carpetas se agrega en Configuración **** general, en el panel Herramientas de administración. Si la configuración es:

* **activado**, el árbol de carpetas que comienza desde la carpeta raíz es visible para los usuarios no administradores. Por lo tanto, concederles una experiencia de navegación similar a la de los administradores.
* **está desactivada**, solo se muestran en la página de aterrizaje las carpetas compartidas.

![](assets/enable-folder-hierarchy.png)

La funcionalidad [Habilitar jerarquía](../using/brand-portal-general-configuration.md) de carpetas (cuando está habilitada) ayuda a diferenciar las carpetas con los mismos nombres compartidos de jerarquías diferentes. Al iniciar sesión, los usuarios que no son administradores ahora ven las carpetas principales virtuales (y antecesoras) de las carpetas compartidas.

![](assets/disabled-folder-hierarchy1-2.png)

![](assets/enabled-hierarchy1-2.png)

Las carpetas compartidas están organizadas dentro de los directorios respectivos en carpetas virtuales. Puede reconocer estas carpetas virtuales con un icono de candado.

Tenga en cuenta que la miniatura predeterminada de las carpetas virtuales es la imagen en miniatura de la primera carpeta compartida.

![](assets/hierarchy1-nonadmin-2.png)

[![](https://helpx.adobe.com/content/dam/help/en/experience-manager/brand-portal/images/see-the-guide.png)](../using/brand-portal-general-configuration.md)

### Buscar en una ruta o jerarquía de carpetas específica

**El predicado del explorador** de rutas se introduce en el formulario de búsqueda para permitir la búsqueda de recursos en un directorio específico. La ruta de búsqueda predeterminada del predicado de búsqueda para el Explorador de rutas es `/content/dam/mac/<tenant-id>/`, que se puede configurar editando el formulario de búsqueda predeterminado.

* Los usuarios administradores pueden utilizar el navegador de rutas para desplazarse a cualquier directorio de carpetas de Brand Portal.
* Los usuarios que no son administradores pueden utilizar el navegador de rutas para desplazarse únicamente a las carpetas (y volver a las carpetas principales) compartidas con ellos.

   Por ejemplo, `/content/dam/mac/<tenant-id>/folderA/folderB/folderC` se comparte con un usuario no administrador. El usuario puede buscar recursos dentro de folderC mediante el navegador de rutas. Este usuario también puede desplazarse a la carpeta B y a la carpeta A (ya que son antecesores de la carpeta C que se comparte con el usuario).

![](assets/edit-search-form.png)


Ahora puede restringir la búsqueda de recursos dentro de una carpeta específica a la que ha navegado, en lugar de comenzar en la carpeta raíz.

Tenga en cuenta que la búsqueda en estas carpetas solo se obtiene a partir de los recursos que se han compartido con el usuario.

![](assets/filter-panel.png)

[![](https://helpx.adobe.com/content/dam/help/en/experience-manager/brand-portal/images/see-the-guide.png)](../using/brand-portal-search-facets.md#listofsearchpredicates)

### Compatibilidad con representaciones de vídeo de Dynamic Media

Los usuarios cuya instancia de AEM Author se encuentra en el modo híbrido Dynamic Media pueden realizar previsualizaciones y descargar las representaciones de medios dinámicos, además de los archivos de vídeo originales.

Para permitir la previsualización y descarga de representaciones de medios dinámicos en cuentas de inquilino específicas, los administradores deben especificar la Configuración **de medios** dinámicos (URL del servicio de vídeo (URL de DM-Gateway) y el ID de registro para recuperar el vídeo dinámico) en la configuración de **vídeo** desde el panel Herramientas de administración.


Los vídeos de Dynamic Media se pueden previsualizar en:

* Página de detalles del recurso
* Vista de tarjetas del recurso
* Página de previsualización de uso compartido de vínculos

Los códigos de vídeo de Dynamic Media se pueden descargar de:

* Brand Portal
* Vínculo compartido

![](assets/edit-dynamic-media-config.png)

[![](https://helpx.adobe.com/content/dam/help/en/experience-manager/brand-portal/images/see-the-guide.png)](../using/brand-portal.md#tenantaliasforportalurl)

### Publicación programada en Brand Portal

Los recursos (y las carpetas) publican el flujo de trabajo desde [AEM (6.4.2.0)](https://helpx.adobe.com/experience-manager/6-4/release-notes/sp-release-notes.html#main-pars_header_9658011) La instancia de creación en Brand Portal se puede programar para una fecha y hora posteriores.

Del mismo modo, los recursos publicados se pueden eliminar del portal en una fecha (hora) posterior, programando el flujo de trabajo Cancelar publicación desde Brand Portal.

![](assets/schedule-publish.png)

![](assets/publishlater-workflow.png)

[![](https://helpx.adobe.com/content/dam/help/en/experience-manager/brand-portal/images/see-the-guide.png)](../using/brand-portal.md#tenantaliasforportalurl)

### Alias de inquilino configurable en URL

Las organizaciones pueden personalizar la dirección URL del portal si tienen un prefijo alternativo en la dirección URL. Para obtener un alias para el nombre del inquilino en la dirección URL del portal existente, las organizaciones deben ponerse en contacto con la asistencia de Adobe.

Tenga en cuenta que solo se puede personalizar el prefijo de la dirección URL de Brand Portal y no toda la dirección URL.\
Por ejemplo, una organización con un dominio existente **geometSymmetrix.brand-portal.adobe.com** puede obtener **geomettrixinc.brand-portal.adobe.com** creada a petición.

Sin embargo, la instancia de AEM Author solo se puede [configurar](https://helpx.adobe.com/experience-manager/6-5/assets/using/brand-portal-configuring-integration.html) con la dirección URL de identificación del inquilino y no con la URL de alias del inquilino (alternativa).

Las organizaciones pueden satisfacer sus necesidades de marca personalizando la dirección URL del portal, en lugar de atenerse a la dirección URL proporcionada por Adobe.

[![](https://helpx.adobe.com/content/dam/help/en/experience-manager/brand-portal/images/see-the-guide.png)](../using/brand-portal.md#tenantaliasforportalurl)

### Mejoras de la experiencia de descarga

La versión oferta una experiencia de descarga simplificada con un número reducido de clics y advertencias, en:

* Al optar por descargar solo las representaciones (y no los recursos originales).
* Descarga de recursos cuando se restringe el acceso a las representaciones originales.

## Qué cambió en 6.4.2 {#what-changed-in-1}

La versión 6.4.2 de Brand Portal ofrece una amplia gama de funciones para satisfacer las necesidades de distribución de recursos de las organizaciones y ayudarles a llegar a un gran número de usuarios distribuidos globalmente mediante el acceso de los invitados y una experiencia óptima con las descargas aceleradas. Brand Portal también proporciona bueno control a las organizaciones a través de nuevas configuraciones para administradores, informes recién agregados y atención a las solicitudes de los clientes.

### Acceso de invitados

![](assets/bp-login-screen-1.png)

AEM portal de marca permite a los invitados acceder al portal. Un usuario invitado no necesita credenciales para entrar en el portal y puede acceder y descargar todas las carpetas y colecciones públicas. Los usuarios invitados pueden añadir recursos a su caja de iluminación (colección privada) y descargar los mismos recursos. También pueden vista los predicados de búsqueda y búsqueda de etiquetas inteligentes establecidos por los administradores. La sesión de invitado no permite a los usuarios crear colecciones y búsquedas guardadas ni compartirlas más, acceder a la configuración de carpetas y colecciones y compartir recursos como vínculos.

En una organización, se permiten varias sesiones de invitados simultáneas, lo que se limita al 10 % de la cuota total de usuarios por organización.

Una sesión de invitado permanece activa durante dos horas. Por lo tanto, el estado de la caja de luz también se conserva hasta dos horas después del tiempo de inicio de la sesión. Después de dos horas, la sesión de invitado debe reiniciarse, por lo que se pierde el estado de la caja de luz.

### Descargas aceleradas

Los usuarios de Brand Portal pueden aprovechar las rápidas descargas basadas en IBM Aspera Connect para obtener velocidades hasta 25 veces más rápidas y disfrutar de una experiencia de descarga sin problemas, independientemente de su ubicación en todo el mundo. Para descargar los recursos más rápidamente desde Brand Portal o el vínculo compartido, los usuarios deben seleccionar la opción **Activar aceleración** de descarga en el cuadro de diálogo de descarga, siempre que la aceleración de la descarga esté habilitada en su organización.

![](assets/donload-assets-dialog-2.png)

Para habilitar la descarga acelerada basada en IBM Aspera para la organización, los administradores pueden activar la opción **Activar aceleración** de descarga (que está deshabilitada de forma predeterminada) desde Configuración [](brand-portal-general-configuration.md#allow-download-acceleration) general en el panel Herramientas administrativas. Para obtener más información sobre los requisitos previos y los pasos de solución de problemas para descargar archivos de recursos más rápidamente desde Brand Portal y vínculos compartidos, consulte [Guía para acelerar las descargas desde Brand Portal](../using/accelerated-download.md#main-pars-header).

### Informe de inicios de sesión de usuario

Se ha introducido un nuevo informe para rastrear los inicios de sesión de los usuarios. El informe **de inicios de sesión** de usuario puede ser fundamental para permitir que las organizaciones auditen y verifiquen a los administradores delegados y otros usuarios de Brand Portal.

Los registros de informes muestran los nombres, los ID de correo electrónico, las personas (administrador, visor, editor, invitado), los grupos, el último inicio de sesión, el estado de actividad y el recuento de inicio de sesión de cada usuario desde la implementación de Brand Portal 6.4.2 hasta el momento de la generación de informes. Los administradores pueden exportar el informe como .csv. Junto con otros informes, el informe de inicios de sesión de usuario permite a las organizaciones monitorear más de cerca las interacciones de los usuarios con los recursos de marca aprobados, asegurando así el cumplimiento de las normas por parte de las oficinas de cumplimiento corporativo.

![](assets/user-logins-1.png)

### Acceso a las representaciones originales

Los administradores pueden restringir el acceso del usuario a los archivos de imagen originales (.jpeg, .tiff, .png, .bmp, .gif, .pjpeg, x-portable-anymap, x-portable-bitmap, x-portable-graymap, x-portable-pixmap, x-rgb, x-xbitmap, x-xxmap, x-icon, image/photoshop, image/x-photoshop, .x-photoshop psd, image/vnd.adobe.photoshop) y dar acceso a representaciones de baja resolución que descargan desde Brand Portal o vínculo compartido. Este acceso se puede controlar a nivel de grupo de usuarios desde la ficha Grupos de la página Funciones de usuario del panel Herramientas de administración.

![](assets/access-original-rend-1.png)

* De forma predeterminada, todos los usuarios pueden descargar las representaciones originales, ya que el acceso al original está habilitado para todos.
* Los administradores deben anular la selección de las casillas de verificación correspondientes para evitar que un grupo de usuarios acceda a las representaciones originales.
* Si un usuario es miembro de varios grupos, pero sólo uno de ellos tiene restricciones, las restricciones se aplican a ese usuario.
* Las restricciones no se aplican a los administradores, aunque sean miembros de grupos restringidos.
* Los permisos del usuario que comparte recursos como vínculo se aplican a los usuarios que descargan recursos mediante vínculos compartidos.

### Ruta de jerarquía de carpetas en vistas de tarjeta y Lista

Las tarjetas de carpetas, en la Vista de tarjetas, ahora muestran información sobre la jerarquía de carpetas a usuarios no administradores (Editor, Visor y Usuario invitado). Esta funcionalidad permite a los usuarios conocer la ubicación de las carpetas a las que acceden, con respecto a la jerarquía principal.

La información sobre la jerarquía de carpetas resulta especialmente útil para diferenciar las carpetas que tienen nombres similares a otras carpetas compartidas desde una jerarquía de carpetas diferente. Si los usuarios que no son administradores no conocen la estructura de carpetas de los recursos compartidos con ellos, los recursos o carpetas con nombres similares parecen confusos.

* Las rutas que se muestran en las tarjetas respectivas se truncan para adaptarse a los tamaños de las tarjetas. Sin embargo, los usuarios pueden ver la ruta completa como información del objeto al pasar el ratón por encima de la ruta truncada.

![](assets/folder-hierarchy1-1.png)

La Vista de lista muestra la ruta de los recursos en una columna para todos los usuarios de Brand Portal.

![](assets/list-view-1.png)

### Opción Información general para propiedades de recursos de vista

Brand Portal proporciona la opción Información general a los usuarios no administradores (editores, visores, usuarios invitados) para la vista de las propiedades de recursos de los recursos o carpetas seleccionados. La opción Información general está visible:

1. En la barra de herramientas de la parte superior, seleccione un recurso o una carpeta.
2. En la lista desplegable al seleccionar el Selector de raíl.

Al seleccionar la opción Información general mientras se selecciona un recurso o carpeta, los usuarios pueden ver el título, la ruta y la hora de creación de recursos. Mientras que, en la página de detalles del recurso, si selecciona la opción Información general, los usuarios podrán ver los metadatos del recurso.

![](assets/overview-option-2.png)

![](assets/overview-rail-selector-2.png)

## Nuevas configuraciones

Se añaden seis nuevas configuraciones para que los administradores habiliten o deshabiliten las siguientes funcionalidades en inquilinos específicos:

* Permitir el acceso de invitados
* Permitir que los usuarios soliciten acceso a Brand Portal
* Permitir que los administradores eliminen recursos de Brand Portal
* Permitir la creación de colecciones públicas
* Permitir la creación de colecciones inteligentes públicas
* Permitir aceleración de descarga

Las configuraciones anteriores están disponibles en Ajustes generales y de acceso en el panel Herramientas administrativas.

![](assets/access-configs-1.png)
![](assets/general-configs-1.png)
![](assets/admin-tools-panel-13.png)

### Interfaz de usuario de E/S de Adobe para configurar integraciones de autenticación

A partir de la versión 6.4.2 de Brand Portal, se utiliza la interfaz Adobe.io [https://legacy-oauth.cloud.adobe.io/](https://legacy-oauth.cloud.adobe.io/) para crear aplicaciones JWT, que permite configurar integraciones oAuth para permitir la integración de AEM Assets con Brand Portal. Anteriormente, la interfaz de usuario para configurar integraciones de OAuth estaba alojada en `https://marketing.adobe.com/developer/`. Para obtener más información sobre la integración de AEM Assets con Brand Portal para la publicación de recursos y colecciones en Brand Portal, consulte [Configurar la integración de AEM Assets con Brand Portal](https://docs.adobe.com/content/help/en/experience-manager-64/assets/brandportal/configure-aem-assets-with-brand-portal.html).

## Mejoras de búsqueda

Los administradores pueden hacer que los predicados de propiedades no distingan entre mayúsculas y minúsculas mediante el predicado de propiedades actualizado, que tiene una comprobación para ignorar mayúsculas y minúsculas. Esta opción está disponible para predicado de propiedades y predicado de propiedades de varios valores.\
Sin embargo, la búsqueda que no distingue entre mayúsculas y minúsculas es comparativamente más lenta que la búsqueda predeterminada del predicado de propiedades. Si hay demasiados predicados que no distinguen entre mayúsculas y minúsculas en el filtro de búsqueda, la búsqueda puede ralentizarse. Por lo tanto, es aconsejable utilizar la búsqueda sin distinción entre mayúsculas y minúsculas con prudencia.

## Qué cambió en 6.4.1 {#what-changed-in-2}

Brand Portal 6.4.1 es una versión de actualización de plataforma que incorpora varias funciones nuevas y mejoras fundamentales, como la exploración, la búsqueda y el rendimiento, para ofrecer una experiencia satisfactoria al cliente.

### Mejoras de exploración

* Nuevo carril del árbol de contenido para navegar rápidamente por una jerarquía de recursos.

![](assets/contenttree-2.png)

* Se han introducido nuevos métodos abreviados de teclado, por ejemplo _(p)_ para la navegación a la página de propiedades, _(e)_ para Editar y _(ctrl+c)_ para las operaciones de copia.
* Se ha mejorado el desplazamiento y la experiencia de carga diferida en la vista de tarjetas y listas para explorar un gran número de recursos.
* Vista de tarjetas mejorada compatible con tarjetas de distintos tamaños según la configuración de vista.

![](assets/cardviewsettings-1.png)

* La vista de tarjetas ahora muestra la marca de fecha y hora al pasar el ratón por encima de la etiqueta de fecha.

* Se ha mejorado la vista de columnas con **Más detalles** en la instantánea de recursos, lo que le permite desplazarse a la página de detalles de un recurso.

![](assets/columnmoredetail.png)

* La vista de lista ahora muestra los nombres de archivo de los recursos en la primera columna de forma predeterminada, además de la configuración regional, el tipo de recurso, las dimensiones, el tamaño, la clasificación y la información de publicación. Se puede utilizar la nueva configuración **de** Vista para configurar la cantidad de detalle que se mostrará en la vista de Listas.

* Se ha mejorado la experiencia de detalle de recursos con la capacidad de desplazarse hacia atrás y adelante entre recursos mediante los nuevos botones de navegación y el recuento de recursos de vista.

![](assets/navbtn.png)

* Nueva capacidad de previsualización de archivos de audio, cargados desde AEM, en la página de detalles del recurso.
* Nueva capacidad Recursos relacionados proporcionada en las propiedades de los recursos. Los recursos relacionados con otros recursos de origen o derivados en AEM y publicados en Brand Portal ahora tienen su relación intacta en Brand Portal, con vínculos a los recursos relacionados en la página de propiedades.
* Se ha introducido una nueva configuración para restringir la creación de colecciones públicas a los usuarios que no son administradores. Las organizaciones pueden trabajar con el equipo de asistencia de Adobe para configurar esta capacidad en cuentas específicas.

### Mejoras de búsqueda

* Capacidad introducida para volver a la misma posición en los resultados de búsqueda, después de navegar a un elemento de búsqueda, sin volver a ejecutar la consulta de búsqueda.
* Se ha proporcionado un nuevo recuento de resultados de búsqueda para mostrar el número de resultados de búsqueda.
* Se mejoró el filtro de búsqueda de tipo de archivo con la capacidad de filtrar los resultados de búsqueda en función de tipos MIME detallados, como .jpg, .png y .psd, en comparación con las opciones anteriores de Imágenes, Documentos y Multimedia.
* Se han mejorado los filtros de búsqueda de colecciones, con marcas de hora precisas en lugar de la funcionalidad del deslizador de tiempo anterior.
* Se han introducido nuevos filtros de tipo Acceso para buscar las colecciones que son públicas o no.

![](assets/accesstypefilter.png)

### Optimizaciones de descarga

* Se descarga directamente un solo archivo grande, sin necesidad de crear un archivo zip, lo que mejora la velocidad y el rendimiento.
* El límite de descargas postales para la función de uso compartido de vínculos ha aumentado a 5 GB, desde 1 GB.

* Ahora los usuarios pueden optar por descargar únicamente los archivos personalizados y originales, y evitar las representaciones integradas, mientras descargan recursos desde Brand Portal o a través de la función de vínculos compartidos.

![](assets/excludeautorendition.png)

### Mejoras de rendimiento

* Mejora de hasta un 100% en la velocidad de descarga de los recursos.
* Mejora de hasta un 40% en la respuesta de búsqueda de recursos.
* Mejora de hasta un 40 % en el rendimiento de navegación.

**Nota**: Las mejoras citadas son las pruebas realizadas en el laboratorio.

### Funciones de sistema de informes mejoradas

**Informe** de uso compartido de vínculos introducido Se ha introducido un nuevo informe para proporcionar información sobre los vínculos compartidos. El informe Compartir vínculos lista todas las direcciones URL, a los recursos, compartidas con usuarios internos y externos de toda la organización en el intervalo de tiempo especificado. También indica cuándo se compartió el vínculo, quién lo compartió y cuándo caduca.

![](assets/navigatereport.png)

**Se modificó el punto de entrada para acceder Informe** de uso El informe de uso ahora se consolida con otros informes y ahora se puede ver desde la consola Informes de recursos. Para acceder a la consola Informes de recursos, vaya al panel **Crear/Administrar informes** desde el panel Herramientas administrativas.

![](assets/accessassetreport.png)

**La mejor experiencia del usuario con la interfaz de sistema de informes** Sistema de informes en Brand Portal se ha vuelto más intuitiva e imparte bueno control a las organizaciones. Además de crear varios informes, los administradores ahora pueden volver a examinar los informes generados y descargarlos o eliminarlos, ya que estos informes se guardan en Brand Portal.

Cada uno de los informes que se crean se puede personalizar agregando o eliminando columnas predeterminadas. Además, se pueden agregar columnas personalizadas a los informes Descargar, Caducidad y Publicar para controlar su grado de granularidad.

### Herramientas de administración mejoradas

Se mejoró el selector de propiedades en las herramientas de administración para metadatos, búsqueda e informes con la capacidad de exploración y escritura anticipada para simplificar la experiencia de administración.

### Otras mejoras

* Los recursos publicados en Brand Portal desde AEM 6.3.2.1 y 6.4 ahora pueden ponerse a disposición del público para los usuarios generales de Brand Portal marcando la casilla de verificación Publicación de carpetas públicas en el cuadro de diálogo Replicación de AEM Assets Brand Portal.

![](assets/public-folder-publish.png)

* Los administradores reciben notificaciones por correo electrónico de solicitud de acceso, aparte de las notificaciones del área de notificación de Brand Portal, si alguien ha solicitado acceso a Brand Portal.

## Qué cambió en 6.3.2 {#what-changed-in-3}

Brand Portal 6.3.2 incluye una funcionalidad nueva y mejorada orientada a las principales solicitudes de los clientes y mejoras generales de rendimiento.

### Request access to Brand Portal {#request-access-to-brand-portal}

Ahora los usuarios pueden solicitar acceso a Brand Portal mediante la nueva función de acceso **** necesaria disponible en la pantalla de inicio de sesión de Brand Portal.

![](assets/bplogin_request_access.png)

Según si los usuarios tienen un Adobe ID o necesitan crear un Adobe ID, los usuarios pueden seguir el flujo de trabajo adecuado para enviar una solicitud. Los administradores de productos de Brand Portal reciben dichas solicitudes en el área de notificación y otorgan acceso a través de Adobe Admin Console.

Para obtener más información, consulte [Solicitud de acceso a Brand Portal](../using/brand-portal.md#requestaccesstobrandportal).

### Mejora en el informe de recursos descargados {#enhancement-in-the-assets-downloaded-report}

El informe de recursos descargados ahora incluye el recuento de descargas de recursos por usuario dentro del intervalo de fecha y hora especificado. Los usuarios pueden descargar este informe en formato .csv y compilar datos como el recuento total de descargas de un recurso con licencia.

![](assets/reports_download_downloaded_by.png)

Para obtener más información, consulte los pasos 3 y 6 en [Crear y administrar informes](../using/brand-portal-reports.md#createandmanageadditionalreports)adicionales.

### Notificación de mantenimiento de Brand Portal {#brand-portal-maintenance-notification}

Brand Portal ahora muestra una pancarta de notificación unos días antes de la próxima actividad de mantenimiento. Una notificación de muestra:

![](assets/bp_maintenance_notification-1.png)

Para obtener más información, consulte la notificación [](https://helpx.adobe.com/experience-manager/brand-portal/using/brand-portal.html#BrandPortalmaintenancenotification)de mantenimiento de Brand Portal.

### Mejora de los recursos con licencia compartidos mediante la función de uso compartido de vínculos {#enhancement-for-licensed-assets-shared-using-the-link-share-feature}

Al descargar recursos con licencia mediante la función de uso compartido de vínculos, ahora se le solicita que acepte el contrato de licencia para dichos recursos.

![](assets/copyright_management.png)

Para obtener más información, consulte el paso 12 en [Compartir recursos como vínculo](../using/brand-portal-link-share.md#shareassetsasalink).

### Mejora del selector de usuarios {#user-picker-enhancement}

El rendimiento del selector de usuarios ahora se ha mejorado para satisfacer las necesidades de los clientes con una gran base de usuarios.

### Cambios en la marca de Experience Cloud {#experience-cloud-branding-changes}

Brand Portal ahora se ajusta a la nueva marca Adobe Experience Cloud.

![](assets/bp_solution_switcher.png)

## Qué cambió en 6.3.1 {#what-changed-in-4}

Brand Portal 6.3.1 incluye una funcionalidad nueva y mejorada orientada a alinear Brand Portal con AEM.

### Interfaz de usuario actualizada {#upgraded-user-interface}

Para alinear la experiencia de usuario de Brand Portal con AEM, Adobe está realizando la transición a la interfaz de usuario de Coral 3. Este cambio mejora el uso general, incluida la navegación, y el aspecto.

#### Experiencia de navegación mejorada {#enhanced-navigational-experience}

* Acceso rápido a las herramientas administrativas a través del nuevo logotipo de Adobe:

![](assets/aemlogo-3.png)

* Navegación del producto a través de una superposición:

![](assets/overlay_navigation.png)

* Navegación rápida a carpetas principales:

![](assets/navigationparentfolders.png)

* Búsqueda y navegación rápidas al contenido y las herramientas necesarios:

![](assets/omnisearchicon.png)

### Experiencia de navegación mejorada {#enhanced-browsing-experience}

* Nueva vista de columna para explorar las carpetas anidadas:

![](assets/millercolumnnavigation.png) ![](assets/multi-columnview.png)

* En la lista de recursos de una carpeta, el último recurso cargado aparece en la parte superior.

### Experiencia de búsqueda mejorada {#enhanced-search-experience}

* La nueva función de búsqueda Omni facilita el acceso rápido al contenido, la capacidad o las etiquetas relevantes a través de sugerencias automáticas a medida que escribe las palabras clave de búsqueda. La búsqueda de Omni está disponible en todas las funciones de búsqueda.

![](assets/omnisearch_whatsnew.png)

* También puede agregar filtros de búsqueda a la búsqueda de Omni para reducir aún más y acelerar la búsqueda.

![](assets/omnisearch_withfilters.png)

* La nueva búsqueda basada en la clasificación de recursos le permite buscar recursos con clasificaciones, si se publican desde AEM Assets.
* La nueva función de búsqueda de varios valores acepta varias palabras clave con el operador Y para descubrir los recursos más rápido.
* La nueva capacidad de ampliación de búsqueda le permite mejorar la relevancia de la búsqueda para que los recursos específicos aparezcan en la parte superior de los resultados de búsqueda.
* La nueva función de búsqueda basada en rutas le permite proporcionar la ruta a una carpeta anidada para poder buscar recursos en esa carpeta.

#### Nueva búsqueda basada en etiquetas inteligentes {#new-smart-tags-based-search}

Si las imágenes con etiquetas inteligentes se publican desde AEM Assets en Brand Portal, puede buscar estas imágenes en Brand Portal utilizando los nombres de etiquetas inteligentes como palabras clave de búsqueda. Esta función solo está disponible para archivos.

### Experiencia de descarga mejorada {#enhanced-downloading-experience}

Después de descargar una carpeta anidada, puede conservar la jerarquía de carpetas original. Los recursos dentro de una carpeta anidada se pueden descargar en una sola carpeta, en lugar de carpetas independientes.

### Rendimiento mejorado {#improved-performance}

Las mejoras en las funciones de exploración, búsqueda y descarga mejoran significativamente el rendimiento de Brand Portal.

### New digital rights management for assets {#new-digital-rights-management-for-assets}

Los administradores pueden definir la fecha y hora de caducidad de los recursos antes de compartirlos. Una vez que un recurso caduca, es visible para los visores y editores, pero no se puede descargar. Cuando un recurso caduca, los administradores reciben una notificación.

### Clasificación de recursos mejorada {#enhanced-asset-sorting}

La ordenación de recursos en una carpeta de la vista de listas ya no está restringida al número de recursos que se muestran en la primera página. Todos los recursos de una carpeta se ordenan, independientemente de si todos aparecen en la primera página.

### Sistema de informes mejorado {#reporting-capabilities}

Los administradores pueden crear y administrar tres tipos de informes: recursos descargados, caducados y publicados. También está disponible la posibilidad de configurar las columnas de un informe y exportar los informes a formato CSV.

![](assets/newreport.png)

### Metadatos adicionales {#additional-metadata}

Brand Portal 6.3.1 introduce metadatos adicionales, que están a la par con AEM Assets 6.3. Puede utilizar el formulario Editor de Esquemas para controlar los metadatos que deben estar visibles en la página Propiedades de recursos. Los metadatos del recurso no son visibles para los usuarios de recursos compartidos de vínculos externos, que solo pueden realizar previsualizaciones y descargar recursos mediante la URL de uso compartido de vínculos.

![](assets/additionsinmetadata.png)

### Funciones adicionales para administradores {#additional-capabilities-for-administrators}

* Antes de finalizar las personalizaciones del fondo de pantalla de inicio de sesión, los administradores pueden realizar previsualizaciones de los cambios.

![](assets/wallpaperpreview.png)

* Una vez que un administrador agrega nuevos usuarios, no necesita aceptar invitaciones para agregarlos a Brand Portal, se agregan automáticamente.

### Nuevas funciones de publicación en AEM Assets 6.3 {#new-publishing-capabilities-in-aem-assets}

* Los administradores de AEM pueden publicar esquemas de metadatos de AEM Assets en Brand Portal mediante AEM 6.3 SP 1-CFP 1 (6.3.1.1), que estará disponible en el cuarto trimestre de 2017.

![](assets/publish_metadataschemaaemassets.png)

* Los administradores de AEM pueden publicar todas las etiquetas de AEM Assets en Brand Portal mediante AEM 6.2 SP1-CFP7 y AEM 6.3 SP 1-CFP 1 (6.3.1.1).

![](assets/publish_tags_aemassets.png)

* Desde AEM Assets, puede publicar recursos y colecciones que tengan etiquetas, incluidas etiquetas inteligentes. A continuación, puede buscar estos recursos o colecciones utilizando estas etiquetas como palabras clave de búsqueda en Brand Portal.
