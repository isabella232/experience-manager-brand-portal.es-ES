---
title: Compatibilidad con vídeos dinámicos en Brand Portal
seo-title: Compatibilidad con vídeos dinámicos en Brand Portal
description: Compatibilidad con vídeos dinámicos en Brand Portal
seo-description: Compatibilidad con vídeos dinámicos en Brand Portal
uuid: a 3502 a 4 d -3971-4 ea 4-953 c -44 ba 04446269
contentOwner: mgulati
products: SG_ EXPERIENCEMANAGER/Brand_ Portal
content-type: referencia
topic-tags: descarga de descarga
discoiquuid: e 18 d 992 a-a 3 b 5-45 f 2-9696-8161993213 ee
translation-type: tm+mt
source-git-commit: d605cdd0083e8e222a3c937ea91d2c04201ab99b

---


# Compatibilidad con vídeos dinámicos en Brand Portal {#dynamic-video-support-on-brand-portal}

Obtenga una vista previa y reproduzca vídeos de forma adaptable en Brand Portal con Dynamic Media. Descargue también las representaciones dinámicas del portal y los vínculos compartidos.
Los usuarios de Brand Portal pueden:

* Previsualice vídeos en la página Detalles del recurso, la Vista de tarjeta y la página de vista previa del vínculo.
* Reproducir codificaciones de vídeo en la página Detalles del recurso.
* Vea representaciones dinámicas en la ficha Representaciones en la página Detalles del recurso.
* Descargue codificaciones y codificaciones de vídeo que contengan vídeos.

>[!NOTE]
>
>Para trabajar con vídeos y publicarlos en Brand Portal, asegúrese de que la instancia de AEM Author esté configurada en modo Dynamic Media Híbrido o en [!DNL Scene 7] modo Dynamic Media.

Para obtener una vista previa, reproducir y descargar vídeos, Brand Portal expone las dos configuraciones siguientes a los administradores:

* [Configuración
híbrida de Dynamic Media](#configure-dm-hybrid-settings)Si la instancia de AEM Author se ejecuta en modo híbrido Dynamic Media.
* [Dynamic Media [! Configuración
DNL Scene 7]](#configure-dm-scene7-settings)Si la instancia de AEM Author se ejecuta en medios dinámicos.
[!DNL Scene 7]
Defina cualquiera de estas configuraciones según las configuraciones configuradas en su instancia de AEM Author con la que se replica el inquilino Brand Portal.

>[!NOTE]
>
>Los vídeos dinámicos no son compatibles con los inquilinos de Brand Portal integrados con AEM Author que se ejecutan en [!UICONTROL el modo de ejecución de Scene 7 Connect] .

## ¿Cómo se reproducen los vídeos dinámicos? {#how-are-dynamic-videos-played}

![Se recuperan codificaciones de vídeo desde la nube](assets/VideoEncodes.png)

Si las configuraciones de Dynamic Media ([híbrido](../using/dynamic-video-brand-portal.md#configure-dm-hybrid-settings) o [[! Las configuraciones DNL Scene 7)](../using/dynamic-video-brand-portal.md#configure-dm-scene7-settings) se configuran en Brand Portal, las representaciones dinámicas se obtienen del [!DNL Scene 7] servidor. Por lo tanto, las codificaciones de vídeo se previsualizan y se reproducen sin retraso y distorsión en calidad.

Dado que las codificaciones de vídeo no se almacenan en repositorio de Brand Portal y se extraen del [!DNL Scene 7] servidor, asegúrese de que las configuraciones de Dynamic Media en AEM Author Instance y Brand Portal son las mismas.

>[!NOTE]
>
>Los visores de vídeos y los ajustes preestablecidos de visor no son compatibles con Brand Portal. Los vídeos se previsualizan y se reproducen en los visores predeterminados de Brand Portal.

## Requisitos previos {#prerequisites}

Para trabajar con vídeos dinámicos en Brand Portal, asegúrese de:

* **Inicie el modo AEM Author en el modo
DM (Dynamic Media)** Start up the AEM Author instance (con which Brand Portal está integrado) en [el modo Dynamic Media Híbrido](https://helpx.adobe.com/experience-manager/6-5/assets/using/config-dynamic.html#EnablingDynamicMedia) o [Dynamic Media [! Modo DNL Scene 7]](https://helpx.adobe.com/experience-manager/6-5/assets/using/config-dms7.html#EnablingDynamicMediainScene7mode).
* **Configure los servicios de nube de Dynamic Media en AEM Author**
según el modo de Dynamic Media en el que se ejecute el autor de AEM Author, establezca los servicios de nube [de Dynamic Media](https://helpx.adobe.com/experience-manager/6-5/assets/using/config-dynamic.html#ConfiguringDynamicMediaCloudServices) o [[! Servicios de nube DNL Scene 7](https://helpx.adobe.com/experience-manager/6-5/assets/using/config-dms7.html#ConfiguringDynamicMediaCloudServices) en AEM Author desde **Herramientas** | **Servicios de nube** | **Dynamic Media**.
* **Configure Dynamic Media en el portal
de marca** basado en las configuraciones de nube de Dynamic Media en AEM Author, configure [la configuración de Dynamic Media](#configure-dm-hybrid-settings) o [[! Configuración DNL Scene 7](#configure-dm-scene7-settings) de las herramientas administrativas de Brand Portal.
Asegúrese de [que los inquilinos de Brand Portal independientes](#separate-tenants) se utilicen para las instancias de AEM Author configuradas con los modos Dynamic Media Híbrido y Dynamic Media [!UICONTROL Scene 7] , si utiliza funcionalidades de Dynamic Media Híbrido y Dynamic Media [!UICONTROL S 7].
* **Publique carpetas con codificaciones de vídeo aplicadas a Brand Portal**
Aplicación [de codificaciones](https://helpx.adobe.com/experience-manager/6-5/assets/using/video-profiles.html) de vídeo y publique la carpeta que contenga recursos de medios enriquecidos de la instancia de AEM Author a Brand Portal.
* **Lista blanca de Egress en SPS si se habilita
la vista previa segura** Si se utiliza Dynamic Media ([!DNL Scene 7] con [la vista previa segura habilitada](https://docs.adobe.com/content/help/en/dynamic-media-classic/using/upload-publish/testing-assets-making-them-public.html) para una empresa), se aconseja a los [!DNL Scene 7] administradores [de la empresa que agreguen las direcciones IP](https://docs.adobe.com/content/help/en/dynamic-media-classic/using/upload-publish/testing-assets-making-them-public.html#testing-the-secure-testing-service) públicas de las regiones correspondientes utilizando la IU Flash de SPS ([!UICONTROL Scene 7] Publishing System).
Las IP de Egress son las siguientes:

| **Región** | **IP de Egress** |
|--- |--- |
| ND | 192.243.237.86 |
| EMEA | 185.34.189.4 |
| APAC | 63.140.44.54 |

Para incluir cualquiera de estas IP de favoritos, consulte [preparación de su cuenta para servicios de prueba seguros](https://docs.adobe.com/content/help/en/dynamic-media-classic/using/upload-publish/testing-assets-making-them-public.html#testing-the-secure-testing-service).

## Prácticas recomendadas

Para asegurarse de que los recursos de vídeo dinámicos se previsualizan, reproducen y descarguen de Brand Portal (y vínculos compartidos), siga estas prácticas:

### Inquilinos independientes para los modos Híbridos de Dynamic Media y Dynamic Media Scene 7 {#separate-tenants}

Si utiliza funciones híbridas de Dynamic Media [!DNL Scene 7] y Dynamic Media, es aconsejable utilizar distintos inquilinos de Brand Portal para las instancias de AEM Author configuradas con [!DNL Scene 7] los modos Dynamic Media Híbrido y Dynamic Media.
![Autor y BP de una a una asignación](assets/BPDynamicMedia.png)

### Los mismos detalles de configuración en la instancia de AEM Author y Brand Portal

Asegúrese de que los detalles de configuración, como [!UICONTROL Título], [!UICONTROL ID de registro], [!UICONTROL URL del servicio de vídeo] (en [!UICONTROL Dynamic Media Híbrido]) y [!UICONTROL Título], las credenciales ([!UICONTROL Correo electrónico] y Contraseña), [!UICONTROL Región], [!UICONTROL Empresa] (en Dynamic Media [!DNL Scene 7]), son los mismos en Brand Portal y [!UICONTROL en la configuración de nube de AEM].

### Lista de direcciones IP públicas para el modo Scene 7 de Dynamic Media

Si Dynamic Media [!UICONTROL Scene 7]-tiene [una vista previa segura habilitada](https://docs.adobe.com/content/help/en/dynamic-media-classic/using/upload-publish/testing-assets-making-them-public.html)para ofrecer recursos de vídeo a Brand Portal, [!UICONTROL Scene 7] establece un servidor de imágenes dedicado para entornos de ensayo o aplicaciones internas. Cualquier solicitud a este servidor comprueba la dirección IP de origen. Si la solicitud entrante no está dentro de la lista aprobada de direcciones IP, se devuelve una respuesta de error.
Por [!UICONTROL lo tanto, el administrador de Scene -7] configura una lista aprobada de direcciones IP para el entorno [!UICONTROL Secure Testing] de su empresa, a través de la interfaz de usuario de [!UICONTROL SPS] (Scene -7 Publishing System). Asegúrese de que la IP de la cookie para su región respectiva (de lo siguiente) se añada a esa lista aprobada.
Para incluir cualquiera de estas IP de favoritos, consulte [preparación de su cuenta para servicios de prueba seguros](https://docs.adobe.com/content/help/en/dynamic-media-classic/using/upload-publish/testing-assets-making-them-public.html#testing-the-secure-testing-service).
Las IP de la edición son las siguientes:

| **Región** | **IP de Egress** |
|--- |--- |
| ND | 192.243.237.86 |
| EMEA | 185.34.189.4 |
| APAC | 63.140.44.54 |

## Configuración de la configuración de Dynamic Media (Híbrido) {#configure-dm-hybrid-settings}

Si la instancia de AEM Author se ejecuta en modo híbrido Dynamic Media, utilice el mosaico [!UICONTROL de vídeo] de panel de herramientas administrativas para configurar la configuración de puerta de enlace de Dynamic Media.
>[!NOTE]
>
>Los perfiles de codificación [de vídeo](https://helpx.adobe.com/experience-manager/6-5/assets/using/video-profiles.html) no se publican en Brand Portal, sino que se obtienen del servidor [!UICONTROL de Scene 7] . Por lo tanto, para que los codificaciones de vídeo se reproduzcan correctamente en Brand Portal, asegúrese de que los detalles de configuración sean los mismos que [[! Configuración de nube UICONTROL Scene 7](https://helpx.adobe.com/experience-manager/6-5/assets/using/config-dms7.html#ConfiguringDynamicMediaCloudServices) en su instancia de AEM Author.
Para configurar las configuraciones de Dynamic Media en inquilinos de Brand Portal:

1. Seleccione el logotipo de AEM para acceder a las herramientas administrativas desde la barra de herramientas de la parte superior, en Brand Portal.

2. En el panel de herramientas administrativas, seleccione el mosaico **[!UICONTROL Vídeo]** .<br />
   ![Configuración híbrida de Dynamic Media en Brand Portal](assets/DMHybrid-Video.png)
   **[!UICONTROL Se abre la página Editar configuración]** de Dynamic Media.<br />
   ![Configuración híbrida de Dynamic Media en Brand Portal](assets/edit-dynamic-media-config.png)

3. Especifique **[!UICONTROL la ID de registro]** y la URL del servicio **[!UICONTROL de vídeo]** (URL de puerta de enlace DM-Gateway). Asegúrese de que estos detalles son los mismos que los de **[!UICONTROL Herramientas &gt; Cloud Services]** en su instancia de AEM Author.

4. Seleccione **Guardar** para guardar la configuración.

## Configuración de la configuración de Scene 7 de Dynamic Media {#configure-dm-scene7-settings}

Si la instancia de AEM Author se ejecuta en el modo Dynamic Media- [!UICONTROL Scene 7] , utilice **[!UICONTROL el mosaico de configuración]** de Dynamic Media desde el panel de herramientas administrativas para configurar los ajustes del servidor [!UICONTROL de Scene 7] .

Para configurar las configuraciones [!UICONTROL de Scene 7] Scene 7 en inquilinos de Brand Portal:

1. Seleccione el logotipo de AEM para acceder a las herramientas administrativas desde la barra de herramientas de la parte superior, en Brand Portal.

2. En el panel de herramientas administrativas, seleccione **[!UICONTROL el mosaico Configuración]** de Dynamic Media.<br />
   ![Configuración de Scene [!UICONTROL 7] en Brand Portal](assets/DMS7-Tile.png)
   [!UICONTROL Se abre la página Editar configuración] de Dynamic Media.<br />
   ![Configuración de Scene 7 en Brand Portal](assets/S7Config.png)

3. Proporcionar:
   * [!UICONTROL Título]
   * Credenciales ([!UICONTROL ID de correo electrónico] y [!UICONTROL contraseña]) para acceder al servidor de Scene 7
   * [!UICONTROL Región]
Asegúrese de que estos valores sean los mismos que los de su instancia de AEM Author.

4. Select **[!UICONTROL Connect to Dynamic Media]**.

5. Proporcione el nombre **[!UICONTROL de Empresa]** y **[!UICONTROL guarde]** la configuración.
