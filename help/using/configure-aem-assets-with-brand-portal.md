---
title: Configuración de Experience Manager Assets con Brand Portal
seo-title: Configure Experience Manager Assets with Brand Portal
description: Obtenga una conocimiento para configurar Experience Manager Assets con Brand portal.
seo-description: Get an insight into configuring Experience Manager Assets with Brand Portal.
uuid: null
content-type: reference
contentOwner: Vishabh Gupta
topic-tags: brand-portal
products: SG_EXPERIENCEMANAGER/Brand_Portal
discoiquuid: null
role: Admin
exl-id: 261c0e84-6b3d-459c-b6b9-a9af106d6943
source-git-commit: 454b05c05359a2068cc29124f826d5bd25a1bad1
workflow-type: tm+mt
source-wordcount: '372'
ht-degree: 6%

---

# Configuración de Experience Manager Assets con Brand Portal {#configure-integration}

La configuración de Adobe Experience Manager Assets con Brand portal permite la publicación recurso, recurso distribución y las funciones de contribución de recurso para los usuarios de Brand portal. Permite a los usuarios de Experience Manager Assets publicar y distribuir activos con los usuarios de Brand portal. Los usuarios de Brand portal pueden acceder a los activos compartidos y contribuyen al cargar nuevos activos en las carpetas de contribución recurso y volver a publicarlos en Experience Manager Assets.

La configuración de Experience Manager Assets con Brand portal es compatible con:

* Experience Manager Assets como Cloud Service
* Experience Manager Assets (on local and Managed Service) 6,5 y posterior

Experience Manager Assets como Cloud Service se configura automáticamente con Brand portal mediante la activación de Brand portal desde Cloud Manager. La activación flujo de trabajo crea las configuraciones requeridas en el back-end y activa el portal de marca en la misma organización IMS que el Experience Manager Assets como una Cloud Service instancia.

Mientras que Experience Manager Assets (on local and Managed Service) se configura manualmente con Brand portal mediante Adobe Systems consola del desarrollador, que proporciona un token de Adobe Systems Identity Management Services (IMS) para la autorización del inquilino de Brand portal.

>[!NOTE]
>
>***Para Experience Manager Assets 6,5 y posterior***
>
>Anteriormente, Brand portal se configuró en la interfaz clásica a través de la puerta de enlace OAuth heredada, que usa el intercambio de token Web de JSON (JWT) para obtener un token IMS para la autorización.
>
>La configuración a través de OAuth heredado ya no se admite el 6 de abril de 2020 y se cambia a la configuración mediante Adobe Systems consola de desarrollador.


>[!TIP]
>
>***Solo para clientes existentes (en servicio local y gestionado)***
>
>La configuración de la puerta de enlace de OAuth heredada seguirá funcionando para los clientes existentes.
>
>En caso de que encuentre problemas con la configuración de la puerta de enlace OAuth heredada, elimine la configuración existente y cree una nueva mediante Adobe Systems consola de desarrollo.

Los pasos para configurar Recursos AEM con Brand portal son diferentes según la versión de AEM y si está configurando por primera vez o actualizando las configuraciones existentes:

| **Versión de AEM** | **Configuración de Nuevo** | **Configuración de actualización** |
|---|---|---|
| **AEM Assets as a Cloud Service** | [Activar portal de marca](https://experienceleague.adobe.com/docs/experience-manager-cloud-service/assets/brand-portal/configure-aem-assets-with-brand-portal.html) | - |
| **AEM 6,5 (6.5.4.0 y posterior)** | [Crear configuración](https://experienceleague.adobe.com/docs/experience-manager-65/assets/brandportal/configure-aem-assets-with-brand-portal.html) | [Configuración de actualización](https://experienceleague.adobe.com/docs/experience-manager-65/assets/brandportal/configure-aem-assets-with-brand-portal.html#upgrade-integration-65) |
