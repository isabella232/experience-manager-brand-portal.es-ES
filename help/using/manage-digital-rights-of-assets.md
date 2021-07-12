---
title: Administración de los derechos digitales de recursos
seo-title: Administración de los derechos digitales de recursos
description: La licencia de recursos y la configuración de la caducidad para los recursos y los vínculos compartidos garantizan el uso controlado de estos recursos y los protegen.
seo-description: La licencia de recursos y la configuración de la caducidad para los recursos y los vínculos compartidos garantizan el uso controlado de estos recursos y los protegen.
uuid: ce30e398-0109-41bf-a4d2-2fcca476f499
contentOwner: bdhar
topic-tags: download-install
products: SG_EXPERIENCEMANAGER/Brand_Portal
content-type: reference
discoiquuid: f77003ba-31fe-4a9e-96c8-dbc4c2eba79e
role: Admin
exl-id: 86c31891-0627-41ca-b571-8dac3a074d55
source-git-commit: 26b009fec800d9b437bde5838009c71b1b3b7ac6
workflow-type: tm+mt
source-wordcount: '829'
ht-degree: 2%

---

# Administración de los derechos digitales de recursos {#manage-digital-rights-of-assets}

Garantizar la distribución y el uso seguros de los recursos creativos y del material de marca es vital para proteger su marca. Esto se puede hacer cumplir en toda la organización y fuera de ella asociando una fecha (y hora) de caducidad con los recursos aprobados publicados de AEM a Brand Portal o otorgando licencias a estos recursos para su uso condicional. Además, Brand Portal le permite especificar una fecha de caducidad para los vínculos a los recursos compartidos desde Brand Portal.

Continúe leyendo para saber cómo se protegen los recursos en Brand Portal y comprenda los permisos de uso asociados.

## Caducidad del recurso {#asset-expiration}

La caducidad de los recursos es una forma eficaz de controlar el uso de los recursos aprobados en Brand Portal en toda una organización. Todos los recursos publicados desde AEM Assets en Brand Portal pueden tener una fecha de caducidad, lo que restringe el uso de estos recursos por diferentes funciones de usuario.

### Permisos de uso relacionados con recursos caducados {#usage-permissions-expired-assets}

En Brand Portal, los administradores pueden ver, descargar y agregar recursos caducados a las colecciones. Por su parte, los editores y los visualizadores solo pueden ver y añadir recursos caducados a las colecciones.

Los administradores pueden publicar recursos caducados de AEM Assets en Brand Portal. Sin embargo, los recursos caducados no se pueden compartir mediante vínculo desde Brand Portal. Si selecciona cualquier recurso caducado de una carpeta que contenga tanto activos caducados como no caducados, la acción **[!UICONTROL Compartir vínculo]** no estará disponible. Sin embargo, si selecciona una carpeta que contiene activos caducados y no caducados, estarán disponibles las acciones [!UICONTROL Compartir] y **[!UICONTROL Compartir vínculo]**.

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

Puede ver el estado de caducidad de los recursos en su **[!UICONTROL Vista de tarjeta]**. Un indicador rojo en la tarjeta indica que el recurso ha caducado.

![](assets/expired_assets_cardview.png)

>[!NOTE]
>
>Las vistas Lista y Columna no muestran el estado de caducidad de los recursos.

## Caducidad del vínculo de recursos {#asset-link-expiration}

Al compartir recursos mediante vínculos, los administradores y editores pueden establecer una fecha y hora de caducidad mediante el campo **[!UICONTROL Expiration]** del cuadro de diálogo **[!UICONTROL Link Sharing]**. La caducidad predeterminada del vínculo es de siete días a partir de la fecha en que se comparte.

![](assets/asset-link-sharing.png)

Garantiza que los recursos compartidos como vínculos caduquen en la fecha y la hora establecidas por los administradores y editores de Brand Portal, y que ya no se puedan ver ni descargar más allá de la fecha de caducidad. Como los recursos compartidos a través de vínculos también pueden verlos usuarios externos que no forman parte de la organización, al especificar la caducidad, puede asegurarse de que los recursos aprobados estén protegidos y no estén expuestos a entidades desconocidas más allá de un tiempo especificado.

Para obtener más información sobre el uso compartido de vínculos, consulte [Compartir recursos como un vínculo](../using/brand-portal-link-share.md).

## Recursos con licencia {#licensed-assets}

Los recursos con licencia están sujetos a la aceptación de un acuerdo de licencia antes de su descarga desde Brand Portal. Este acuerdo para los recursos con licencia se produce cuando se descarga directamente el recurso desde Brand Portal o a través de un vínculo compartido. Ya sea que haya caducado o no, todos los usuarios pueden ver los recursos protegidos por licencias. Sin embargo, la descarga y el uso de recursos con licencia caducados son limitados. Para obtener información sobre el comportamiento de los recursos con licencia caducados y las actividades permisibles basadas en las funciones de usuario, consulte [permisos de uso de los recursos caducados](../using/manage-digital-rights-of-assets.md#usage-permissions-expired-assets).

Los recursos protegidos por licencias tienen [contrato de licencia adjunto](https://helpx.adobe.com/experience-manager/6-5/assets/using/drm.html#DigitalRightsManagementinAssets), lo que se hace estableciendo la [propiedad de metadatos](https://helpx.adobe.com/experience-manager/6-5/assets/using/drm.html#DigitalRightsManagementinAssets) del recurso en AEM Assets.

Si decide descargar recursos protegidos por licencias, se le redirigirá a la página **[!UICONTROL Administración de derechos de autor]**.

![](assets/asset-copyright-mgmt.png)

Aquí debe seleccionar el recurso para descargar y aceptar el acuerdo de licencia asociado. Si no acepta el acuerdo de licencia, el botón **[!UICONTROL Download]** no está habilitado.

![](assets/licensed-asset-download-2.png)

Si la selección contiene varios recursos protegidos, seleccione un recurso a la vez, acepte el acuerdo de licencia y continúe descargando el recurso.

## Generar informe de activos caducados {#generate-report-about-expired-assets}

Los administradores pueden generar y descargar un informe con todos los recursos caducados en un lapso de tiempo específico. Este informe incluye información detallada (como tamaño, tipo, ruta que especifica la ubicación del recurso en la jerarquía de activos, cuándo caducó el activo y cuándo se publicó el activo) sobre los activos caducados. Las columnas de este informe se pueden personalizar para que muestren más datos según los requisitos del usuario.

![](assets/assets-expired.png)

Para obtener más información sobre la función de informes, consulte [Trabajar con informes](../using/brand-portal-reports.md#work-with-reports).
