---
title: Configurar AEM Assets con Brand Portal
seo-title: Configurar AEM Assets con Brand Portal
description: Obtenga una visión detallada de la configuración de AEM Assets con Brand Portal.
seo-description: Obtenga una visión detallada de la configuración de AEM Assets con Brand Portal.
uuid: null
content-type: reference
contentOwner: Vishabh Gupta
topic-tags: brand-portal
products: SG_EXPERIENCEMANAGER/Brand_Portal
discoiquuid: null
translation-type: tm+mt
source-git-commit: ba8a1f09573766643f6a5013a8d181f0f0dbb4f2
workflow-type: tm+mt
source-wordcount: '335'
ht-degree: 10%

---


# Configurar AEM Assets con Brand Portal {#configure-integration}

Recursos de Adobe Experience Manager (AEM) se configura con Brand Portal mediante Adobe Developer Console, que proporciona un distintivo IMS para la autorización del inquilino de Brand Portal. Brand Portal ahora es compatible con el servicio en la nube de AEM Assets, AEM Assets 6.3 y versiones posteriores.

La configuración de AEM Assets podría servir con Brand Portal y le permite publicar y distribuir recursos con los usuarios de Brand Portal. Mientras que la configuración de Brand Portal en AEM 6.3 (y versiones posteriores) permite la publicación de recursos, la distribución de recursos y las funciones de contribución de recursos para los usuarios de Brand Portal.

>[!NOTE]
>
>***Para AEM Assets 6.3 y superiores***
>
>Anteriormente, Brand Portal se configuraba en la IU clásica mediante OAuth Gateway heredado, que utiliza el intercambio de tokens JWT para obtener un Token de acceso IMS para la autorización.
>
>La configuración mediante OAuth heredado ya no se admite a partir del 6 de abril de 2020 y se cambia a la configuración mediante Adobe Developer Console.


>[!TIP]
>
>***Solo para clientes existentes***
>
>La configuración heredada de OAuth Gateway seguirá funcionando para los clientes existentes.
>
>En caso de que surjan problemas con la configuración heredada de OAuth Gateway, elimine la configuración existente y cree una nueva mediante Adobe Developer Console.


Los pasos para configurar AEM Assets con Brand Portal son diferentes en función de la versión de AEM y de si está configurando por primera vez o actualizando las configuraciones existentes:

| **Versión de AEM** | **Nueva configuración** | **Configuración de actualización** |
|---|---|---|
| **AEM Assets as a Cloud Service** | [Crear configuración](https://docs.adobe.com/content/help/en/experience-manager-cloud-service/assets/brand-portal/configure-aem-assets-with-brand-portal.html) | - |
| **AEM 6.5 (6.5.4.0 y posterior)** | [Crear configuración](https://docs.adobe.com/content/help/en/experience-manager-65/assets/brandportal/configure-aem-assets-with-brand-portal.html) | [Configuración de actualización](https://docs.adobe.com/content/help/en/experience-manager-65/assets/brandportal/configure-aem-assets-with-brand-portal.html#upgrade-integration-65) |
| **AEM 6.4 (6.4.8.0 y posterior)** | [Crear configuración](https://docs.adobe.com/content/help/en/experience-manager-64/assets/brandportal/configure-aem-assets-with-brand-portal.html) | [Configuración de actualización](https://docs.adobe.com/content/help/en/experience-manager-64/assets/brandportal/configure-aem-assets-with-brand-portal.html#upgrade-integration-64) |
| **AEM 6.3 (6.3.3.8 y posterior)** | [Crear configuración](https://helpx.adobe.com/experience-manager/6-3/assets/using/brand-portal-configuring-integration.html) | [Configuración de actualización](https://helpx.adobe.com/experience-manager/6-3/assets/using/brand-portal-configuring-integration.html#Upgradeconfiguration) |
| **AEM 6.2** | Comuníquese con la asistencia técnica | Comuníquese con la asistencia técnica |


