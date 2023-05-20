---
title: Preguntas frecuentes
seo-title: null
description: Obtenga información sobre las preguntas más frecuentes de Adobe Experience Manager Assets Brand Portal.
seo-description: null
uuid: null
content-type: reference
contentOwner: Vishabh Gupta
topic-tags: frequently-asked-questions
products: SG_EXPERIENCEMANAGER/Brand_Portal
discoiquuid: null
exl-id: 4a8f7fbd-7485-421d-a8db-755324d2dbef
source-git-commit: 4caa4263bd74b51af7504295161c421524e51f0c
workflow-type: tm+mt
source-wordcount: '1509'
ht-degree: 0%

---

# Preguntas frecuentes  {#frequently-asked-questions}

Las preguntas más frecuentes de Brand Portal se centran en las consultas y problemas que pueden encontrar los usuarios finales al trabajar con la última versión de Experience Manager Assets Brand Portal 6.4.6 o versiones anteriores.


## Preguntas frecuentes sobre Brand Portal 6.4.6  {#faqs-bp646}

**Preguntas. El punto final de OAuth heredado existente (`https://legacy-oauth.cloud.adobe.io/login`) no funciona. ¿Cuál podría ser la posible razón?**

**Ans.** La configuración OAuth heredada está obsoleta. Debe actualizar las instancias de autor de Experience Manager Assets al Service Pack más reciente y configurarlo mediante la consola de Adobe Developer. Consulte [Configuración de Experience Manager Assets con Brand Portal](configure-aem-assets-with-brand-portal.md) para obtener más información. Sin embargo, para que la configuración de OAuth anterior funcione hasta que actualice, actualice el extremo de OAuth heredado a `https://hypnosisprod.ethos11-prod-or1.ethos.adobe.net/` .

<!--
**Ques. I have created a collection using the asset link shared by the administrator. But I am unable to create a share link for my collection. Do I need special permissions to do this?**

**Ans.** The functionality is by design, the viewer users are not permitted to share link for collections as they have limited privileges due to which they cannot add users to create a share link. It is a known issue that the share link for collections is currently visible to the viewer users. This issue will be fixed in the upcoming release, the option to share link for the collections will not be available to the viewer users.    
-->

**Colas. No puedo publicar la carpeta de contribución activos de Brand portal a Experience Manager Assets después de actualizar a Adobe Systems consola de desarrollador. Mi instancia de autor está en Experience Manager Assets 6.5.4. ¿Cuál podría ser la razón posible?**

**Ans.** Sí, hay un problema conocido durante la publicación activos de la carpeta de contribución para Experience Manager Assets 6.5.4 mediante Adobe Systems consola de desarrollador.

El problema se corrigió en Experience Manager Assets 6.5.5. Puede actualizar el Experience Manager Assets instancia al último Service Pack y [ actualizar las configuraciones ](https://experienceleague.adobe.com/docs/experience-manager-65/assets/brandportal/configure-aem-assets-with-brand-portal.html#upgrade-integration-65) en Adobe Systems consola de desarrollador.

<!--
Broken link of download hotfix, comment out this section until we have the latest URL.

For immediate fix on AEM 6.5.4, it is recommended to [download the hotfix](https://www.adobeaemcloud.com/content/marketplace/marketplaceProxy.html?packagePath=/content/companies/public/adobe/packages/cq650/hotfix/cq-6.5.0-hotfix-33041) and install on your AEM author instance.
-->

**Preguntas. No veo el contenido de la carpeta Contribution publicado desde Brand Portal en Experience Manager Assets. ¿Cuál podría ser la posible razón?**

**Ans.** Póngase en contacto con el administrador de Experience Manager Assets para comprobar las configuraciones y asegurarse de que el inquilino de Brand Portal esté configurado solo con una instancia de autor de Experience Manager Assets.

Este problema posiblemente se produce cuando se ha configurado un inquilino de Brand portal en varias instancias de autor de Experience Manager Assets. Por ejemplo, el administrador configura el mismo inquilino de Brand portal en la Experience Manager Assets autor instancia de los entorno de ensayo y producción. En este caso, el recurso Publishing triggers in Brand portal, pero el Experience Manager Assets autor instancia no ha podido importar la recurso Coz el agente de replicación no recibe el token de solicitud.


**Preguntas. No puedo publicar recursos de Experience Manager Assets en Brand Portal. El registro de replicación indica que se agotó el tiempo de espera de la conexión. ¿Hay alguna solución rápida?**

**Ans.** Normalmente, la publicación falla con un error de tiempo de espera si hay varias solicitudes pendientes en la cola de replicación. Para resolver este problema, asegúrese de que los agentes de replicación estén configurados para evitar el tiempo de espera.

Realice los siguientes pasos para configurar el agente de replicación:

1. Inicie sesión en la instancia de autor de Experience Manager Assets.
1. Desde el **Herramientas** panel, vaya a **[!UICONTROL Implementación]** > **[!UICONTROL Replicación]**.
1. En la página Replicación, haga clic en **[!UICONTROL Agentes en el autor]**. Puede ver los cuatro agentes de replicación para su inquilino de Brand Portal.
1. Haga clic en la URL del agente de replicación para abrir los detalles del agente.
1. Clic **[!UICONTROL Editar]** para modificar la configuración del agente de replicación.
1. En Configuración de agente, haga clic en **[!UICONTROL Extendido]** pestaña.
1. Seleccione el **[!UICONTROL Cerrar conexión]** casilla de verificación.
1. Repita los pasos del 4 al 7 para configurar los cuatro agentes de replicación.
1. Reinicie el servidor y compruebe la conexión.


## Preguntas frecuentes sobre Brand Portal 6.4.5  {#faqs-bp645}

**Preguntas. ¿Cuál es el cambio más importante en la versión 6.4.5 de Brand Portal?**

**Ans.** Experience Manager Assets Brand Portal 6.4.5 es una versión de funcionalidades que permite a los usuarios de Brand Portal cargar contenido desde la instancia de Brand Portal y volver a publicar la carpeta Contribution en Experience Manager Assets sin necesidad de derechos de administrador.
Para obtener más información, consulte [Abastecimiento de recursos en Brand Portal](brand-portal-asset-sourcing.md).



**Preguntas. ¿Perderé el acceso a algún recurso, función o configuración existente que haya creado?**

**Ans.** Todas las funciones y configuraciones existentes permanecen intactas. Los usuarios finales no se verán afectados y el contenido permanecerá intacto.



**Preguntas. ¿Cuándo me voy a trasladar a la nueva versión de Brand Portal?**

**Ans.** Brand Portal 6.4.5 entró en producción en octubre de 2019. Y se espera que la próxima versión de Brand Portal se publique en el tercer trimestre de 2020.
Para actualizaciones y cambios de versión, se recomienda realizar un seguimiento de la [Notas de versión](brand-portal-release-notes.md) y [Novedades de Brand Portal.](whats-new.md).



**Preguntas. ¿Se verán afectados mis usuarios?**

**Ans.** La versión de Brand Portal 6.4.5 se realiza exclusivamente en Brand Portal, por lo que no afecta a los usuarios finales.



**Preguntas. ¿Se requiere alguna acción por mi parte como usuario de Brand Portal?**

**Ans.** La versión 6.4.5 de Brand Portal incluye una nueva función llamada Abastecimiento de recursos. El administrador debe configurar la función de obtención de recursos en Experience Manager Assets para habilitar dicha función para los usuarios de Brand Portal. Para obtener más información, consulte [Activar Abastecimiento de recursos](brand-portal-asset-sourcing.md).



**Preguntas. ¿Quién puede crear una carpeta Contribution?**

**Ans.** Cualquier usuario de Experience Manager Assets que tenga permisos para crear una nueva carpeta en Experience Manager Assets puede crear una **Contribución** carpeta. Para crear un **Contribución** carpeta, crear una nueva carpeta de tipo **Contribución de recursos**.
Esta carpeta se comparte con los usuarios activos de Brand Portal para que contribuyan.



**Preguntas. ¿Qué contiene una carpeta Contribution?**

**Ans.** **Contribución** La carpeta contiene dos subcarpetas **NUEVO** y **COMPARTIDO**. Inicialmente, la carpeta NUEVA está en blanco y la carpeta COMPARTIDA contiene el contenido de referencia (recursos reutilizables) para los usuarios de Brand Portal.
Los usuarios de Brand Portal acceden a **Contribución** y cargue contenido en la carpeta **NUEVO** carpeta.



**Preguntas.  ¿Puedo modificar el nombre de una carpeta Contribution existente?**

**Ans.** **No**, no puede modificar el nombre de un existente **Contribución** carpeta.



**Preguntas. ¿Qué es la contribución de requisitos de recursos w.r.t?**

**Ans.** El **Breve** documento adjunto al **Contribución** y el contenido de referencia (recursos reutilizables) cargados en la carpeta **COMPARTIDO** Esta carpeta ayuda al usuario de Brand Portal a comprender las necesidades de contribución y las expectativas como colaborador, y se denomina colectivamente como requisitos de recursos.



**Preguntas. ¿Puedo cargar recursos en cualquier carpeta permitida?**

**Ans.** No todas las carpetas permitidas. El usuario de un portal de marca puede cargar contenido únicamente a la **carpeta de contribución** que comparte el administrador de assets o del portal Experience Manager de marca.



**Colas. ¿Cómo puedo obtener acceso a una carpeta de contribución?**

**Ans.** Puede acceder a una carpeta de **contribución** solo si se ha compartido con usted. Recibirá un notificación correo electrónico/pulso cada vez que comparta una carpeta de contribución. Puede acceder a la carpeta de contribución a través de la vincular compartidos en el correo electrónico, o inicio de sesión al portal de marca instancia y navegar al icono de Bell para notfication para acceder a la carpeta de contribución.

>[!NOTE]
>
>Si no es un usuario de Brand Portal existente, solicite al administrador de Experience Manager Assets que cree su usuario en Admin Console y agregue su perfil al archivo de configuración de usuario en la lista de usuarios de Brand Portal.

**Preguntas. ¿Cuál es el formato del archivo de CSV para usuario importación?**

**Ans.** La formato es la misma que la que admite Admin Console para la importación masiva usuario. El correo electrónico, el nombre y los apellidos son obligatorios.



**Colas. ¿Qué rellena la lista de usuarios (colaboradores de Brand Portal) en la lista desplegable de usuarios de contribución de recursos?**

**Ans.** Los usuarios de la lista desplegable se rellenan desde el archivo de configuración de usuario de Brand Portal (.csv) cargado en Experience Manager Assets.



**Preguntas. ¿Dónde puedo ver el estado de los trabajos de importación y publicación?**

**Ans.** En Experience Manager Assets, puede ver el estado de una importación en **asíncrona** página de trabajo. En Brand Portal, puede ver el estado de un trabajo de publicación en **[!UICONTROL Herramientas > Estado de contribución de recursos]**.



**Preguntas. ¿Cuál es la frecuencia de un trabajo de importación que se ejecuta periódicamente en Experience Manager?**

**Ans.** En Experience Manager Assets, el sondeo se ejecuta cada 5 minutos.



**Preguntas. ¿Hay algún umbral en la cantidad de veces que una carpeta se puede publicar desde Brand Portal a Experience Manager Assets?**

**Ans.** No, todos los recursos del **NUEVO** Las carpetas de se publican en Experience Manager Assets independientemente de si se publicaron anteriormente. Cada vez que **Contribución** se publica desde Brand Portal en Experience Manager Assets, anula el contenido de la **NUEVO** carpeta.



**Preguntas. ¿Cómo se cargan nuevos recursos en una carpeta Contribution?**

**Ans.** Consulte la documentación detallada para [Cargando recursos a la carpeta Contribution](brand-portal-publish-contribution-folder-to-brand-portal.md).



**Preguntas. ¿No veo miniaturas o vistas previas en los recursos cargados en la carpeta NUEVA por un usuario de Brand Portal?**

**Ans.** Es como está diseñado, ya que no hay ningún flujo de trabajo que se ejecute en el extremo de Brand Portal.



**Preguntas. ¿Qué sucede si se publica una carpeta de Experience Manager Assets a Brand Portal que está en proceso de cambio?**

**Ans.** En Experience Manager Assets, los registros se mantienen cada vez que se publica una carpeta en Brand Portal. En el momento de la publicación, todos los recursos que no se publican en Brand Portal se colocan en una cola de replicación. Los recursos agregados a la carpeta después de activarse el trabajo de publicación no se publican en Brand Portal. Cuando el usuario de Experience Manager Assets vuelve a publicar la carpeta, solo los recursos que no se publicaron anteriormente (existentes en la cola de replicación) se publican en Brand Portal.
Esto se aplica a cualquier carpeta publicada desde Experience Manager Assets a Brand Portal y a una carpeta COMPARTIDA dentro de una carpeta Contribution.

**Preguntas. ¿Con quién debo contactar si tengo alguna pregunta?**

**Ans.** Póngase en contacto con el administrador de cuentas de Adobe o con Atención al cliente.

>[!NOTE]
>
>La programación de versiones es provisional y está sujeta a cambios. Póngase en contacto con el administrador de cuentas de Adobe o con la asistencia al cliente para obtener la programación de versiones actualizada.


## Acceso y asistencia de productos (sitios restringidos) {#product-access-and-support-restricted-sites}

Estos sitios solo están disponibles para los clientes de. Si es cliente y necesita acceso, póngase en contacto con el administrador de cuentas de Adobe.

<!--
* [](https://daycare.day.com) [Product Access](https://login.marketing.adobe.com)

* [Adobe Customer Support]()
-->
