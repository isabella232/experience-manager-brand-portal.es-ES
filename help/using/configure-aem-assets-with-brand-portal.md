---
title: Configuración de Experience Manager Assets con Brand Portal
seo-title: Configure Experience Manager Assets with Brand Portal
description: Obtenga información sobre la configuración de Recursos de Experience Manager con Brand Portal.
seo-description: Get an insight into configuring Experience Manager Assets with Brand Portal.
uuid: null
content-type: reference
contentOwner: Vishabh Gupta
topic-tags: brand-portal
products: SG_EXPERIENCEMANAGER/Brand_Portal
discoiquuid: null
role: Admin
exl-id: 261c0e84-6b3d-459c-b6b9-a9af106d6943
source-git-commit: 955cd8afe939ff47e9f08f312505e230e2f38495
workflow-type: tm+mt
source-wordcount: '419'
ht-degree: 11%

---

# Configuración de Experience Manager Assets con Brand Portal {#configure-integration}

La configuración de Adobe Experience Manager Assets con Brand Portal habilita la publicación de recursos, la distribución de recursos y las funciones de contribución de recursos para los usuarios de Brand Portal. Permite a los usuarios de Recursos de Experience Manager publicar y distribuir recursos con los usuarios de Brand Portal. Los usuarios de Brand Portal pueden acceder a los recursos compartidos y contribuir cargando nuevos recursos en las carpetas de contribución de recursos y publicándolos de nuevo en Recursos de Experience Manager.

La configuración de recursos Experience Manager con Brand Portal es compatible con:

* Experience Manager Assets as a Cloud Service
* Experience Manager Assets (local y servicio administrado) 6.3 y superior

Recursos de Experience Manager como Cloud Service se configura automáticamente con Brand Portal activando Brand Portal desde Cloud Manager. El flujo de trabajo de activación crea las configuraciones necesarias en el back-end y activa Brand Portal en la misma organización de IMS que en la instancia de Experience Manager Assets como Cloud Service.

Por su parte, Recursos de Experience Manager (servicio local y administrado) se configura manualmente con Brand Portal mediante Adobe Developer Console, que obtiene un token de Identity Management Services (IMS) de Adobe para la autorización del inquilino de Brand Portal.

>[!NOTE]
>
>***Para Experience Manager Assets 6.3 y superior***
>
>Anteriormente, Brand Portal se configuraba en la interfaz clásica a través de la puerta de enlace OAuth heredada, que utiliza el intercambio de token web JSON (JWT) para obtener un testigo IMS para la autorización.
>
>La configuración mediante OAuth heredado ya no es compatible a partir del 6 de abril de 2020 y se cambia a configurarse mediante Adobe Developer Console.


>[!TIP]
>
>***Solo para clientes existentes (servicio local y administrado)***
>
>La configuración heredada de OAuth Gateway seguirá funcionando para los clientes existentes.
>
>En caso de que encuentre problemas con la configuración heredada de OAuth Gateway, elimine la configuración existente y cree una nueva configuración a través de Adobe Developer Console.

Los pasos para configurar AEM Assets con Brand Portal son diferentes en función de la versión de AEM y de si está configurando por primera vez o actualizando las configuraciones existentes:

| **Versión de AEM** | **Nueva configuración** | **Configuración de actualización** |
|---|---|---|
| **AEM Assets as a Cloud Service** | [Activar Brand Portal](https://experienceleague.adobe.com/docs/experience-manager-cloud-service/assets/brand-portal/configure-aem-assets-with-brand-portal.html) | - |
| **AEM 6.5 (6.5.4.0 y posterior)** | [Crear configuración](https://experienceleague.adobe.com/docs/experience-manager-65/assets/brandportal/configure-aem-assets-with-brand-portal.html) | [Actualización de la configuración](https://experienceleague.adobe.com/docs/experience-manager-65/assets/brandportal/configure-aem-assets-with-brand-portal.html#upgrade-integration-65) |
| **AEM 6.4 (6.4.8.0 y posterior)** | [Crear configuración](https://experienceleague.adobe.com/docs/experience-manager-64/assets/brandportal/configure-aem-assets-with-brand-portal.html) | [Actualización de la configuración](https://experienceleague.adobe.com/docs/experience-manager-64/assets/brandportal/configure-aem-assets-with-brand-portal.html#upgrade-integration-64) |
| **AEM 6.3 (6.3.3.8 y posterior)** | [Crear configuración](https://helpx.adobe.com/es/experience-manager/6-3/assets/using/brand-portal-configuring-integration.html) | [Actualización de la configuración](https://helpx.adobe.com/es/experience-manager/6-3/assets/using/brand-portal-configuring-integration.html#Upgradeconfiguration) |
| **AEM 6.2** | Contacto con el servicio de asistencia | Contacto con el servicio de asistencia |
