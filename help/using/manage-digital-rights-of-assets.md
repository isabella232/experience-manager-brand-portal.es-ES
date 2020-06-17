---
title: Administración de los derechos digitales de recursos
seo-title: Administración de los derechos digitales de recursos
description: La concesión de licencias a los recursos y la configuración de la caducidad de los recursos y los vínculos compartidos garantizan el uso controlado de estos recursos y la protección de los mismos.
seo-description: La concesión de licencias a los recursos y la configuración de la caducidad de los recursos y los vínculos compartidos garantizan el uso controlado de estos recursos y la protección de los mismos.
uuid: ce30e398-0109-41bf-a4d2-2fcca476f499
contentOwner: bdhar
topic-tags: download-install
products: SG_EXPERIENCEMANAGER/Brand_Portal
content-type: reference
discoiquuid: f77003ba-31fe-4a9e-96c8-dbc4c2eba79e
translation-type: tm+mt
source-git-commit: b724038ac2b6ea5189a012fbb2f812a2a55ffcd0
workflow-type: tm+mt
source-wordcount: '829'
ht-degree: 2%

---


# Administración de los derechos digitales de recursos {#manage-digital-rights-of-assets}

Garantizar la distribución y el uso seguros de los activos creativos y del material de la marca es vital para proteger su marca. Esto se puede hacer cumplir en toda la organización y fuera de ella asociando una fecha (y hora) de caducidad con los recursos aprobados publicados desde AEM a Brand Portal, o autorizando estos recursos para uso condicional. Además, Brand Portal le permite especificar una fecha de caducidad para los vínculos a los recursos compartidos desde Brand Portal.

Continúe leyendo para saber cómo se protegen los recursos en Brand Portal y comprenda los permisos de uso asociados.

## Caducidad del recurso {#asset-expiration}

La caducidad de los recursos es una forma eficaz de controlar el uso de los recursos aprobados en Brand Portal en toda una organización. Todos los recursos publicados desde AEM Assets hasta Brand Portal pueden tener una fecha de caducidad, lo que restringe el uso de estos recursos según las distintas funciones de usuario.

### Permisos de uso relacionados con recursos caducados {#usage-permissions-expired-assets}

En Brand Portal, los administradores pueden realizar vistas, descargar y añadir recursos caducados a las colecciones. Mientras que los editores y los visores solo pueden realizar vistas y añadir recursos caducados a las colecciones.

Los administradores pueden publicar recursos caducados de AEM Assets en Brand Portal. Sin embargo, los recursos caducados no se pueden compartir mediante tinta desde Brand Portal. Si selecciona cualquier recurso caducado de una carpeta que contenga tanto recursos caducados como no caducados, la acción **[!UICONTROL Compartir vínculo]** no estará disponible. Sin embargo, si selecciona una carpeta que contiene recursos caducados y no caducados, estarán disponibles las acciones [!UICONTROL Compartir] y **[!UICONTROL Compartir vínculo]** .

>[!NOTE]
>
>Una carpeta puede seguir compartiéndose como vínculo, incluso si contiene recursos caducados. En este caso, el vínculo no lista los recursos caducados y solo se comparten los recursos no caducados.


La siguiente tabla muestra los permisos de uso de los recursos caducados:

|  | **[!UICONTROL Uso compartido de vínculos]** | **[!UICONTROL Descargar]** | **[!UICONTROL Propiedades]** | **[!UICONTROL Añadir a la colección]** | **[!UICONTROL Eliminar]** |
|---|---|---|---|---|---|
| **[!UICONTROL Administrador]** | No disponible | Disponible | Disponible | Disponible | Disponible |
| **[!UICONTROL Editor]** | No disponible | No disponible | Disponible | Disponible | No disponible |
| **[!UICONTROL Visor]** | No disponible | No disponible | Disponible | Disponible | No disponible |
| **[!UICONTROL Usuario invitado]** | No disponible | No disponible | Disponible | Disponible | No disponible |

>[!NOTE]
>
>Si los visores y editores descargan una carpeta que contenga recursos caducados y no caducados, solo se descargarán los recursos que no hayan caducado. Si una carpeta solo contiene recursos caducados, se descarga una carpeta vacía.


### Estado de caducidad de los activos {#expiration-status-of-assets}

Puede vista del estado de caducidad de los recursos en su Vista **** de tarjetas. Un indicador rojo de la tarjeta indica que el recurso ha caducado.

![](assets/expired_assets_cardview.png)

>[!NOTE]
>
>Las vistas de Listas y columnas no muestran el estado de caducidad de los recursos.


## Caducidad del vínculo de recursos {#asset-link-expiration}

Al compartir recursos a través de vínculos, los administradores y editores pueden establecer una fecha y hora de caducidad mediante el campo **[!UICONTROL Caducidad]** del cuadro de diálogo Uso compartido **[!UICONTROL de]** vínculos. La caducidad predeterminada del vínculo es de siete días a partir de la fecha en que se comparte.

![](assets/asset-link-sharing.png)

Garantiza que los recursos compartidos como vínculos caduquen en la fecha y hora establecidas por los administradores y editores de Brand Portal y que ya no se puedan ver ni descargar más allá de la fecha de caducidad. Dado que los recursos compartidos mediante vínculos también pueden ser vistos por usuarios externos que no forman parte de la organización, al especificar la caducidad puede asegurarse de que los recursos aprobados están protegidos y no expuestos a entidades desconocidas más allá de un tiempo especificado.

Para obtener más información sobre el uso compartido de vínculos, consulte [Compartir recursos como vínculo](../using/brand-portal-link-share.md).

## Recursos con licencia {#licensed-assets}

Los recursos con licencia están sujetos a la aceptación de un contrato de licencia antes de descargarlos de Brand Portal. Este acuerdo para los recursos con licencia se produce cuando se descarga directamente el recurso desde Brand Portal o a través de un vínculo compartido. Todos los usuarios pueden ver los recursos protegidos por licencias que hayan caducado o no. Sin embargo, la descarga y el uso de los recursos con licencia caducados son limitados. Para conocer el comportamiento de los recursos con licencia caducados y las actividades permisibles en función de las funciones de usuario, consulte los permisos de [uso de los recursos](../using/manage-digital-rights-of-assets.md#usage-permissions-expired-assets)caducados.

Los recursos protegidos por licencias tienen un contrato de [licencia adjunto](https://helpx.adobe.com/experience-manager/6-5/assets/using/drm.html#DigitalRightsManagementinAssets) , lo que se realiza estableciendo la propiedad [de](https://helpx.adobe.com/experience-manager/6-5/assets/using/drm.html#DigitalRightsManagementinAssets) metadatos del recurso en AEM Assets.

Si decide descargar recursos protegidos por licencias, se le redirigirá a la página Administración **[!UICONTROL de]** derechos de autor.

![](assets/asset-copyright-mgmt.png)

Aquí debe seleccionar el recurso para descargar y aceptar el contrato de licencia asociado. Si no acepta el contrato de licencia, el botón **[!UICONTROL Descargar]** no estará activado.

![](assets/licensed-asset-download-2.png)

Si la selección contiene varios recursos protegidos, selecciónelos de uno en uno, acepte el contrato de licencia y continúe con la descarga del recurso.

## Generar informe de recursos caducados {#generate-report-about-expired-assets}

Los administradores pueden generar y descargar un informe que enumera todos los recursos caducados dentro de un intervalo de tiempo específico. Este informe incluye información detallada— como tamaño, tipo, ruta de acceso que especifica la ubicación del recurso en la jerarquía de recursos, cuándo caducó el recurso y cuándo se publicó el activo— acerca de los recursos caducados. Las columnas de este informe se pueden personalizar para mostrar más datos en función de los requisitos del usuario.

![](assets/assets-expired.png)

Para obtener más información sobre la función de informes, consulte [Trabajar con informes](../using/brand-portal-reports.md#work-with-reports).
