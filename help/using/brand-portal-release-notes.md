---
title: Notas de la versión
seo-title: Notas de la versión
description: Obtenga una visión detallada de las funciones, mejoras, problemas importantes solucionados y problemas conocidos de la versión 6.4.6 de Adobe Experience Manager Assets Brand Portal.
seo-description: Obtenga una visión detallada de las mejoras, los problemas críticos solucionados y los problemas conocidos en la versión 6.4.6 de Adobe Experience Manager Assets Brand Portal.
uuid: 3d6ffb6f-4608-4e83-8486-5c90e06cdb43
content-type: reference
contentOwner: Vishabh Gupta
topic-tags: brand-portal
products: SG_EXPERIENCEMANAGER/Brand_Portal
discoiquuid: 79ebb9fc-385c-48a8-979e-374f42517988
translation-type: tm+mt
source-git-commit: 9bb1538165030f7f9e78af99bb89ea38897c3967

---


# Notas de la versión {#release-notes}

Obtenga una visión detallada de las nuevas funciones, mejoras, problemas importantes solucionados y problemas conocidos de la versión 6.4.6 de Adobe Experience Manager Assets Brand Portal.

## Información de la versión {#release-information}

| Producto | Adobe Experience Manager Assets Brand Portal |
|---|---|
| Versión | 6.4.6 |
| Fecha | Marzo de 2020 |

## Información general {#overview}

Recursos Adobe Experience Manager (AEM) Assets Brand Portal le ayuda a adquirir, controlar y distribuir de forma segura recursos creativos aprobados a terceros externos y usuarios empresariales internos entre dispositivos. Ayuda a mejorar la eficiencia del uso compartido de activos, acelera el tiempo de comercialización de los activos y reduce el riesgo de incumplimiento y acceso no autorizado. Brand Portal permite a los usuarios explorar, buscar, previsualización, descargar y exportar recursos en formatos aprobados por la empresa, en cualquier momento y lugar.

## Novedades de 6.4.6 {#what-s-new-in-646}

### New Features {#new-feature}

Esta versión incluye las siguientes nuevas funciones:

* Captcha para iniciar sesión como invitado en Brand Portal. Consulte Acceso [de invitados a](../using/guest-access.md) Brand Portal para obtener más información.

* Brand Portal ahora es compatible con el servicio en la nube de AEM Assets. Puede configurar Recursos AEM para que el servicio con Brand Portal pueda compartir y distribuir recursos con los usuarios de Brand Portal.
Para obtener más información, consulte [Configuración del servicio en la nube de AEM Assets con Brand Portal](https://docs.adobe.com/content/help/en/experience-manager-cloud-service/assets/brand-portal/configure-aem-assets-with-brand-portal.html).

### Mejoras {#enhancements-646}

Esta versión de Brand Portal incluye las siguientes mejoras:

* En AEM 6.3 y versiones posteriores, se cambia el canal de autorización entre AEM Assets y Brand Portal. Recursos AEM ahora se configura con Brand Portal a través de Adobe I/O, que proporciona un distintivo IMS para la autorización del inquilino de Brand Portal.

   >[!NOTE]
   >
   >La configuración mediante OAuth heredado ya no se admite a partir del 6 de abril de 2020 y se cambia a la configuración mediante Adobe I/O.


>[!TIP]
>
>***Solo para clientes existentes***
>
>Se recomienda seguir utilizando la configuración heredada de OAuth Gateway. En caso de que surjan problemas con la configuración heredada de OAuth Gateway, elimine la configuración existente y cree una nueva configuración mediante Adobe I/O.


For more information, see [Configure AEM Assets with Brand Portal](configure-aem-assets-with-brand-portal.md)

### Problemas críticos solucionados {#critical-issues-fixed}

Esta versión incluye correcciones a los siguientes problemas críticos:

* Los valores desplegables del esquema de metadatos no están visibles en las propiedades de los recursos.

* El subesquema de metadatos no muestra fichas basadas en mimetype en las propiedades del recurso.

* El esquema Cancelar la publicación de metadatos rellena un mensaje de error aunque el esquema se elimina al final.

* La imagen de Previsualización no se muestra para un recurso publicado.

* El usuario no puede publicar ni cancelar la publicación de recursos que contengan una sola cita en el nombre.

* Los términos y condiciones no se muestran al descargar varios recursos.

* Se han solucionado pequeñas vulnerabilidades de seguridad.

### Problemas conocidos {#known-issues}

Esta versión incluye los siguientes problemas conocidos:

* Los usuarios de Brand Portal no pueden publicar recursos de carpetas de contribución en Recursos AEM al actualizar a Adobe I/O en AEM 6.5.4.

   Este problema se solucionará en el próximo Service Pack 6.5.5.

   Para una corrección inmediata en AEM 6.5.4, se recomienda [descargar la revisión](https://www.adobeaemcloud.com/content/marketplace/marketplaceProxy.html?packagePath=/content/companies/public/adobe/packages/cq650/hotfix/cq-6.5.0-hotfix-33041) e instalarla en la instancia de creación.

* La opción Excluir representaciones del sistema no funciona correctamente al descargar un recurso.


## Idiomas {#languages}

La interfaz de usuario de Brand Portal está disponible en los siguientes idiomas:

* Inglés
* Alemán
* Francés
* Español
* Italiano
* Portugués de Brasil
* Japonés
* Chino simplificado
* Coreano

## Plataformas certificadas {#certified-platforms}

Para determinar qué plataformas están certificadas para ejecutarse con esta versión de Brand Portal, consulte la columna **Asistencia para la IU** táctil en la tabla de la sección Exploradores **admitidos para la interfaz** de usuario de creación de Requisitos [](https://helpx.adobe.com/experience-manager/6-4/sites/deploying/using/technical-requirements.html)técnicos.

## Vínculos {#links}

* [Página del producto Adobe Experience Manager en adobe.com](http://www.adobe.com/in/marketing-cloud/experience-manager.html)
* [Documentación de Assets Brand Portal](https://helpx.adobe.com/es/experience-manager/brand-portal/user-guide.html)

## Asistencia y acceso al producto (sitios restringidos) {#product-access-and-support-restricted-sites}

Estos sitios solo están disponibles para los clientes. Si es un cliente y necesita acceso, póngase en contacto con su administrador de cuentas de Adobe.

* [https://daycare.day.com](https://daycare.day.com)

* [Acceso a productos](https://login.marketing.adobe.com)

* [Servicio de atención al cliente de Adobe](https://helpx.adobe.com/contact.html)
