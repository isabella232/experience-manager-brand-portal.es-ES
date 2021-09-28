---
title: 'Preguntas frecuentes '
seo-title: null
description: Obtenga información sobre las preguntas más frecuentes en Adobe Experience Manager Assets Brand Portal.
seo-description: null
uuid: null
content-type: reference
contentOwner: Vishabh Gupta
topic-tags: frequently-asked-questions
products: SG_EXPERIENCEMANAGER/Brand_Portal
discoiquuid: null
exl-id: 4a8f7fbd-7485-421d-a8db-755324d2dbef
source-git-commit: d7dbf9ae2d27dda2edb60d8f861e618fb6332ec7
workflow-type: tm+mt
source-wordcount: '1480'
ht-degree: 1%

---

# Preguntas frecuentes  {#frequently-asked-questions}

Las preguntas frecuentes de Brand Portal se centran en las consultas y los problemas que los usuarios finales pueden encontrar al trabajar con la última versión de AEM Assets Brand Portal 6.4.6 o versiones anteriores.


## Preguntas más frecuentes sobre Brand Portal 6.4.6  {#faqs-bp646}

**Ques. El extremo OAuth heredado existente (`https://legacy-oauth.cloud.adobe.io/login`) no funciona. ¿Cuál podría ser la posible razón?**

**Ans.** La configuración OAuth heredada está en desuso. Debe actualizar las instancias de autor de AEM Assets al Service Pack más reciente y configurarlas mediante Adobe Developer Console. Consulte [Configurar AEM Assets con Brand Portal](configure-aem-assets-with-brand-portal.md) para obtener más información. Sin embargo, para que la configuración heredada de OAuth funcione hasta que actualice, actualice el extremo heredado de OAuth a `https://hypnosisprod.ethos11-prod-or1.ethos.adobe.net/`.

<!--
**Ques. I have created a collection using the asset link shared by the administrator. But I am unable to create a share link for my collection. Do I need special permissions to do this?**

**Ans.** The functionality is by design, the viewer users are not permitted to share link for collections as they have limited privileges due to which they cannot add users to create a share link. It is a known issue that the share link for collections is currently visible to the viewer users. This issue will be fixed in the upcoming release, the option to share link for the collections will not be available to the viewer users.    
-->

**Ques. No puedo publicar los recursos de la carpeta de contribución de Brand Portal a AEM Assets después de actualizar a Adobe Developer Console. Mi instancia de autor se encuentra en la AEM 6.5.4. ¿Cuál podría ser la razón posible?**

**Ans.** Sí, hay un problema conocido al publicar los recursos de la carpeta de contribución en AEM Assets en AEM 6.5.4 a través de Adobe Developer Console.

El problema se ha solucionado en AEM 6.5.5. Puede actualizar la instancia de AEM Assets al último Service Pack AEM 6.5.5 y [actualizar sus configuraciones](https://experienceleague.adobe.com/docs/experience-manager-65/assets/brandportal/configure-aem-assets-with-brand-portal.html#upgrade-integration-65) en Adobe Developer Console.

<!--
Broken link of download hotfix, comment out this section until we have the latest URL.

For immediate fix on AEM 6.5.4, it is recommended to [download the hotfix](https://www.adobeaemcloud.com/content/marketplace/marketplaceProxy.html?packagePath=/content/companies/public/adobe/packages/cq650/hotfix/cq-6.5.0-hotfix-33041) and install on your AEM author instance.
-->

**Ques. No veo el contenido de la carpeta de contribución publicado desde Brand Portal en AEM Assets. ¿Cuál podría ser la posible razón?**

**Ans.** Póngase en contacto con el administrador de AEM Assets para comprobar las configuraciones y asegurarse de que el inquilino de Brand Portal esté configurado con una sola instancia de autor de AEM Assets.

Este problema posiblemente se produzca cuando haya configurado un inquilino de Brand Portal en varias instancias de autor de AEM Assets. Por ejemplo, el administrador configura el mismo inquilino de Brand Portal en la instancia de autor de AEM Assets del entorno de ensayo y producción. En este caso, los déclencheur de publicación de recursos en Brand Portal, pero la instancia de autor de AEM Assets no pudo importar el recurso porque el agente de replicación no recibe el token de solicitud.


**Ques. No puedo publicar recursos de AEM Assets en Brand Portal. El registro de replicación indica que se agotó el tiempo de espera de la conexión. ¿Hay alguna solución rápida?**

**Ans.** Normalmente, la publicación falla con un error de tiempo de espera si hay varias solicitudes pendientes en la cola de replicación. Para resolver este problema, asegúrese de que los agentes de replicación estén configurados para evitar el tiempo de espera.

Realice los siguientes pasos para configurar el agente de replicación:

1. Inicie sesión en la instancia de autor de AEM Assets.
1. En el panel **Herramientas**, vaya a **[!UICONTROL Implementación]** > **[!UICONTROL Replicación]**.
1. En la página Replicación, haga clic en **[!UICONTROL Agentes del autor]**. Puede ver los cuatro agentes de replicación para su inquilino de Brand Portal.
1. Haga clic en la URL del agente de replicación para abrir los detalles del agente.
1. Haga clic en **[!UICONTROL Editar]** para modificar la configuración del agente de replicación.
1. En Configuración del agente, haga clic en la pestaña **[!UICONTROL Extended]**.
1. Seleccione la casilla de verificación **[!UICONTROL Cerrar conexión]**.
1. Repita los pasos del 4 al 7 para configurar los cuatro agentes de replicación.
1. Reinicie el servidor y compruebe la conexión.


## Preguntas más frecuentes sobre Brand Portal 6.4.5  {#faqs-bp645}

**Ques. ¿Cuál es el cambio más importante en la versión 6.4.5 de Brand Portal?**

**Ans.** AEM Assets Brand Portal 6.4.5 es una versión de funciones que permite a los usuarios de Brand Portal cargar contenido desde la instancia de Brand Portal y volver a publicar la carpeta Contribution en AEM Assets sin necesidad de derechos de administrador.
Para obtener más información, consulte [Asset Sourcing in Brand Portal](brand-portal-asset-sourcing.md).



**Ques. ¿Perderé acceso a cualquier recurso, función o configuración existente que haya creado?**

**Ans.** Todas las funciones y configuraciones existentes permanecen intactas. Los usuarios finales no se ven afectados y el contenido permanece intacto.



**Ques. ¿Cuándo paso a la nueva versión de Brand Portal?**

**Ans.** Brand Portal 6.4.5 se publicó para su producción en octubre de 2019. Y se espera que la próxima versión de Brand Portal se publique en el tercer trimestre de 2020.
Para actualizaciones y cambios de versión, se recomienda realizar el seguimiento de las [Notas de la versión](brand-portal-release-notes.md) y las [Novedades de Brand Portal](whats-new.md).



**Ques. ¿Se verán afectados mis usuarios?**

**Ans.** La versión de Brand Portal 6.4.5 se encuentra exclusivamente en Brand Portal, por lo que no afecta a los usuarios finales.



**Ques. ¿Se requiere alguna acción por mi parte como usuario de Brand Portal?**

**Ans.** La versión 6.4.5 de Brand Portal incorpora una nueva función denominada Asset Sourcing. AEM administrador debe configurar la función de abastecimiento de recursos en AEM Assets para que los usuarios de Brand Portal puedan habilitarla. Para obtener más información, consulte [Habilitar abastecimiento de recursos](brand-portal-asset-sourcing.md).



**Ques. ¿Quién puede crear una carpeta de contribución?**

**Ans.** Cualquier usuario AEM que tenga permisos para crear una carpeta nueva en AEM Assets puede crear una carpeta de  **** contribución. Para crear una carpeta **Contribution**, cree una nueva carpeta de tipo **Asset Contribution**.
Esta carpeta se comparte con los usuarios activos de Brand Portal para obtener contribución.



**Ques. ¿Qué contiene una carpeta de contribución?**

**Ans.** **** La carpeta Contributionfolder contiene dos subcarpetas  **** NEW **y SHARED**. Inicialmente, la carpeta NEW está en blanco y la carpeta SHARED contiene el contenido de referencia (recursos reutilizables) para los usuarios de Brand Portal.
Los usuarios de Brand Portal acceden a la carpeta **Contribution** y cargan contenido en la carpeta **NEW**.



**Ques.  ¿Puedo modificar el nombre de una carpeta de contribución existente?**

**Ans.** **No**, no se puede modificar el nombre de una carpeta de  **** contribución existente.



**Ques. ¿Cuáles son los requisitos de los recursos con contribución de r.t?**

**Ans.** El  **** documento breve adjunto a la carpeta  **** Contributionfolder y el contenido de referencia (recursos reutilizables) cargados en la carpeta  **** SHARED ayuda al usuario de Brand Portal a comprender la necesidad de la contribución y las expectativas como colaborador, y se denomina de forma colectiva como requisitos de recursos.



**Ques. ¿Puedo cargar recursos en cualquier carpeta permitida?**

**Ans.** No todas las carpetas permitidas. Un usuario de Brand Portal solo puede cargar contenido en la carpeta **Contribution** que comparte el administrador de AEM o Brand Portal.



**Ques. ¿Cómo puedo obtener acceso a una carpeta de contribución?**

**Ans.** Solo puede acceder a una carpeta de  **** contribución si se ha compartido con usted. Recibirá una notificación por correo electrónico/pulso cada vez que se comparta una carpeta de Contribution con usted. Puede acceder a la carpeta Contribución a través del vínculo compartido en el correo electrónico o iniciar sesión en la instancia de Brand Portal y navegar hasta el icono de la campana para que la notificación acceda a la carpeta Contribución .

>[!NOTE]
>
>Si no es un usuario de Brand Portal existente, solicite al administrador de AEM que cree su usuario en Admin Console de AEM y añada su perfil al archivo de configuración de usuario en la lista de usuarios de Brand Portal.

**Ques. ¿Cuál es el formato del archivo CSV para la importación del usuario?**

**Ans.** El formato es el mismo que el que admite Admin Console para la importación masiva de usuarios. El correo electrónico, el nombre y los apellidos son obligatorios.



**Ques. ¿Qué rellena la lista de usuarios (colaboradores de Brand Portal) en la lista desplegable de usuarios de Asset Contribution?**

**Ans.** Los usuarios de la lista desplegable se rellenan desde el archivo de configuración de usuario de Brand Portal (.csv) cargado en AEM.



**Ques. ¿Dónde puedo ver el estado de los trabajos de importación y publicación?**

**Ans.** En AEM, puede ver el estado de una importación en la página  **** asyncjob. En Brand Portal, puede ver el estado de un trabajo de publicación en **[!UICONTROL Tools > Asset Contribution status]**.



**Ques. ¿Cuál es la frecuencia de un trabajo de importación que se ejecuta periódicamente en AEM?**

**Ans.** En AEM, la votación se realiza cada 5 minutos.



**Ques. ¿Hay algún umbral en la cantidad de veces que se puede publicar una carpeta de Brand Portal a AEM Assets?**

**Ans.** No, todos los recursos de la  **** carpeta NEW se publican en AEM Assets independientemente de que se hayan publicado anteriormente. Cada vez que se publica una carpeta **Contribution** de Brand Portal en AEM Assets, anula el contenido de la carpeta **NEW**.



**Ques. ¿Cómo cargar nuevos activos en una carpeta de contribución?**

**Ans.** Consulte la documentación detallada para  [Cargar recursos a la carpeta](brand-portal-publish-contribution-folder-to-brand-portal.md) Contribución .



**Ques. ¿No veo miniaturas o vistas previas en los recursos cargados en la NUEVA carpeta por un usuario de Brand Portal?**

**Ans.** Está diseñado, ya que no se está ejecutando ningún flujo de trabajo en el extremo de Brand Portal.



**Ques. ¿Qué sucede si una carpeta se publica de AEM Assets en Brand Portal que está en flujo?**

**Ans.** En AEM, los registros se mantienen para cada vez que se publica una carpeta en Brand Portal. En el momento de la publicación, todos los recursos que no se publican en Brand Portal se colocan en una cola de replicación. Cualquier recurso añadido a la carpeta después de activar el trabajo de publicación no se publica en Brand Portal. Cuando el usuario AEM publica la carpeta de nuevo, solo los recursos que no se publicaron anteriormente (que ya existían en la cola de replicación) se publican en Brand Portal.
Esto se aplica a todas las carpetas publicadas desde AEM Assets en Brand Portal y a las carpetas COMPARTIDAS en una carpeta de Contribución.

**Ques. ¿Con quién puedo contactar?**

**Ans.** Póngase en contacto con el administrador de cuentas de Adobe o con la asistencia al cliente.

>[!NOTE]
>
>La programación de versiones es provisional y está sujeta a cambios. Póngase en contacto con el administrador de cuentas de Adobe o con el servicio de atención al cliente para obtener el programa de versiones actualizado.


## Asistencia y acceso al producto (sitios restringidos) {#product-access-and-support-restricted-sites}

Estos sitios solo están disponibles para los clientes. Si es cliente de y requiere acceso, póngase en contacto con su administrador de cuentas de Adobe.

* [](https://daycare.day.com) [Acceso a productos](https://login.marketing.adobe.com)

* [Servicio de atención al cliente de Adobe](https://helpx.adobe.com/contact.html)
