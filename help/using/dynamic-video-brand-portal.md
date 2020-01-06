---
title: Compatibilidad con vídeos dinámicos en Brand Portal
seo-title: Compatibilidad con vídeos dinámicos en Brand Portal
description: Compatibilidad con vídeos dinámicos en Brand Portal
seo-description: Compatibilidad con vídeos dinámicos en Brand Portal
uuid: a3502a4d-3971-4ea4-953c-44ba04446269
contentOwner: mgulati
products: SG_EXPERIENCEMANAGER/Brand_Portal
content-type: reference
topic-tags: download-install
discoiquuid: e18d992a-a3b5-45f2-9696-8161993213ee
translation-type: tm+mt
source-git-commit: 86078dd07b5d487f8cf5cd08bc46e4745529c873

---


# Compatibilidad con vídeos dinámicos en Brand Portal {#dynamic-video-support-on-brand-portal}

Obtenga una vista previa y reproduzca vídeos de forma adaptable en Brand Portal con compatibilidad con Dynamic Media. Descargue también las representaciones dinámicas desde el portal y los vínculos compartidos.
Los usuarios de Brand Portal pueden:

* Obtenga una vista previa de los vídeos en la página Detalles del recurso, en la vista de tarjeta y en la página de vista previa del uso compartido de vínculos.
* Reproducir codificaciones de vídeo en la página Detalles del recurso.
* Vea las representaciones dinámicas en la ficha Representaciones de la página Detalles del recurso.
* Descargue codificaciones de vídeo y carpetas que contengan vídeos.

>[!NOTE]
>
>Para trabajar con vídeos y publicarlos en Brand Portal, asegúrese de que la instancia de AEM Author está configurada en el modo Dynamic Media Hybrid o en el **[!DNL Scene 7]**modo Dynamic Media.

Para obtener una vista previa, reproducir y descargar vídeos, Brand Portal expone las dos configuraciones siguientes a los administradores:

* [Configuración](#configure-dm-hybrid-settings)híbrida de Dynamic Media Si la instancia de AEM Author se está ejecutando en modo híbrido de Dynamic Media.
* [Configuración](#configure-dm-scene7-settings)de Dynamic Media [!DNL Scene 7] Si la instancia de AEM Author se está ejecutando en modo Dynamic Media-**[!DNL Scene 7]**.
Configure cualquiera de estas configuraciones en función de las configuraciones que defina en la instancia de AEM Author con la que se replique el inquilino de Brand Portal.

>[!NOTE]
>
>Los vídeos dinámicos no son compatibles con los inquilinos de Brand Portal integrados con AEM Author que se ejecutan en el modo de ejecución de **[!UICONTROL Scene7 Connect]**.

## ¿Cómo se reproducen los vídeos dinámicos? {#how-are-dynamic-videos-played}

![Las codificaciones de vídeo se obtienen de la nube](assets/VideoEncodes.png)

Si las configuraciones de Dynamic Media (configuraciones[híbridas](../using/dynamic-video-brand-portal.md#configure-dm-hybrid-settings) o [[!DNL Scene7]](../using/dynamic-video-brand-portal.md#configure-dm-scene7-settings) ) están configuradas en Brand Portal, las representaciones dinámicas se recuperan del **[!DNL Scene 7]**servidor. Por lo tanto, las codificaciones de vídeo se previsualizan y reproducen sin demora y con distorsión de la calidad.

Dado que las codificaciones de vídeo no se almacenan en el repositorio de Brand Portal y se recuperan del **[!DNL Scene 7]**servidor, asegúrese de que las configuraciones de Dynamic Media en la instancia de AEM Author y en Brand Portal sean las mismas.

>[!NOTE]
>
>Los visores de vídeo y los ajustes preestablecidos de visor no son compatibles con Brand Portal. Los vídeos se previsualizan y se reproducen en los visores predeterminados de Brand Portal.

## Requisitos previos {#prerequisites}

Para trabajar con vídeos dinámicos en Brand Portal, asegúrese de:

* **Iniciar AEM Author en modo** DM (Dynamic Media) Inicie la instancia de AEM Author (con la que Brand Portal está integrado) en modo [híbrido](https://helpx.adobe.com/experience-manager/6-5/assets/using/config-dynamic.html#EnablingDynamicMedia) Dynamic Media o en modo [](https://helpx.adobe.com/experience-manager/6-5/assets/using/config-dms7.html#EnablingDynamicMediainScene7mode)Dynamic Media [!DNL Scene 7].
* **Configuración de servicios de nube de Dynamic Media en AEM Author** Basado en el modo de Dynamic Media en el que AEM Author se está ejecutando, se establece en los servicios [de nube de](https://helpx.adobe.com/experience-manager/6-5/assets/using/config-dynamic.html#ConfiguringDynamicMediaCloudServices) Dynamic Media o en los servicios [de nube](https://helpx.adobe.com/experience-manager/6-5/assets/using/config-dms7.html#ConfiguringDynamicMediaCloudServices) [!DNL Scene 7] en AEM Author desde **Herramientas** | **Cloud Services** | Medios **dinámicos**.
* **Configure Dynamic Media en Brand Portal** En función de las configuraciones de Dynamic Media Cloud en AEM Author, configure los ajustes [de](#configure-dm-hybrid-settings) Dynamic Media o los ajustes [](#configure-dm-scene7-settings) [!DNL Scene 7] de las herramientas administrativas de Brand Portal.
Asegúrese de que los inquilinos [](#separate-tenants) independientes de Brand Portal se utilizan para instancias de AEM Author configuradas con los modos Dynamic Media Hybrid y Dynamic Media **[!UICONTROL Scene7]**, si utiliza funcionalidades de Dynamic Media Hybrid y Dynamic Media**[!UICONTROL  S7]**.
* **Publicar carpetas con codificaciones de vídeo aplicadas a Brand Portal** Aplicar codificaciones [de](https://helpx.adobe.com/experience-manager/6-5/assets/using/video-profiles.html) vídeo y publicar la carpeta que contiene recursos de medios enriquecidos de la instancia de AEM Author en Brand Portal.
* **Lista blanca de direcciones IP de salida en SPS si la vista previa segura está habilitada**. Si se utiliza Dynamic Media-**[!DNL Scene 7]**(con la vista previa[segura habilitada](https://docs.adobe.com/content/help/en/dynamic-media-classic/using/upload-publish/testing-assets-making-them-public.html)para una empresa), se aconseja que**[!DNL Scene 7]** el administrador de la empresa [incluya en la lista blanca las direcciones IP](https://docs.adobe.com/content/help/en/dynamic-media-classic/using/upload-publish/testing-assets-making-them-public.html#testing-the-secure-testing-service) de salida públicas para las regiones respectivas mediante la interfaz de usuario flash de SPS (**[!UICONTROL Scene 7]**Publishing System).
Las direcciones IP de salida son las siguientes:

| **Región** | **IP de salida** |
|--- |--- |
| ND | 192.243.237.86 |
| EMEA | 185.34.189.4 |
| APAC | 63.140.44.54 |

Para incluir cualquiera de estas direcciones IP de salida en la lista blanca, consulte [Preparación de la cuenta para el servicio](https://docs.adobe.com/content/help/en/dynamic-media-classic/using/upload-publish/testing-assets-making-them-public.html#testing-the-secure-testing-service)de prueba segura.

## Prácticas recomendadas

Para asegurarse de que los recursos de vídeo dinámicos se previsualizan, reproducen y descargan correctamente desde Brand Portal (y vínculos compartidos), siga estas prácticas:

### Inquilinos independientes para los modos Dynamic Media híbrido y Dynamic Media Scene7 {#separate-tenants}

Si utiliza funciones tanto de Dynamic Media **[!DNL Scene 7]**como de Dynamic Media Hybrid, se aconseja utilizar distintos inquilinos de Brand Portal para instancias de AEM Author configuradas con los modos Dynamic Media Hybrid y Dynamic Media**[!DNL Scene 7]** .<br />

![Asignación de uno a uno de Autor y BP](assets/BPDynamicMedia.png)

### Los mismos detalles de configuración en la instancia de AEM Author y en Brand Portal

Asegúrese de que los detalles de configuración, tales como **[!UICONTROL Título]**, Id****de registro, URL **[!UICONTROL del servicio de]**vídeo (en**[!UICONTROL  Dynamic Media Hybrid]**) y **[!UICONTROL Título]****** ******** **[!DNL Scene 7]******, credenciales (Correo electrónico y contraseña), Región, Compañía(en Dynamic Media)-sean los mismos en Brand Portal y en la configuración de la nube AEMniv.

### Lista blanca de direcciones IP de salida pública para el modo de Dynamic Media Scene7

Si **[!UICONTROL Scene7]**de Dynamic Media tiene habilitada[la vista previa](https://docs.adobe.com/content/help/en/dynamic-media-classic/using/upload-publish/testing-assets-making-them-public.html)segura para ofrecer recursos de vídeo a Brand Portal,**[!UICONTROL  Scene 7]** establece un servidor de imágenes dedicado para entornos de ensayo o aplicaciones internas. Cualquier solicitud a este servidor comprueba la dirección IP de origen. Si la solicitud entrante no está dentro de la lista aprobada de direcciones IP, se devuelve una respuesta de error.
Por lo tanto, el administrador de la empresa de **[!UICONTROL Scene-7]**configura una lista aprobada de direcciones IP para el entorno de prueba**** segura de su empresa mediante la interfaz de usuario flash de **[!UICONTROL SPS]**(Scene-7 Publishing System). Asegúrese de que la dirección IP de salida de su región respectiva (de la siguiente) se agrega a esa lista aprobada.
Para incluir cualquiera de estas direcciones IP de salida en la lista blanca, consulte[Preparación de la cuenta para el servicio](https://docs.adobe.com/content/help/en/dynamic-media-classic/using/upload-publish/testing-assets-making-them-public.html#testing-the-secure-testing-service)de prueba segura.
Las direcciones IP de salida son las siguientes:

| **Región** | **IP de salida** |
|--- |--- |
| ND | 192.243.237.86 |
| EMEA | 185.34.189.4 |
| APAC | 63.140.44.54 |

## Configuración de la configuración de Dynamic Media (híbrido) {#configure-dm-hybrid-settings}

Si la instancia de AEM Author se está ejecutando en modo híbrido de Dynamic Media, utilice el mosaico **[!UICONTROL Vídeo]**del panel Herramientas administrativas para configurar la puerta de enlace de Dynamic Media.
>[!NOTE]
>
>Los perfiles [de codificación de](https://helpx.adobe.com/experience-manager/6-5/assets/using/video-profiles.html) vídeo no se publican en Brand Portal, sino que se recuperan del servidor de **[!UICONTROL Scene 7]**. Por lo tanto, para que las codificaciones de vídeo se reproduzcan correctamente en Brand Portal, asegúrese de que los detalles de configuración son los mismos que los de la configuración[[!UICONTROL de nube de]](https://helpx.adobe.com/experience-manager/6-5/assets/using/config-dms7.html#ConfiguringDynamicMediaCloudServices)Scene7 en la instancia de AEM Author.
Para configurar las opciones de Dynamic Media en los inquilinos de Brand Portal:

1. Seleccione el logotipo de AEM para acceder a las herramientas administrativas desde la barra de herramientas situada en la parte superior, en Brand Portal.

2. En el panel Herramientas administrativas, seleccione el mosaico **[!UICONTROL Vídeo]**.<br />   ![Configuración híbrida de Dynamic Media en Brand Portal](assets/DMHybrid-Video.png)
   **[!UICONTROL Se abre la página Editar configuración]**de Dynamic Media.<br />   ![Configuración híbrida de Dynamic Media en Brand Portal](assets/edit-dynamic-media-config.png)

3. Especifique el ID ****de registro y la URL**[!UICONTROL  del servicio]** de vídeo (URL de DM-Gateway). Asegúrese de que estos detalles son los mismos que los de **[!UICONTROL Herramientas > Servicios]**de nube en la instancia de AEM Author.

4. Seleccione **Guardar** para guardar la configuración.

## Configuración de los ajustes de Dynamic Media Scene7 {#configure-dm-scene7-settings}

Si la instancia de AEM Author se está ejecutando en el modo Dynamic Media: **[!UICONTROL Scene 7]**, utilice el mosaico Configuración**[!UICONTROL  de medios]** dinámicos del panel Herramientas administrativas para configurar la configuración del servidor de **[!UICONTROL Scene7]**.

Para configurar las configuraciones de Dynamic Media **[!UICONTROL Scene 7]**en los inquilinos de Brand Portal:

1. Seleccione el logotipo de AEM para acceder a las herramientas administrativas desde la barra de herramientas situada en la parte superior, en Brand Portal.

2. En el panel Herramientas administrativas, seleccione el mosaico Configuración **[!UICONTROL de medios]**dinámicos.<br />   ![Configuración de DM [!UICONTROL Scene 7] en Brand Portal](assets/DMS7-Tile.png)
   **[!UICONTROL Se abre la página Editar configuración]**de Dynamic Media.<br />   ![Configuración de Scene7 en Brand Portal](assets/S7Config.png)

3. Proporcione:
   * **[!UICONTROL Título]**
   * Credenciales (ID **[!UICONTROL de]**correo electrónico y**[!UICONTROL  contraseña]**) para acceder al servidor de Scene 7
   * **[!UICONTROL Región]**Asegúrese de que estos valores son los mismos que los de la instancia de AEM Author.

4. Select **[!UICONTROL Connect to Dynamic Media]**.

5. Proporcione el nombre **[!UICONTROL de la]**empresa y**[!UICONTROL  guarde]** la configuración.
