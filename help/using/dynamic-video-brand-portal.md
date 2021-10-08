---
title: Compatibilidad con vídeos dinámicos en Brand Portal
seo-title: Dynamic video support on Brand Portal
description: Compatibilidad con vídeos dinámicos en Brand Portal
seo-description: Dynamic video support on Brand Portal
uuid: a3502a4d-3971-4ea4-953c-44ba04446269
contentOwner: mgulati
products: SG_EXPERIENCEMANAGER/Brand_Portal
content-type: reference
topic-tags: download-install
discoiquuid: e18d992a-a3b5-45f2-9696-8161993213ee
exl-id: 08d6a0fb-061e-4bef-b8e2-bb8522e7482e
source-git-commit: e970775efa611357378516119077a3bfd52b124f
workflow-type: tm+mt
source-wordcount: '1191'
ht-degree: 2%

---

# Compatibilidad con vídeos dinámicos en Brand Portal {#dynamic-video-support-on-brand-portal}

Previsualice y reproduzca vídeos de forma adaptable en Brand Portal con compatibilidad con Dynamic Media. Descargue también las representaciones dinámicas desde el portal y los vínculos compartidos.
Los usuarios de Brand Portal pueden:

* Obtenga una vista previa de los vídeos en la página Detalles del recurso, la vista de tarjeta y la página de vista previa del uso compartido de vínculos.
* Reproducir las codificaciones de vídeo en la página Detalles del recurso .
* Vea las representaciones dinámicas en la pestaña Representaciones de la página Detalles del recurso .
* Descargue codificaciones de vídeo y carpetas que contengan vídeos.

>[!NOTE]
>
>Para trabajar con vídeos y publicarlos en Brand Portal, asegúrese de que la instancia de Autor Experience Manager esté configurada en el modo Híbrido de Dynamic Media o en el modo **[!DNL Scene 7]** de Dynamic Media.

Para obtener una vista previa, reproducir y descargar vídeos, Brand Portal expone las dos configuraciones siguientes a los administradores:

* [Configuración híbrida de Dynamic Media](#configure-dm-hybrid-settings)
Si la instancia de Autor de Experience Manager se está ejecutando en el modo híbrido de Dynamic Media.
* [Dynamic  [!DNL Scene 7] ](#configure-dm-scene7-settings)
MediaconfigurationSi la instancia de Autor de Experience Manager se está ejecutando en **[!DNL Scene 7]** modo de Dynamic Media.
Establezca cualquiera de estas configuraciones en función de las configuraciones establecidas en la instancia de Autor de Experience Manager con la que se replica el inquilino de Brand Portal.

>[!NOTE]
>
>Los vídeos dinámicos no son compatibles con los inquilinos de Brand Portal configurados con el Autor de Experience Manager que se ejecuta en el modo de ejecución **[!UICONTROL Scene7Connect]**.

## ¿Cómo se reproducen los vídeos dinámicos? {#how-are-dynamic-videos-played}

![Los códigos de vídeo se recuperan de la nube](assets/VideoEncodes.png)

Si las configuraciones de Dynamic Media ([Hybrid](../using/dynamic-video-brand-portal.md#configure-dm-hybrid-settings) o [[!DNL Scene 7]](../using/dynamic-video-brand-portal.md#configure-dm-scene7-settings)) están configuradas en Brand Portal, las representaciones dinámicas se recuperan del servidor **[!DNL Scene 7]**. Por lo tanto, las codificaciones de vídeo se previsualizan y se reproducen sin demora y con distorsión de la calidad.

Como las codificaciones de vídeo no se almacenan en el repositorio de Brand Portal y se recuperan del servidor **[!DNL Scene 7]**, asegúrese de que las configuraciones de Dynamic Media en la instancia de autor de AEM y Brand Portal sean las mismas.

>[!NOTE]
>
>Los visores de vídeo y los ajustes preestablecidos de visor no son compatibles con Brand Portal. Los vídeos se previsualizan y reproducen en los visores predeterminados en Brand Portal.

## Requisitos previos {#prerequisites}

Para trabajar con vídeos dinámicos en Brand Portal, asegúrese de:

* **Iniciar AEM Author en el**
modo DM (Dynamic Media)Iniciar la instancia de AEM Author (con la que se configura Brand Portal) en  [Dynamic Media Hybrid ](https://experienceleague.adobe.com/docs/experience-manager-65/assets/dynamic/config-dynamic.html) o  [Dynamic  [!DNL Scene 7] Media](https://experienceleague.adobe.com/docs/experience-manager-65/assets/dynamic/config-dms7.html).
* **Configure los servicios de nube de Dynamic Media en AEM**
AutorBasado en el modo Dynamic Media en el que se ejecuta AEM Author, establezca cualquiera de los servicios de nube de  [Dynamic Media ](https://experienceleague.adobe.com/docs/experience-manager-65/assets/dynamic/config-dynamic.html) o servicios de  [[!DNL Scene 7] nube en AEM ](https://experienceleague.adobe.com/docs/experience-manager-65/assets/dynamic/config-dms7.html) Author desde  **Herramientas**  |  **Cloud Services** |  **Dynamic Media**.
* **Configurar Dynamic Media en Brand**
PortalEn función de las configuraciones de nube de Dynamic Media en AEM Author, configure  [Dynamic Media ](#configure-dm-hybrid-settings) o  [[!DNL Scene 7] ](#configure-dm-scene7-settings)  configure desde las herramientas administrativas de Brand Portal.
Asegúrese de que [los inquilinos separados de Brand Portal](#separate-tenants) se utilizan para instancias de AEM Author configuradas con los modos Dynamic Media Hybrid y Dynamic Media **[!UICONTROL Scene7]**, si está utilizando funcionalidades de Dynamic Media Hybrid y Dynamic Media **[!UICONTROL S7]**.
* **Publicar carpetas con codificaciones de vídeo aplicadas a Brand**
PortalAplicar codificaciones de  [vídeo ](https://experienceleague.adobe.com/docs/experience-manager-65/assets/dynamic/video-profiles.html) y publicar la carpeta que contiene recursos de medios enriquecidos desde la instancia de AEM Author a Brand Portal.
* **IP de salida de lista de permitidos en SPS si la vista previa segura está**
habilitadaSi utiliza Dynamic Media-**[!DNL Scene 7]**  (con vista previa  [segura ](https://experienceleague.adobe.com/docs/dynamic-media-classic/using/upload-publish/testing-assets-making-them-public.html) habilitada para una empresa), se recomienda que el administrador de la  **[!DNL Scene 7]** empresa  [lista de permitidos las ](https://experienceleague.adobe.com/docs/dynamic-media-classic/using/upload-publish/testing-assets-making-them-public.html#testing-the-secure-testing-service) IP de salida pública para las regiones respectivas mediante la interfaz de usuario flash de SPS (Sistema de publicación de **[!UICONTROL Scene 7]** ).
Las direcciones IP de salida son las siguientes:

| **Región** | **IP de salida** |
|--- |--- |
| ND | 130.248.160.68, 20.94.203.130 |
| EMEA | 185.34.189.3, 51.132.146.75 |
| APAC | 63 140 44 54 |

Para incluir cualquiera de estas direcciones IP de salida en la lista de permitidos, consulte [preparar su cuenta para el servicio de pruebas seguras](https://experienceleague.adobe.com/docs/dynamic-media-classic/using/upload-publish/testing-assets-making-them-public.html#testing-the-secure-testing-service).

## Prácticas recomendadas  

Para asegurarse de que los recursos de vídeo dinámico se previsualizan, reproducen y descargan correctamente desde Brand Portal (y vínculos compartidos), siga estas prácticas:

### Inquilinos separados para los modos híbrido de Dynamic Media y Dynamic Media Scene7 {#separate-tenants}

Si utiliza las funciones **[!DNL Scene 7]** de Dynamic Media y las características híbridas de Dynamic Media, se recomienda utilizar diferentes inquilinos de Brand Portal para instancias de AEM Author configuradas con los modos **[!DNL Scene 7]** híbrido de Dynamic Media y Dynamic Media.


![Autor y BP de una a una asignación](assets/BPDynamicMedia.png)

### Los mismos detalles de configuración en la instancia de autor de AEM y Brand Portal

Asegúrese de que los detalles de configuración, como **[!UICONTROL Title]**, **[!UICONTROL Registration ID]**, **[!UICONTROL Video Service URL]** (en **[!UICONTROL Dynamic Media Hybrid]**) y **[!UICONTROL Title]**, credenciales (**[!UICONTROL Correo electrónico]** y contraseña), 12/>Región ]**,**[!UICONTROL  Empresa ]**(en Dynamic Media **[!DNL Scene 7]**) son iguales en Brand Portal y en**[!UICONTROL  AEM configuración de nube ]**.**[!UICONTROL 

### Lista de permitidos de direcciones IP de salida pública para el modo Dynamic Media Scene7

Si se utiliza Dynamic Media **[!UICONTROL Scene 7]** con [vista previa segura habilitada](https://experienceleague.adobe.com/docs/dynamic-media-classic/using/upload-publish/testing-assets-making-them-public.html) para servir recursos de vídeo en Brand Portal, **[!UICONTROL Scene 7]** establece un servidor de imágenes dedicado para entornos de ensayo o aplicaciones internas. Cualquier solicitud a este servidor comprueba la dirección IP de origen. Si la solicitud entrante no está dentro de la lista aprobada de direcciones IP, se devuelve una respuesta de error.
Por lo tanto, el **[!UICONTROL administrador de la empresa de Scene-7]** configura una lista aprobada de direcciones IP para el entorno **[!UICONTROL Secure Testing]** de su empresa a través de la interfaz de usuario flash de **[!UICONTROL SPS]** (Scene-7 Publishing System). Asegúrese de que la IP de salida de su región respectiva (de la siguiente) se agrega a esa lista aprobada.
Para incluir cualquiera de estas direcciones IP de salida en la lista de permitidos, consulte [preparar su cuenta para el servicio de pruebas seguras](https://experienceleague.adobe.com/docs/dynamic-media-classic/using/upload-publish/testing-assets-making-them-public.html#testing-the-secure-testing-service).
Las direcciones IP de salida son las siguientes:

| **Región** | **IP de salida** |
|--- |--- |
| ND | 130.248.160.66, 52.151.32.108 |
| EMEA | 185.34.189.1 |
| APAC | 63 140 44 54 |

## Configuración de la configuración de Dynamic Media (híbrido) {#configure-dm-hybrid-settings}

Si la instancia de AEM Author se está ejecutando en el modo híbrido de Dynamic Media, utilice el mosaico **[!UICONTROL Vídeo]** del panel de herramientas administrativas para configurar la configuración de la puerta de enlace de Dynamic Media.

>[!NOTE]
>
>Los [perfiles de codificación de vídeo](https://experienceleague.adobe.com/docs/experience-manager-65/assets/dynamic/video-profiles.html) no se publican en Brand Portal, sino que se recuperan del servidor **[!UICONTROL Scene 7]**. Por lo tanto, para que las codificaciones de vídeo se reproduzcan correctamente en Brand Portal, asegúrese de que los detalles de configuración sean los mismos que los de la [configuración de nube de Scene7](https://experienceleague.adobe.com/docs/experience-manager-65/assets/dynamic/config-dms7.html) en su instancia de autor de AEM.

Para configurar configuraciones de Dynamic Media en inquilinos de Brand Portal:

1. Seleccione el logotipo de AEM para acceder a las herramientas administrativas desde la barra de herramientas situada en la parte superior, en Brand Portal.
1. En el panel de herramientas administrativas, seleccione el mosaico **[!UICONTROL Video]**.

   ![Configuración híbrida de Dynamic Media en Brand Portal](assets/DMHybrid-Video.png)

   **[!UICONTROL Se abre la página Editar]** configuración de Dynamic Media.

   ![Configuración híbrida de Dynamic Media en Brand Portal](assets/edit-dynamic-media-config.png)

1. Especifique **[!UICONTROL ID de registro]** y **[!UICONTROL URL del servicio de vídeo]** (URL de DM-Gateway). Asegúrese de que estos detalles son los mismos que los de **[!UICONTROL Tools > Cloud Services]** en la instancia de autor de AEM.
1. Seleccione **Guardar** para guardar la configuración.

## Configuración de la configuración de Dynamic Media Scene7 {#configure-dm-scene7-settings}

Si la instancia de Autor de AEM se está ejecutando en modo Dynamic Media- **[!UICONTROL Scene 7]**, utilice el mosaico **[!UICONTROL Configuración de Dynamic Media]** del panel de herramientas administrativas para configurar los ajustes del servidor de **[!UICONTROL Scene 7]**.

Para configurar las configuraciones de Dynamic Media **[!UICONTROL Scene 7]** en inquilinos de Brand Portal:

1. Seleccione el logotipo de AEM para acceder a las herramientas administrativas desde la barra de herramientas situada en la parte superior, en Brand Portal.

2. En el panel de herramientas administrativas, seleccione el mosaico **[!UICONTROL Configuración de Dynamic Media]**.

   ![Configuración de DM  [!UICONTROL Scene7]  en Brand Portal](assets/DMS7-Tile.png)

   **[!UICONTROL Se abre la página Editar]** configuración de Dynamic Media.

   ![Configuración de Scene7 en Brand Portal](assets/S7Config.png)

3. Proporcione:

   * **[!UICONTROL Título]**
   * Credenciales (**[!UICONTROL ID de correo electrónico]** y **[!UICONTROL Contraseña]**) para acceder al servidor de Scene7
   * **[!UICONTROL Región]**

   Asegúrese de que estos valores son los mismos que los de la instancia de autor de AEM.

4. Seleccione **[!UICONTROL Connect to Dynamic Media]**.

5. Proporcione **[!UICONTROL Company name]** y **[!UICONTROL Save]** la configuración.
