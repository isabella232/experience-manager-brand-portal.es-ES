---
title: Configuración de AEM Assets con Brand Portal
seo-title: Configuración de AEM Assets con Brand Portal
description: Obtenga información sobre cómo configurar Recursos AEM con Brand Portal.
seo-description: Obtenga información sobre cómo configurar Recursos AEM con Brand Portal.
uuid: null
content-type: reference
contentOwner: Vishabh Gupta
topic-tags: brand-portal
products: SG_EXPERIENCEMANAGER/Brand_Portal
discoiquuid: null
translation-type: tm+mt
source-git-commit: 75d69f85a4178b78eba15a13f865a602e73d3a88

---


# Configuración de AEM Assets con Brand Portal {#configure-integration}

Los recursos de Adobe Experience Manager (AEM) se configuran con Brand Portal a través de Adobe I/O, que proporciona un distintivo IMS para la autorización del inquilino de Brand Portal. Brand Portal ahora es compatible con el servicio en la nube AEM Assets, AEM Assets 6.3 y versiones posteriores.

La configuración de Recursos AEM podría funcionar con Brand Portal y le permite publicar y distribuir recursos con los usuarios de Brand Portal. Mientras que la configuración de Brand Portal en AEM 6.3 (y versiones posteriores) permite la publicación de recursos, la distribución de recursos y las funciones de contribución de recursos para los usuarios de Brand Portal.

>[!NOTE]
>
>***Para AEM Assets 6.3 y posterior***
>
>Anteriormente, Brand Portal se configuraba en la IU clásica mediante OAuth Gateway heredado, que utiliza el intercambio de tokens JWT para obtener un Token de acceso IMS para la autorización.
>
>La configuración mediante OAuth heredado ya no se admite a partir del 6 de abril de 2020 y se cambia a la configuración mediante Adobe I/O.


>[!TIP]
>
>***Solo para clientes existentes***
>
>Se recomienda seguir utilizando la configuración heredada de OAuth Gateway. En caso de que surjan problemas con la configuración heredada de OAuth Gateway, elimine la configuración existente y cree una nueva configuración mediante Adobe I/O.


Los pasos para configurar Recursos AEM con Brand Portal son diferentes en función de la versión de AEM y de si está configurando por primera vez o actualizando las configuraciones existentes:

| **Versión de AEM** | **Nueva configuración** | **Configuración de actualización** |
|---|---|---|
| **AEM Assets as a Cloud Service** | [Crear configuración](https://docs.adobe.com/content/help/en/experience-manager-cloud-service/assets/brandportal/configure-aem-assets-with-brand-portal.html) | - |
| **AEM 6.5 (6.5.4.0 y posterior)** | [Crear configuración](https://docs.adobe.com/content/help/en/experience-manager-65/assets/brandportal/configure-aem-assets-with-brand-portal.html) | [Configuración de actualización](https://docs.adobe.com/content/help/en/experience-manager-65/assets/brandportal/configure-aem-assets-with-brand-portal.html#upgrade-integration-65) |
| **AEM 6.4 (6.4.8.0 y posterior)** | [Crear configuración](https://docs.adobe.com/content/help/en/experience-manager-64/assets/brandportal/configure-aem-assets-with-brand-portal.html) | [Configuración de actualización](https://docs.adobe.com/content/help/en/experience-manager-64/assets/brandportal/configure-aem-assets-with-brand-portal.html#upgrade-integration-64) |
| **AEM 6.3 (6.3.3.8 y posterior)** | [Crear configuración](https://helpx.adobe.com/experience-manager/6-3/assets/using/brand-portal-configuring-integration.html) | [Configuración de actualización](https://helpx.adobe.com/experience-manager/6-3/assets/using/brand-portal-configuring-integration.html#Upgradeconfiguration) |
| **AEM 6.2** | Comuníquese con la asistencia técnica | Comuníquese con la asistencia técnica |


<!--
   Comment Type: draft

   <li> </li>
   -->

<!--
   Comment Type: draft

   <li>Step text</li>
   -->
