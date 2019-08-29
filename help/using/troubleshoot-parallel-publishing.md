---
title: Solución de problemas en la publicación paralela en Brand Portal
seo-title: Solución de problemas en la publicación paralela en Brand Portal
description: Solución de problemas de publicación paralela.
seo-description: Solución de problemas de publicación paralela.
uuid: 51 e 45 cca -8 c 96-4 c 69-84 ef -2 ef 34 f 3 bcde 2
products: SG_ EXPERIENCEMANAGER/Brand_ Portal
content-type: referencia
topic-tags: brand-portal
discoiquuid: a 4801024-b 509-4 c 51-afd 8-e 337417 e 658 b
translation-type: tm+mt
source-git-commit: 770c353b1143d879280df310012ce9d4d30b40c9

---


# Solución de problemas en la publicación paralela en Brand Portal {#troubleshoot-issues-in-parallel-publishing-to-brand-portal}

[!DNL Brand Portal] admite la integración con [!DNL AEM Assets] los recursos de marca aprobados que se ingestan (o publican) perfectamente desde la instancia de autor de AEM Assets. Una vez [integrado](https://helpx.adobe.com/experience-manager/6-5/assets/using/brand-portal-configuring-integration.html), [!DNL AEM] Autor utiliza un agente de replicación para replicar los recursos seleccionados en [!DNL Brand Portal] el servicio de nube para el uso aprobado por [!DNL Brand Portal] los usuarios. Se utilizan [!DNL AEM 6.2 SP1-CFP5]varios agentes de replicación, [!DNL AEM CFP 6.3.0.2]y después, para permitir publicación paralela de alta velocidad.

>[!NOTE]
>
>Adobe recomienda actualizar a [!DNL AEM 6.4.1.0] para garantizar [!DNL AEM Assets Brand Portal] que se integra correctamente con Recursos AEM. Una limitación en [!DNL AEM 6.4] proporciona un error mientras se produce un error al configurar la integración con Brand Portal y la replicación.

Al configurar el servicio de nube para el portal de marca en [!UICONTROL /etc/cloudservice], todos los usuarios y token necesarios se generan automáticamente y se guardan en el repositorio. Se crea la configuración de servicio de nube, se crean los usuarios de servicio requeridos para replicaciones y agentes de replicación para reproducir el contenido. Esto crea cuatro agentes de replicación. Por lo tanto, cuando publica numerosos recursos [!DNL AEM] desde [!DNL Brand Portal], estos se ponen en cola y se distribuyen entre estos agentes de replicación a través de Round Robin.

Sin embargo, la publicación puede fallar intermitentemente debido a trabajos de sling grandes, a una mayor red y a un disco [!UICONTROL o a una instancia de disco] en [!DNL AEM] la instancia de autor o al ralentizar el rendimiento de la instancia [!DNL AEM] de autor. Por lo tanto, es aconsejable probar la conexión con los agentes de replicación antes de comenzar a publicar.

![](assets/test-connection.png)

## Solución de errores en la primera publicación: Validación de la configuración de publicación {#troubleshoot-failures-in-first-time-publishing-validating-your-publish-configuration}

Para validar las configuraciones de publicación:

1. Comprobación de los registros de errores
2. Comprobar si se crea el agente de replicación
3. Conexión de prueba

**Al crear el servicio Cloud**

Compruebe los registros de cola. Compruebe si el agente de replicación se ha creado o no. Si falla la creación del agente de replicación, edite el servicio en la nube realizando pequeños cambios en el servicio de nube. Valide y verifique de nuevo si se crea o no el agente de replicación. Si no es así, vuelva a editar el servicio.

Si al editar repetidamente el servicio en la nube no está configurado correctamente, informe de un ticket de Daycare.

**Conexión de comprobación con agentes de replicación**

Ver registro, si se encuentran errores en el registro de replicación:

1. Póngase en contacto con el servicio de asistencia de Adobe.

2. Vuelva a intentar [limpiar](../using/troubleshoot-parallel-publishing.md#clean-up-existing-config) y cree la configuración de publicación de nuevo.

<!--
Comment Type: remark
Last Modified By: Mini Gulati (mgulati)
Last Modified Date: 2018-06-21T22:56:21.256-0400
<p>?? check and compare public key. At times public key is different</p>
<p>?? another thing to check in /useradmin</p>
-->

### Limpieza de las configuraciones de publicación de Brand Portal {#clean-up-existing-config}

La mayoría de las veces cuando no funciona la publicación, el motivo puede ser que el usuario que está publicando (mac-&lt; tenantid &gt;-replicación) no tiene la clave privada más reciente y, por lo tanto, la publicación falla con "401 no autorizado" y no se informa ningún otro error en los registros de agente de replicación. Es posible que desee evitar la resolución de problemas y crear una nueva configuración en su lugar. Para que la nueva configuración funcione correctamente, debe limpiar lo siguiente desde la configuración del autor de AEM:

1. ir a [!UICONTROL localhost: 4502/crx/de] (asume que está ejecutando la instancia de autor en [!UICONTROL localhost: 4502]):\
   i delete [!UICONTROL /etc/replication/agents.author/mp_replication &amp; # 42];\
   ii delete [!UICONTROL /etc/cloudservices/mediaportal/ &lt; config_ name &amp; gt];

2. ir a [!UICONTROL localhost: 4502/useradmin]:\
   i search for user [!UICONTROL mac-&lt; tenantid &gt;-replication]\
   ii eliminar este usuario

Ahora el sistema se limpia. Ahora puede intentar crear una nueva configuración de Cloudservice y seguir usando [!DNL JWT] la aplicación existente en [https://legacy-oauth.cloud.adobe.io/](https://legacy-oauth.cloud.adobe.io/). No es necesario crear una aplicación nueva, sino que solo es necesario actualizar la clave pública desde la configuración de nube creada recientemente.

## Problema de visibilidad del inquilino de la conexión del desarrollador de la conexión {#developer-connection-jwt-application-tenant-visibility-issue}

Si se encuentran en [!UICONTROL https://legacy-oauth.cloud.adobe.io/](https://legacy-oauth.cloud.adobe.io/), se enumeran todas las orgs (inquilinos) para las que tienen los usuarios actuales. Si no encuentra el nombre de la organización aquí o no puede crear una aplicación para un inquilino requerido aquí, compruebe si dispone de suficientes derechos (administrador del sistema) para hacerlo.

Hay un problema conocido en esta interfaz de usuario que para cualquier inquilino solo se ven las 10 aplicaciones principales. Cuando cree la aplicación, permanezca en esa página y marque la URL. No es necesario que vaya a la página de lista de la aplicación y busque la aplicación que ha creado. Puede visitar esta URL con marcador directamente y actualizar o eliminar la aplicación cuando sea necesario.

Es posible que [!DNL JWT] la aplicación no esté enumerada correctamente. Por lo tanto, es aconsejable anotar o marcar la URL al crear la aplicación JWT.

## La configuración de ejecución deja de funcionar {#running-configuration-stops-working}

<!--
Comment Type: draft

<p>If the running configuration stops working, either of the following two possibilities
<g class="gr_ gr_15 gr-alert gr_gramm gr_inline_cards gr_run_anim Grammar multiReplace" data-gr-id="15" id="15" style="font-size: 12px;">
are
</g> there:</p>
<p>1.
<g class="gr_ gr_14 gr-alert gr_gramm gr_inline_cards gr_run_anim Grammar only-ins doubleReplace replaceWithoutSep" data-gr-id="14" id="14">
Connection
</g> has failed, or</p>
<p>2. Publish has failed with permission to dam-replication-service denied, while connection has passed </p>
<p>If the connection has failed [1], the
<g class="gr_ gr_10 gr-alert gr_spell gr_inline_cards gr_run_anim ContextualSpelling ins-del multiReplace" data-gr-id="10" id="10">
fail safe
</g> way to fix it is to <a href="../using/troubleshoot-parallel-publishing.md#main-pars-header-1664955658">clean up</a> the existing Brand Portal publish configuration and recreate a publish configuration. </p>
<p>However, if the
<g class="gr_ gr_18 gr-alert gr_spell gr_inline_cards gr_run_anim ContextualSpelling" data-gr-id="18" id="18">
publish
</g> has failed with
<g class="gr_ gr_16 gr-alert gr_gramm gr_inline_cards gr_run_anim Grammar only-ins doubleReplace replaceWithoutSep" data-gr-id="16" id="16">
permission
</g> denied to dam-replication-service, raise a support ticket.</p>
-->

Si un agente de replicación (que estaba publicando en Brand Portal simplemente) deja de procesar los trabajos de publicación, compruebe los registros de replicación. [!DNL AEM] se reintenta automáticamente, de modo que si una publicación de recurso en particular falla, se vuelve a probar automáticamente. Si hay algún problema intermitente como el error de red, puede suceder durante la reedición.

Sin embargo, si hay errores de publicación continuos y se bloquea la cola. a continuación, debe comprobar "conexión de prueba" e intentar resolver los errores que se generan.

En base a los errores, se recomienda registrar un ticket de asistencia técnica para que el equipo [!DNL Brand Portal] de ingeniería pueda resolver los problemas.
