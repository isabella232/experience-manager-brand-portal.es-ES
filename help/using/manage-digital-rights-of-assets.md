---
title: Administración de los derechos digitales de recursos
seo-title: Manage digital rights of assets
description: La activos de licencias y la caducidad de los enlaces activos y compartidos garantizan el uso controlado de estos activos y salvaguardarlos.
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

Garantizar la distribución y el uso seguros de los recursos creativos y del material de la marca es vital para proteger su marca. Esto se puede aplicar a toda la organización y en el exterior mediante la Asociación de una fecha y hora de caducidad con la activos publicada de AEM en Brand portal o mediante la licencia de estos activos para un uso condicional. Además, Brand portal permite especificar una fecha de caducidad para los vínculos a la activos compartido en Brand portal.

Continúe leyendo para saber cómo se protegen los activos en Brand portal y cuáles son los permisos de uso asociados.

## Caducidad del recurso {#asset-expiration}

La caducidad de recursos es una forma eficaz de controlar el uso de activos aprobados en el portal de marca en una organización. Todos los activos publicados de Recursos AEM en Brand portal pueden tener una fecha de caducidad, lo que limita el uso de estos activos por diferentes funciones de usuario.

### Permisos de uso relacionados con los activos caducados {#usage-permissions-expired-assets}

En Brand Portal, los administradores pueden ver, descargar y agregar recursos caducados a colecciones. Por su parte, los editores y visualizadores solo pueden ver y agregar recursos caducados a las colecciones.

Los administradores pueden publicar recursos caducados de AEM Assets en Brand Portal. Sin embargo, los recursos caducados no se pueden compartir mediante un vínculo de Brand Portal. Si selecciona cualquier recurso caducado de una carpeta que contenga recursos caducados y no caducados, la variable **[!UICONTROL Compartir vínculo]** La acción no está disponible. Sin embargo, si selecciona una carpeta que contiene recursos caducados y no caducados, la variable [!UICONTROL Compartir] y **[!UICONTROL Compartir vínculo]** Las acciones están disponibles.

>[!NOTE]
>
>Una carpeta se puede seguir compartiendo como vincular, igualado si contiene activos caducados. En este caso, el vincular no lista caducado activos y solo se comparten los activos no caducados.

La siguiente tabla muestra los permisos de uso de los recursos caducados:

|  | **[!UICONTROL Vínculos compartidos]** | **[!UICONTROL Descargar]** | **[!UICONTROL Propiedades]** | **[!UICONTROL Añadir a la colección]** | **[!UICONTROL Eliminar]** |
|---|---|---|---|---|---|
| **[!UICONTROL Administrador]** | Carácter | Disponible | Disponible | Disponible | Disponible |
| **[!UICONTROL Editor]** | Carácter | Carácter | Disponible | Disponible | No disponible |
| **[!UICONTROL Visor]** | No disponible | Carácter | Disponible | Disponible | No disponible |
| **[!UICONTROL Usuario invitado]** | No disponible | No disponible | Disponible | Disponible | No disponible |

>[!NOTE]
>
>Si los visualizadores y editores descargan una carpeta que contiene recursos caducados y no caducados, solo se descargan los recursos no caducados. Si una carpeta solo contiene recursos caducados, se descarga una carpeta vacía.

### Estado de caducidad de los recursos {#expiration-status-of-assets}

Puede vista el estado de caducidad de activos en su **[!UICONTROL Ver]** de tarjeta. Un indicador rojo en la tarjeta indica que el recurso ha caducado.

![](assets/expired_assets_cardview.png)

>[!NOTE]
>
>Las vistas Lista y Columna no muestran el estado de caducidad de los recursos.

## Caducidad de Asset Link {#asset-link-expiration}

Al compartir recursos mediante vínculos, los administradores y editores pueden establecer una fecha y una hora de caducidad mediante **[!UICONTROL Caducidad]** en el campo **[!UICONTROL Vínculos compartidos]** Cuadro de diálogo. La caducidad predeterminada del vínculo es de siete días a partir de la fecha en que se comparte.

![](assets/asset-link-sharing.png)

Garantiza que los recursos compartidos como vínculos caduquen en la fecha y hora establecidas por los administradores y editores de Brand Portal y que ya no se puedan ver ni descargar más allá de la fecha de caducidad. Como los recursos compartidos a través de vínculos también los pueden ver usuarios externos que no forman parte de la organización, al especificar la caducidad, puede asegurarse de que los recursos aprobados estén protegidos y no expuestos a entidades desconocidas más allá de un tiempo especificado.

Para obtener más información sobre cómo compartir vínculos, consulte [Uso compartido de recursos como vínculo](../using/brand-portal-link-share.md).

## Recursos con licencia {#licensed-assets}

Los activos con licencia están sujetos a la aceptación de un acuerdo de licencia antes de su descarga desde Brand Portal. Este acuerdo para los recursos con licencia se produce cuando se descarga directamente el recurso desde Brand Portal o a través de un vínculo compartido. Ya caducados o no, todos los usuarios pueden ver los recursos protegidos por licencias. Sin embargo, la descarga y el uso de los recursos con licencia caducados son limitados. Para obtener información sobre el comportamiento de los recursos con licencia caducados y las actividades permisibles basadas en las funciones de usuario, consulte [permisos de uso de recursos caducados](../using/manage-digital-rights-of-assets.md#usage-permissions-expired-assets).

Los activos protegidos por la licencia tienen [ un acuerdo de licencia vinculado ](https://experienceleague.adobe.com/docs/experience-manager-65/assets/administer/drm.html) a ellos, lo que se realiza estableciendo la metadatos Propiedad [!DNL Experience Manager Assets] del recurso.

Una recurso se considera protegida si contiene una de las siguientes propiedades (o ambas) metadatos:

* `xmpRights:WebStatement`: Este Propiedad hace referencia a la ruta de la Página que contiene el contrato de licencia para la recurso. `xmpRights:WebStatement` debe ser una ruta válida en el repositorio.
* `adobe_dam:restrictions`: El valor de esta Propiedad es un HTML sin procesar que especifica el contrato de licencia.


Si decide descargar recursos protegidos por licencias, se le redirigirá al **[!UICONTROL Administración de copyright]** según las propiedades de los metadatos.

| `adobe_dam:restrictions` | `xmpRights:WebStatement` | Administración de copyright |
| --- | --- | --- |
| Sí | - | La interfaz aparece tanto en como en Assets como en el portal de marca |
| - | Sí (ruta no válida) | Sin interfaz |
| Sí | Sí (ruta no válida) | Sin interfaz |
| Sí | Sí (ruta válida) | La interfaz aparece en Assets o Brand Portal </br> En función de si la ruta es válida para Assets o Brand Portal (o ambos). |

![](assets/asset-copyright-mgmt.png)

Aquí debe seleccionar el recurso que desea descargar y aceptar el acuerdo de licencia asociado. Si no acepta el acuerdo de licencia, la variable **[!UICONTROL Descargar]** El botón no está activado.

![](assets/licensed-asset-download-2.png)

Si la selección contiene varios recursos protegidos, seleccione un recurso a la vez, acepte el acuerdo de licencia y proceda a descargar el recurso.

## Generar informe sobre recursos caducados {#generate-report-about-expired-assets}

Los administradores pueden generar y descargar un informe que enumera todas las activos caducados dentro de una lapso de tiempo específica. Este informe incluye información detallada como, por ejemplo, el tamaño, el tipo, la ruta que especifica recurso ubicación en el recurso jerarquía, Cuándo caduca la recurso y Cuándo fue publicada la recurso, acerca de los activos caducados. Las columnas de este informe se pueden personalizar para mostrar más datos en base a los requisitos de usuario.

![](assets/assets-expired.png)

Para obtener más información sobre la función de informes, consulte [Trabajo con informes](../using/brand-portal-reports.md#work-with-reports).
