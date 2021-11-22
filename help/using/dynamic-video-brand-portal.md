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
source-git-commit: 7128c71576ae938a49f9bff0b95b98b7fc480f69
workflow-type: tm+mt
source-wordcount: '1256'
ht-degree: 3%

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
>Para trabajar con vídeos y publicarlos en Brand Portal, asegúrese de que la instancia de Autor Experience Manager esté configurada en el modo Híbrido de Dynamic Media o en Dynamic Media **[!DNL Scene7]** en el menú contextual.

Para obtener una vista previa, reproducir y descargar vídeos, Brand Portal expone las dos configuraciones siguientes a los administradores:

* [Configuración híbrida de Dynamic Media](#configure-dm-hybrid-settings)
Si la instancia de Autor de Experience Manager se está ejecutando en el modo híbrido de Dynamic Media.
* [Dynamic Media [!DNL Scene7] configuración](#configure-dm-scene7-settings)
Si la instancia de Experience Manager Author se está ejecutando en Dynamic Media-**[!DNL Scene7]** en el menú contextual.
Establezca cualquiera de estas configuraciones en función de las configuraciones establecidas en la instancia de Autor de Experience Manager con la que se replica el inquilino de Brand Portal.

>[!NOTE]
>
>Los vídeos dinámicos no son compatibles con los inquilinos de Brand Portal configurados con el Autor Experience Manager que se ejecuta en **[!UICONTROL Scene7Connect]** ejecutar modo.

## ¿Cómo se reproducen los vídeos dinámicos? {#how-are-dynamic-videos-played}

![Los códigos de vídeo se recuperan de la nube](assets/VideoEncodes.png)

Si las configuraciones de Dynamic Media ([Híbrido](../using/dynamic-video-brand-portal.md#configure-dm-hybrid-settings) o [[!DNL Scene7]](../using/dynamic-video-brand-portal.md#configure-dm-scene7-settings) configuraciones) están configuradas en Brand Portal, las representaciones dinámicas se recuperan de **[!DNL Scene7]** servidor. Por lo tanto, las codificaciones de vídeo se previsualizan y se reproducen sin demora y con distorsión de la calidad.

Como las codificaciones de vídeo no se almacenan en el repositorio de Brand Portal y se recuperan de **[!DNL Scene7]** , asegúrese de que las configuraciones de Dynamic Media en la instancia de autor de Adobe Experience Manager y Brand Portal son las mismas.

>[!NOTE]
>
>Los visores de vídeo y los ajustes preestablecidos de visor no son compatibles con Brand Portal. Los vídeos se previsualizan y reproducen en los visores predeterminados en Brand Portal.

## Requisitos previos {#prerequisites}

Para trabajar con vídeos dinámicos en Brand Portal, asegúrese de:

* **Iniciar Experience Manager Author en el modo Dynamic Media**
Inicie la instancia de Autor del Experience Manager (con la que está configurado Brand Portal) en [Dynamic Media - [!DNL Scene7] mode](https://experienceleague.adobe.com/docs/experience-manager-65/assets/dynamic/config-scene7-mode/config-dms7.html?lang=en#enabling-dynamic-media-in-scene-mode) o [Dynamic Media: modo híbrido](https://experienceleague.adobe.com/docs/experience-manager-65/assets/dynamic/config-dynamic.html) o
* **Configuración de Cloud Services de Dynamic Media en el autor del Experience Manager**
En función del modo Dynamic Media (modo Scene7 o modo híbrido), el autor del Experience Manager se está ejecutando en, establezca una de las opciones siguientes: [Cloud Services de Dynamic Media ([!DNL Scene7] mode)](https://experienceleague.adobe.com/docs/experience-manager-65/assets/dynamic/config-scene7-mode/config-dms7.html?lang=en#configuring-dynamic-media-cloud-services) o [Cloud Services de Dynamic Media (modo híbrido)](https://experienceleague.adobe.com/docs/experience-manager-65/assets/dynamic/config-dynamic.html?lang=en#configuring-dynamic-media-cloud-services) en el autor Experience Manager de **Herramientas** | **Cloud Services** | **Dynamic Media**.
* **Configuración de Dynamic Media en Brand Portal**
En función de las configuraciones de nube de Dynamic Media en Autor Experience Manager, configure [Configuración de Dynamic Media](#configure-dm-hybrid-settings) o [[!DNL Scene7] configuración](#configure-dm-scene7-settings)  desde las herramientas administrativas de Brand Portal.
Asegúrese de que [inquilinos separados de Brand Portal](#separate-tenants) se utilizan para instancias de Autor de Experience Manager configuradas en Dynamic Media - **[!UICONTROL Scene7]** y Dynamic Media: modo híbrido. Especialmente si utiliza funcionalidades de Dynamic Media **[!UICONTROL S7]** y Dynamic Media Hybrid.
* **Publicar carpetas con codificaciones de vídeo aplicadas a Brand Portal**
Aplicar [codificaciones de vídeo](https://experienceleague.adobe.com/docs/experience-manager-65/assets/dynamic/video-profiles.html) y publique la carpeta que contiene recursos de medios enriquecidos desde la instancia de autor de Experience Manager a Brand Portal.
* **IP de salida de lista de permitidos en SPS si la previsualización segura está habilitada**
Si utiliza Dynamic Media-**[!DNL Scene7]** (con [vista previa segura habilitada](https://experienceleague.adobe.com/docs/dynamic-media-classic/using/upload-publish/testing-assets-making-them-public.html) para una empresa), se recomienda que **[!DNL Scene7]** administrador de empresa [lista de permitidos de las IP de salida públicas](https://experienceleague.adobe.com/docs/dynamic-media-classic/using/upload-publish/testing-assets-making-them-public.html#testing-the-secure-testing-service) para las regiones respectivas que utilicen SPS (**[!UICONTROL Scene7]** Sistema de publicación) interfaz de usuario flash.
Las direcciones IP de salida son las siguientes:

| **Región** | **IP de salida** |
|--- |--- |
| ND | 130.248.160.68, 20.94.203.130 |
| EMEA | 185.34.189.3, 51.132.146.75 |
| APAC | 63 140 44 54 |

Para incluir en la lista de permitidos cualquiera de estas direcciones IP de salida, consulte [prepare su cuenta para el servicio de pruebas seguras](https://experienceleague.adobe.com/docs/dynamic-media-classic/using/upload-publish/testing-assets-making-them-public.html#testing-the-secure-testing-service).

## Prácticas recomendadas  

Para asegurarse de que los recursos de vídeo dinámico se previsualizan, reproducen y descargan correctamente desde Brand Portal (y vínculos compartidos), siga estas prácticas:

### Inquilinos separados para Dynamic Media - Scene7 y Dynamic Media - Modos híbridos {#separate-tenants}

Si usa ambas Dynamic Media: **[!DNL Scene7]** modo y Dynamic Media: funciones de modo híbrido, utilice diferentes inquilinos de Brand Portal para instancias de Experience Manager Author configuradas con Dynamic Media - **[!DNL Scene7]** y Dynamic Media: modos híbridos.


![Autor y BP de una a una asignación](assets/BPDynamicMedia.png)

### Los mismos detalles de configuración en la instancia de autor del Experience Manager y en Brand Portal

Asegúrese de que los detalles de configuración son los mismos en Brand Portal y **[!UICONTROL Configuración de Experience Manager Cloud]**. Los mismos detalles de configuración incluyen lo siguiente:

* **[!UICONTROL Título]**
* **[!UICONTROL ID de registro]**
* **[!UICONTROL URL del servicio de vídeo]** en **[!UICONTROL Dynamic Media: modo híbrido]**
* **[!UICONTROL Título]**
* Credenciales (**[!UICONTROL Correo electrónico]** y contraseña)
* **[!UICONTROL Región]**
* **[!UICONTROL Empresa]** en Dynamic Media - **[!DNL Scene7]** mode

### Lista de permitidos de IP de salida pública para el modo Scene7 de Dynamic Media

Si Dynamic Media **[!UICONTROL Scene7]**-Having [vista previa segura habilitada](https://experienceleague.adobe.com/docs/dynamic-media-classic/using/upload-publish/testing-assets-making-them-public.html)-se utiliza para servir recursos de vídeo a Brand Portal y, a continuación, **[!UICONTROL Scene7]** establece un servidor de imagen dedicado para entornos de ensayo o aplicaciones internas. Cualquier solicitud a este servidor comprueba la dirección IP de origen. Si la solicitud entrante no está dentro de la lista aprobada de direcciones IP, se devuelve una respuesta de error.
La variable **[!UICONTROL Scene7]** Por lo tanto, el administrador de la empresa configura una lista aprobada de direcciones IP para la **[!UICONTROL Pruebas seguras]** entorno, hasta **[!UICONTROL SPS]** Interfaz de usuario flash (Scene7 Publishing System). Asegúrese de que la IP de salida de su región respectiva (de la siguiente) se agrega a esa lista aprobada.
Para incluir en la lista de permitidos cualquiera de estas direcciones IP de salida, consulte [prepare su cuenta para el servicio de pruebas seguras](https://experienceleague.adobe.com/docs/dynamic-media-classic/using/upload-publish/testing-assets-making-them-public.html#testing-the-secure-testing-service).
Las direcciones IP de salida son las siguientes:

| **Región** | **IP de salida** |
|--- |--- |
| ND | 130.248.160.66, 52.151.32.108 |
| EMEA | 185.34.189.1 |
| APAC | 63 140 44 54 |

## Configuración de la configuración de Dynamic Media (híbrido) {#configure-dm-hybrid-settings}

Si la instancia de Experience Manager Author se está ejecutando en el modo híbrido de Dynamic Media, utilice **[!UICONTROL Vídeo]** mosaico del panel de herramientas administrativas para configurar los ajustes de la puerta de enlace de Dynamic Media.

>[!NOTE]
>
>La variable [perfiles de codificación de vídeo](https://experienceleague.adobe.com/docs/experience-manager-65/assets/dynamic/video-profiles.html) no se publican en Brand Portal, sino que se recuperan del **[!UICONTROL Scene7]** servidor. Por lo tanto, para que las codificaciones de vídeo se reproduzcan correctamente en Brand Portal, asegúrese de que los detalles de configuración sean los mismos que los del [Cloud Services de Dynamic Media ([!DNL Scene7] mode)](https://experienceleague.adobe.com/docs/experience-manager-65/assets/dynamic/config-scene7-mode/config-dms7.html?lang=en#configuring-dynamic-media-cloud-services) en la instancia de Autor del Experience Manager.

Para configurar configuraciones de Dynamic Media en inquilinos de Brand Portal:

1. Seleccione el logotipo del Experience Manager para acceder a las herramientas administrativas desde la barra de herramientas situada en la parte superior, en Brand Portal.
1. En el panel de herramientas administrativas, seleccione la **[!UICONTROL Vídeo]** mosaico.

   ![Configuración híbrida de Dynamic Media en Brand Portal](assets/DMHybrid-Video.png)

   **[!UICONTROL Editar configuración de Dynamic Media]** se abre.

   ![Configuración híbrida de Dynamic Media en Brand Portal](assets/edit-dynamic-media-config.png)

1. Especifique **[!UICONTROL ID de registro]** y **[!UICONTROL URL del servicio de vídeo]** (URL de puerta de enlace DM). Asegúrese de que estos detalles sean los mismos que esos detalles en **[!UICONTROL Herramientas > Cloud Services]** en la instancia de Autor del Experience Manager.
1. Select **Guardar** para guardar la configuración.

## Configuración de la configuración de Dynamic Media Scene7 {#configure-dm-scene7-settings}

Si la instancia de Experience Manager Author se está ejecutando en Dynamic Media- **[!UICONTROL Scene7]** y, a continuación, utilice **[!UICONTROL Configuración de Dynamic Media]** mosaico del panel de herramientas administrativas para configurar el **[!UICONTROL Scene7]** configuración del servidor.

Para configurar Dynamic Media **[!UICONTROL Scene7]** configuraciones en inquilinos de Brand Portal:

1. Seleccione el logotipo del Experience Manager para acceder a las herramientas administrativas desde la barra de herramientas situada en la parte superior, en Brand Portal.

2. En el panel de herramientas administrativas, seleccione la **[!UICONTROL Configuración de Dynamic Media]** mosaico.

   ![DM [!UICONTROL Escena 7] configuración en Brand Portal](assets/DMS7-Tile.png)

   **[!UICONTROL Editar configuración de Dynamic Media]** se abre.

   ![Configuración de Scene7 en Brand Portal](assets/S7Config.png)

3. Proporcione:

   * **[!UICONTROL Título]**
   * Credenciales (**[!UICONTROL ID de correo electrónico]** y **[!UICONTROL Contraseña]**) para acceder al servidor de Scene7
   * **[!UICONTROL Región]**

   Asegúrese de que estos valores son los mismos que los que se encuentran en la instancia de autor de Experience Manager.

4. Select **[!UICONTROL Conectarse a Dynamic Media]**.

5. Proporcione la variable **[!UICONTROL Nombre de la empresa]** y **[!UICONTROL Guardar]** la configuración.
