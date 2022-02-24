---
title: Administración de los derechos digitales de recursos
seo-title: Manage digital rights of assets
description: La licencia de recursos y la configuración de la caducidad para los recursos y los vínculos compartidos garantizan el uso controlado de estos recursos y los protegen.
seo-description: Licensing assets and setting expiration for assets and shared links ensure controlled usage of these assets and safeguard them.
uuid: ce30e398-0109-41bf-a4d2-2fcca476f499
contentOwner: bdhar
topic-tags: download-install
products: SG_EXPERIENCEMANAGER/Brand_Portal
content-type: reference
discoiquuid: f77003ba-31fe-4a9e-96c8-dbc4c2eba79e
role: Admin
exl-id: 86c31891-0627-41ca-b571-8dac3a074d55
source-git-commit: d1487434b10b01eaf55f34672267490fd8fd907e
workflow-type: tm+mt
source-wordcount: '907'
ht-degree: 2%

---

# Administración de los derechos digitales de recursos {#manage-digital-rights-of-assets}

Garantizar la distribución y el uso seguros de los recursos creativos y del material de marca es vital para proteger su marca. Esto se puede hacer cumplir en toda la organización y fuera de ella asociando una fecha (y hora) de caducidad con los recursos aprobados publicados de AEM a Brand Portal o otorgando licencias a estos recursos para su uso condicional. Además, Brand Portal le permite especificar una fecha de caducidad para los vínculos a los recursos compartidos desde Brand Portal.

Continúe leyendo para saber cómo se protegen los recursos en Brand Portal y comprenda los permisos de uso asociados.

## Caducidad del recurso {#asset-expiration}

La caducidad de los recursos es una forma eficaz de controlar el uso de los recursos aprobados en Brand Portal en toda una organización. Todos los recursos publicados desde AEM Assets en Brand Portal pueden tener una fecha de caducidad, lo que restringe el uso de estos recursos por diferentes funciones de usuario.

### Permisos de uso relacionados con recursos caducados {#usage-permissions-expired-assets}

En Brand Portal, los administradores pueden ver, descargar y agregar recursos caducados a las colecciones. Por su parte, los editores y los visualizadores solo pueden ver y añadir recursos caducados a las colecciones.

Los administradores pueden publicar recursos caducados de AEM Assets en Brand Portal. Sin embargo, los recursos caducados no se pueden compartir mediante vínculo desde Brand Portal. Si selecciona cualquier recurso caducado de una carpeta que contenga tanto recursos caducados como no caducados, la variable **[!UICONTROL Compartir vínculo]** la acción no está disponible. Sin embargo, si selecciona una carpeta que contiene recursos caducados y no caducados, la variable [!UICONTROL Compartir] y **[!UICONTROL Compartir vínculo]** están disponibles.

>[!NOTE]
>
>Una carpeta se puede seguir compartiendo como vínculo, incluso si contiene recursos caducados. En este caso, el vínculo no enumera los recursos caducados y solo se comparten los recursos no caducados.

La tabla siguiente muestra los permisos de uso de los recursos caducados:

|  | **[!UICONTROL Compartir vínculos]** | **[!UICONTROL Descargar]** | **[!UICONTROL Propiedades]** | **[!UICONTROL Agregar a colección]** | **[!UICONTROL Eliminar]** |
|---|---|---|---|---|---|
| **[!UICONTROL Administrador]** | No disponible | Disponible | Disponible | Disponible | Disponible |
| **[!UICONTROL Editor]** | No disponible | No disponible | Disponible | Disponible | No disponible |
| **[!UICONTROL Visor]** | No disponible | No disponible | Disponible | Disponible | No disponible |
| **[!UICONTROL Usuario invitado]** | No disponible | No disponible | Disponible | Disponible | No disponible |

>[!NOTE]
>
>Si Visualizadores y editores descargan una carpeta que contenga recursos caducados y no caducados, solo se descargarán los recursos que no hayan caducado. Si una carpeta contiene solo recursos caducados, se descarga una carpeta vacía.

### Estado de caducidad de los activos {#expiration-status-of-assets}

Puede ver el estado de caducidad de los recursos en sus **[!UICONTROL Vista de tarjeta]**. Un indicador rojo en la tarjeta indica que el recurso ha caducado.

![](assets/expired_assets_cardview.png)

>[!NOTE]
>
>Las vistas Lista y Columna no muestran el estado de caducidad de los recursos.

## Caducidad del vínculo de recursos {#asset-link-expiration}

Al compartir recursos a través de vínculos, los administradores y editores pueden establecer una fecha y hora de caducidad mediante la variable **[!UICONTROL Caducidad]** en el campo **[!UICONTROL Uso compartido de vínculos]** para abrir el Navegador. La caducidad predeterminada del vínculo es de siete días a partir de la fecha en que se comparte.

![](assets/asset-link-sharing.png)

Garantiza que los recursos compartidos como vínculos caduquen en la fecha y la hora establecidas por los administradores y editores de Brand Portal, y que ya no se puedan ver ni descargar más allá de la fecha de caducidad. Como los recursos compartidos a través de vínculos también pueden verlos usuarios externos que no forman parte de la organización, al especificar la caducidad, puede asegurarse de que los recursos aprobados estén protegidos y no estén expuestos a entidades desconocidas más allá de un tiempo especificado.

Para obtener más información sobre el uso compartido de vínculos, consulte [Compartir recursos como vínculo](../using/brand-portal-link-share.md).

## Recursos con licencia {#licensed-assets}

Los recursos con licencia están sujetos a la aceptación de un acuerdo de licencia antes de su descarga desde Brand Portal. Este acuerdo para los recursos con licencia se produce cuando se descarga directamente el recurso desde Brand Portal o a través de un vínculo compartido. Ya sea que haya caducado o no, todos los usuarios pueden ver los recursos protegidos por licencias. Sin embargo, la descarga y el uso de recursos con licencia caducados son limitados. Para obtener información sobre el comportamiento de los recursos con licencia caducados y las actividades permisibles basadas en las funciones de usuario, consulte [permisos de uso de recursos caducados](../using/manage-digital-rights-of-assets.md#usage-permissions-expired-assets).

Los recursos protegidos por licencias tienen [contrato de licencia adjunto](https://experienceleague.adobe.com/docs/experience-manager-65/assets/administer/drm.html) para ellos, lo que se hace estableciendo la propiedad de metadatos del recurso en [!DNL Experience Manager Assets].

Un recurso se considera protegido si contiene una de las siguientes propiedades de metadatos (o ambas):

* `xmpRights:WebStatement`: Esta propiedad hace referencia a la ruta de la página que contiene el acuerdo de licencia del recurso. `xmpRights:WebStatement` debe ser una ruta válida en el repositorio.
* `adobe_dam:restrictions`: El valor de esta propiedad es un HTML sin procesar que especifica el acuerdo de licencia.


Si decide descargar recursos protegidos por licencias, se le redirigirá al **[!UICONTROL Administración de derechos de autor]** en función de las propiedades de los metadatos.

| `adobe_dam:restrictions` | `xmpRights:WebStatement` | Administración de copyright |
| --- | --- | --- |
| Sí | - | La interfaz aparece tanto en Assets como en Brand Portal |
| - | Sí (ruta de acceso no válida) | Sin interfaz |
| Sí | Sí (ruta de acceso no válida) | Sin interfaz |
| Sí | Sí (ruta válida) | La interfaz aparece en Assets o Brand Portal </br> Dependiendo de si la ruta es válida para Assets o Brand Portal (o ambos). |

![](assets/asset-copyright-mgmt.png)

Aquí debe seleccionar el recurso para descargar y aceptar el acuerdo de licencia asociado. Si no acepta el acuerdo de licencia, la variable **[!UICONTROL Descargar]** no está activado.

![](assets/licensed-asset-download-2.png)

Si la selección contiene varios recursos protegidos, seleccione un recurso a la vez, acepte el acuerdo de licencia y continúe descargando el recurso.

## Generar informe de activos caducados {#generate-report-about-expired-assets}

Los administradores pueden generar y descargar un informe con todos los recursos caducados en un lapso de tiempo específico. Este informe incluye información detallada (como tamaño, tipo, ruta que especifica la ubicación del recurso en la jerarquía de activos, cuándo caducó el activo y cuándo se publicó el activo) sobre los activos caducados. Las columnas de este informe se pueden personalizar para que muestren más datos según los requisitos del usuario.

![](assets/assets-expired.png)

Para obtener más información sobre la función de informes, consulte [Trabajar con informes](../using/brand-portal-reports.md#work-with-reports).
