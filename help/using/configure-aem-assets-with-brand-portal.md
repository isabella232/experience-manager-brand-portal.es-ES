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
source-git-commit: ecd53a7d92dd020e6a3527793ff11efadcb531ee
workflow-type: tm+mt
source-wordcount: '334'
ht-degree: 10%

---


# Configurar AEM Assets con Brand Portal {#configure-integration}

La configuración de Adobe Experience Manager Assets como Cloud Service con Adobe Experience Manager Assets Brand Portal le permite publicar y distribuir recursos con los usuarios de Brand Portal. Mientras que la configuración de AEM 6.3 (y posterior) con Brand Portal permite la publicación de recursos, la distribución de recursos y las funciones de contribución de recursos para los usuarios de Brand Portal.

Adobe Experience Manager Assets se configura con Brand Portal mediante Adobe Developer Console, que proporciona un token de Identity Management Services (IMS) de Adobe para la autorización del inquilino de Brand Portal.

>[!NOTE]
>
>***Para AEM Assets 6.3 y posterior***
>
>Anteriormente, Brand Portal se configuraba en la interfaz clásica mediante OAuth Gateway heredado, que utiliza el intercambio de tokens web JSON (JWT) para obtener un token de IMS para la autorización.
>
>La configuración mediante OAuth heredado ya no se admite a partir del 6 de abril de 2020 y se cambia a la configuración mediante la consola de desarrollador de Adobe.

>[!TIP]
>
>***Solo para clientes existentes***
>
>La configuración heredada de OAuth Gateway seguirá funcionando para los clientes existentes.
>
>En caso de que surjan problemas con la configuración heredada de OAuth Gateway, elimine la configuración existente y cree una nueva mediante Adobe Developer Console.

Los pasos para configurar AEM Assets con Brand Portal son diferentes en función de la versión AEM y de si está configurando por primera vez o actualizando las configuraciones existentes:

| **Versión de AEM** | **Nueva configuración** | **Configuración de actualización** |
|---|---|---|
| **AEM Assets as a Cloud Service** | [Crear configuración](https://docs.adobe.com/content/help/en/experience-manager-cloud-service/assets/brand-portal/configure-aem-assets-with-brand-portal.html) | - |
| **AEM 6.5 (6.5.4.0 y posterior)** | [Crear configuración](https://docs.adobe.com/content/help/en/experience-manager-65/assets/brandportal/configure-aem-assets-with-brand-portal.html) | [Configuración de actualización](https://docs.adobe.com/content/help/en/experience-manager-65/assets/brandportal/configure-aem-assets-with-brand-portal.html#upgrade-integration-65) |
| **AEM 6.4 (6.4.8.0 y posterior)** | [Crear configuración](https://docs.adobe.com/content/help/en/experience-manager-64/assets/brandportal/configure-aem-assets-with-brand-portal.html) | [Configuración de actualización](https://docs.adobe.com/content/help/en/experience-manager-64/assets/brandportal/configure-aem-assets-with-brand-portal.html#upgrade-integration-64) |
| **AEM 6.3 (6.3.3.8 y posterior)** | [Crear configuración](https://helpx.adobe.com/experience-manager/6-3/assets/using/brand-portal-configuring-integration.html) | [Configuración de actualización](https://helpx.adobe.com/experience-manager/6-3/assets/using/brand-portal-configuring-integration.html#Upgradeconfiguration) |
| **AEM 6.2** | Comuníquese con la asistencia técnica | Comuníquese con la asistencia técnica |
