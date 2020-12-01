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
source-git-commit: b41f86824afd5be043c7b91035b01b71fdb69a26
workflow-type: tm+mt
source-wordcount: '1207'
ht-degree: 3%

---


# Compatibilidad con vídeos dinámicos en Brand Portal {#dynamic-video-support-on-brand-portal}

Previsualización y reproducción de vídeos de forma adaptable en Brand Portal con compatibilidad con Dynamic Media. Descargue también las representaciones dinámicas desde el portal y los vínculos compartidos.
Los usuarios de Brand Portal pueden:

* Vídeos de previsualización en la página Detalles del recurso, Vista de tarjetas y página de previsualización de uso compartido de vínculos.
* Reproducir codificaciones de vídeo en la página Detalles del recurso.
* Vista las representaciones dinámicas en la ficha Representaciones de la página Detalles del recurso.
* Descargue codificaciones de vídeo y carpetas que contengan vídeos.

>[!NOTE]
>
>Para trabajar con vídeos y publicarlos en Brand Portal, asegúrese de que la instancia de AEM Author está configurada en el modo Dynamic Media Hybrid o en el modo Dynamic Media **[!DNL Scene 7]**.

Para la previsualización, reproducción y descarga de vídeos, Brand Portal expone las dos configuraciones siguientes a los administradores:

* [Configuración híbrida de Dynamic Media ](#configure-dm-hybrid-settings)
Si la instancia de AEM Author se está ejecutando en modo híbrido de Dynamic Media.
* [Mediaconfiguración dinámica  [!DNL Scene 7] ](#configure-dm-scene7-settings)
Si la instancia de AEM Author se está ejecutando en **[!DNL Scene 7]** modo de medios dinámicos.
Configure cualquiera de estas configuraciones en función de las configuraciones que defina en la instancia de AEM Author con la que se replique el inquilino de Brand Portal.

>[!NOTE]
>
>Los vídeos dinámicos no son compatibles con los inquilinos de Brand Portal configurados con AEM Author que se ejecutan en el modo de ejecución **[!UICONTROL Scene7Connect]**.

## ¿Cómo se reproducen los vídeos dinámicos? {#how-are-dynamic-videos-played}

![Las codificaciones de vídeo se obtienen de la nube](assets/VideoEncodes.png)

Si las configuraciones de Dynamic Media ([Hybrid](../using/dynamic-video-brand-portal.md#configure-dm-hybrid-settings) o [[!DNL Scene 7]](../using/dynamic-video-brand-portal.md#configure-dm-scene7-settings)) están configuradas en Brand Portal, las representaciones dinámicas se recuperan del servidor **[!DNL Scene 7]**. Por lo tanto, las codificaciones de vídeo se previsualizan y reproducen sin demora y con distorsión de la calidad.

Dado que las codificaciones de vídeo no se almacenan en el repositorio de Brand Portal y se recuperan del servidor **[!DNL Scene 7]**, asegúrese de que las configuraciones de Dynamic Media en la instancia de AEM Author y en Brand Portal sean las mismas.

>[!NOTE]
>
>Los visores de vídeo y los ajustes preestablecidos de visor no son compatibles con Brand Portal. Los vídeos se previsualizan y se reproducen en los visores predeterminados de Brand Portal.

## Requisitos previos {#prerequisites}

Para trabajar con vídeos dinámicos en Brand Portal, asegúrese de:

* **Inicio de AEM Author en el**
modo DM (Dynamic Media)Inicie la instancia de AEM Author (con la que se ha configurado Brand Portal) en  [Dynamic Media Hybrid ](https://helpx.adobe.com/experience-manager/6-5/assets/using/config-dynamic.html#EnablingDynamicMedia) Modo o en  [Dynamic  [!DNL Scene 7] Media](https://helpx.adobe.com/experience-manager/6-5/assets/using/config-dms7.html#EnablingDynamicMediainScene7mode).
* **Configuración de servicios de nube de Dynamic Media en AEM**
AutorBasado en el modo de Dynamic Media en el que AEM Author se está ejecutando, establezca los servicios de nube de  [Dynamic Media o los servicios de ](https://helpx.adobe.com/experience-manager/6-5/assets/using/config-dynamic.html#ConfiguringDynamicMediaCloudServices) nube  [[!DNL Scene 7] en AEM Author desde ](https://helpx.adobe.com/experience-manager/6-5/assets/using/config-dms7.html#ConfiguringDynamicMediaCloudServices) Herramientas **|** Cloud Services **| Medios**   **** dinámicos.
* **Configuración de Dynamic Media en Brand**
PortalEn función de las configuraciones de Dynamic Media Cloud en AEM Author, configure  [Dynamic Media ](#configure-dm-hybrid-settings) o  [[!DNL Scene 7] ](#configure-dm-scene7-settings)  configure desde las herramientas administrativas de Brand Portal.
Asegúrese de que [los inquilinos de Brand Portal independientes](#separate-tenants) se utilizan para instancias de AEM Author configuradas con los modos Dynamic Media Hybrid y Dynamic Media **[!UICONTROL Scene7]**, si utiliza funcionalidades de Dynamic Media Hybrid y Dynamic Media **[!UICONTROL S7]**.
* **Publicar carpetas con codificaciones de vídeo aplicadas a Brand**
PortalAplicar codificaciones de  [ ](https://helpx.adobe.com/experience-manager/6-5/assets/using/video-profiles.html) vídeo y publicar la carpeta que contiene recursos de medios enriquecidos de la instancia de AEM Author en Brand Portal.
* **IP de salida de lista de permitidos en SPS si la previsualización segura**
está habilitadaSi se utiliza Dynamic Media-**[!DNL Scene 7]** (con previsualización  [segura ](https://docs.adobe.com/content/help/en/dynamic-media-classic/using/upload-publish/testing-assets-making-them-public.html) habilitada para una compañía), se aconseja que el administrador de  **[!DNL Scene 7]** compañía  [lista de permitidos las ](https://docs.adobe.com/content/help/en/dynamic-media-classic/using/upload-publish/testing-assets-making-them-public.html#testing-the-secure-testing-service) IP de salida pública para las regiones respectivas mediante la interfaz de usuario flash de SPS (**[!UICONTROL Scene 7]** Publishing System).
Las direcciones IP de salida son las siguientes:

| **Región** | **IP de salida** |
|--- |--- |
| ND | 192 243 237 86 |
| EMEA | 185,34,189,4 |
| APAC | 63 140 44 54 |

Para permitir cualquiera de estas direcciones IP de salida, consulte [prepare su cuenta para el servicio de pruebas seguras](https://docs.adobe.com/content/help/en/dynamic-media-classic/using/upload-publish/testing-assets-making-them-public.html#testing-the-secure-testing-service).

## Prácticas recomendadas  

Para asegurarse de que los recursos de vídeo dinámicos se previsualizan, reproducen y descargan correctamente desde Brand Portal (y vínculos compartidos), siga estas prácticas:

### Inquilinos separados para los modos Dynamic Media Hybrid y Dynamic Media Scene7 {#separate-tenants}

Si está utilizando las funciones Dynamic Media **[!DNL Scene 7]** y Dynamic Media Hybrid, se recomienda usar diferentes inquilinos de Brand Portal para instancias de AEM Author configuradas con Dynamic Media Hybrid y Dynamic Media **[!DNL Scene 7]** modos.<br />

![Asignación de uno a uno de Autor y BP](assets/BPDynamicMedia.png)

### Los mismos detalles de configuración en la instancia de AEM Author y en Brand Portal

Asegúrese de que los detalles de configuración, como **[!UICONTROL Título]**, **[!UICONTROL Id. de registro]**, **[!UICONTROL URL del servicio de vídeo]** (en **[!UICONTROL Dynamic Media Hybrid]**) y **[!UICONTROL Título]**, credenciales (**[!UICONTROL Correo electrónico]** y contraseña), a12/>Región ]**,**[!UICONTROL  Compañía ]**(en Dynamic Media **[!DNL Scene 7]**) son iguales en Brand Portal y**[!UICONTROL  configuración de nube AEM ]**.**[!UICONTROL 

### IP de salida pública de lista de permitidos para el modo de Dynamic Media Scene 7

Si se utiliza Dynamic Media **[!UICONTROL Scene 7]**, con [previsualización segura habilitada](https://docs.adobe.com/content/help/en/dynamic-media-classic/using/upload-publish/testing-assets-making-them-public.html), para proporcionar recursos de vídeo a Brand Portal, **[!UICONTROL Scene 7]** establece un servidor de imágenes dedicado para entornos de ensayo o aplicaciones internas. Cualquier solicitud a este servidor comprueba la dirección IP del origen. Si la solicitud entrante no está dentro de la lista aprobada de direcciones IP, se devuelve una respuesta de error.
Por lo tanto, el administrador de Compañía **[!UICONTROL Scene-7]** configura una lista aprobada de direcciones IP para el entorno **[!UICONTROL Secure Testing]** de su compañía mediante la interfaz de usuario flash **[!UICONTROL SPS]** (Scene-7 Publishing System). Asegúrese de que la dirección IP de salida de su región respectiva (de lo siguiente) se agrega a esa lista aprobada.
Para permitir cualquiera de estas direcciones IP de salida, consulte [prepare su cuenta para el servicio de pruebas seguras](https://docs.adobe.com/content/help/en/dynamic-media-classic/using/upload-publish/testing-assets-making-them-public.html#testing-the-secure-testing-service).
Las direcciones IP de salida son las siguientes:

| **Región** | **IP de salida** |
|--- |--- |
| ND | 192 243 237 86 |
| EMEA | 185,34,189,4 |
| APAC | 63 140 44 54 |

## Configuración de la configuración de Dynamic Media (híbrido) {#configure-dm-hybrid-settings}

Si la instancia de AEM Author se está ejecutando en modo híbrido de Dynamic Media, utilice **[!UICONTROL mosaico de vídeo]** del panel Herramientas administrativas para configurar la puerta de enlace de Dynamic Media.

>[!NOTE]
>
>Los [perfiles de codificación de vídeo](https://helpx.adobe.com/experience-manager/6-5/assets/using/video-profiles.html) no se publican en Brand Portal, sino que se recuperan del servidor **[!UICONTROL Scene 7]**. Por lo tanto, para que las codificaciones de vídeo se reproduzcan correctamente en Brand Portal, asegúrese de que los detalles de configuración sean los mismos que la [[!UICONTROL configuración de nube de Scene7]](https://helpx.adobe.com/experience-manager/6-5/assets/using/config-dms7.html#ConfiguringDynamicMediaCloudServices) en la instancia de AEM Author.

Para configurar las opciones de Dynamic Media en los inquilinos de Brand Portal:

1. Seleccione el logotipo de AEM para acceder a las herramientas administrativas desde la barra de herramientas situada en la parte superior, en Brand Portal.
1. En el panel Herramientas administrativas, seleccione el mosaico **[!UICONTROL Video]**.

   ![Configuración híbrida de Dynamic Media en Brand Portal](assets/DMHybrid-Video.png)

   **[!UICONTROL Se abre la página Editar]** configuración de Dynamic Media.

   ![Configuración híbrida de Dynamic Media en Brand Portal](assets/edit-dynamic-media-config.png)

1. Especifique **[!UICONTROL ID de registro]** y **[!UICONTROL URL del servicio de vídeo]** (URL de DM-Gateway). Asegúrese de que estos detalles son los mismos que los de **[!UICONTROL Herramientas > Cloud Services]** en la instancia de AEM Author.
1. Seleccione **Guardar** para guardar la configuración.

## Configuración de la configuración de Dynamic Media para Scene7 {#configure-dm-scene7-settings}

Si la instancia de AEM Author se está ejecutando en el modo Dynamic Media: **[!UICONTROL Scene 7]**, utilice el mosaico **[!UICONTROL Configuración de Dynamic Media]** del panel Herramientas administrativas para configurar la configuración del servidor de **[!UICONTROL Scene 7]**.

Para configurar las configuraciones de Dynamic Media **[!UICONTROL Scene 7]** en los inquilinos de Brand Portal:

1. Seleccione el logotipo de AEM para acceder a las herramientas administrativas desde la barra de herramientas situada en la parte superior, en Brand Portal.

2. En el panel Herramientas administrativas, seleccione el mosaico **[!UICONTROL Configuración de Dynamic Media]**.<br />
   ![Configuración de DM  [!UICONTROL Scene 7] en Brand Portal](assets/DMS7-Tile.png)
   **[!UICONTROL Se abre la página Editar]** configuración de Dynamic Media.<br />
   ![Configuración de Scene7 en Brand Portal](assets/S7Config.png)

3. Proporcione:
   * **[!UICONTROL Título]**
   * Credenciales (**[!UICONTROL ID de correo electrónico]** y **[!UICONTROL Contraseña]**) para acceder al servidor de Scene7
   * ****
RegiónAsegúrese de que estos valores son los mismos que los de la instancia de AEM Author.

4. Seleccione **[!UICONTROL Conectar a Dynamic Media]**.

5. Proporcione el **[!UICONTROL nombre de Compañía]** y **[!UICONTROL Guardar]** la configuración.
