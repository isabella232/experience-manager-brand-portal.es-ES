---
title: Solución de problemas en la publicación paralela de Brand Portal
seo-title: Solución de problemas en la publicación paralela de Brand Portal
description: Solucionar problemas de publicación paralela.
seo-description: Solucionar problemas de publicación paralela.
uuid: 51e45cca-8c96-4c69-84ef-2ef34f3bcde2
products: SG_EXPERIENCEMANAGER/Brand_Portal
content-type: reference
topic-tags: brand-portal
discoiquuid: a4801024-b509-4c51-afd8-e337417e658b
translation-type: tm+mt
source-git-commit: a502a60a7d93595a202d50a79e2374c8d9734486
workflow-type: tm+mt
source-wordcount: '892'
ht-degree: 2%

---


# Solución de problemas en la publicación paralela de Brand Portal {#troubleshoot-issues-in-parallel-publishing-to-brand-portal}

Brand Portal se ha configurado con AEM Assets para que los recursos de marca aprobados se transfieran (o publiquen) sin problemas desde la instancia de creación de AEM Assets. Una vez [configurado](../using/configure-aem-assets-with-brand-portal.md), AEM Author utiliza un agente de replicación para replicar los recursos seleccionados en el servicio en la nube de Brand Portal para que los usuarios de Brand Portal los usen de forma aprobada. Se utilizan varios agentes de replicación AEM 6.2 SP1-CFP5, AEM CFP 6.3.0.2 y versiones posteriores para permitir la publicación en paralelo de alta velocidad.

>[!NOTE]
>
>Adobe recomienda actualizar a AEM 6.4.1.0 para garantizar que AEM Assets Brand Portal se configure correctamente con AEM Assets. Una limitación en AEM 6.4 produce un error al configurar AEM Assets con Brand Portal y falla la replicación.

Al configurar el servicio en la nube para el portal de marca en **[!UICONTROL /etc/cloudservice]**, todos los usuarios y tokens necesarios se generan automáticamente y se guardan en el repositorio. Se crea la configuración del servicio en la nube, también se crean los usuarios de servicio necesarios para los agentes de replicación y replicación para replicar contenido. Esto crea cuatro agentes de replicación. Así que cuando publica numerosos recursos de AEM en Brand Portal, estos se ponen en cola y se distribuyen entre estos agentes de replicación a través de Round Robin.

Sin embargo, la publicación puede fallar de forma intermitente debido a los grandes trabajos de sling, el aumento de la red y de la **[!UICONTROL E/S de disco]** en la instancia de AEM Author o el menor rendimiento de la instancia de AEM Author. Por lo tanto, se recomienda probar la conexión con los agentes de replicación antes de comenzar a publicar.

![](assets/test-connection.png)

## Solucionar errores en la primera publicación: validación de la configuración de publicación {#troubleshoot-failures-in-first-time-publishing-validating-your-publish-configuration}

Para validar las configuraciones de publicación:

1. Compruebe los registros de errores
1. Compruebe si se ha creado el agente de replicación
1. Probar conexión

**Registros de seguimiento al crear Cloud Service**

Compruebe los registros de cola. Compruebe si se ha creado o no el agente de replicación. Si la creación del agente de replicación falla, edite el servicio en la nube realizando cambios menores en el servicio en la nube. Valide y vuelva a comprobar si el agente de replicación se ha creado o no. Si no es así, vuelva a editar el servicio.

Si al editar repetidamente el servicio en la nube no está configurado correctamente, informe de un ticket de guardería.

**Probar la conexión con los agentes de replicación**

Registro de vista, si se encuentran errores en el registro de replicación:

1. Póngase en contacto con la asistencia de Adobe.

1. Vuelva a intentar [limpiar](../using/troubleshoot-parallel-publishing.md#clean-up-existing-config) y cree de nuevo la configuración de publicación.

<!--
Comment Type: remark
Last Modified By: Mini Gulati (mgulati)
Last Modified Date: 2018-06-21T22:56:21.256-0400
<p>?? check and compare public key. At times public key is different</p>
<p>?? another thing to check in /useradmin</p>
-->

### Limpiar las configuraciones de publicación existentes de Brand Portal {#clean-up-existing-config}

La mayoría de las veces, cuando la publicación no funciona, el motivo puede ser que el usuario que está publicando (por ejemplo: `mac-<tenantid>-replication` no tiene la clave privada más reciente y, por lo tanto, la publicación falla con el error &quot;401 no autorizado&quot; y no se notifica ningún otro error en los registros del agente de replicación. Es posible que desee evitar la resolución de problemas y crear una nueva configuración. Para que la nueva configuración funcione correctamente, limpie lo siguiente de AEM configuración del autor:

1. Vaya a `localhost:4502/crx/de/` (teniendo en cuenta que está ejecutando la instancia de autor en localhost:4502:\
   i. delete `/etc/replication/agents.author/mp_replication`
ii. delete 
`/etc/cloudservices/mediaportal/<config_name>`

1. Vaya a localhost:4502/useradmin:\
   i. buscar usuario `mac-<tenantid>replication`
ii. eliminar este usuario

Ahora todo el sistema está limpio. Ahora puede intentar crear una nueva configuración de cloudservice y seguir usando la aplicación JWT ya existente en [https://legacy-oauth.cloud.adobe.io/](https://legacy-oauth.cloud.adobe.io/). No es necesario crear una nueva aplicación, sino que solo es necesario actualizar la clave pública desde la configuración de nube recién creada.

## Problema de visibilidad del inquilino de la aplicación JWT de conexión de desarrollador {#developer-connection-jwt-application-tenant-visibility-issue}

Si se encuentra en [https://legacy-oauth.cloud.adobe.io/](https://legacy-oauth.cloud.adobe.io/), se enumeran todas las organizaciones (inquilinos) para las que los usuarios actuales tienen administrador del sistema. Si no encuentra el nombre de la organización aquí o no puede crear una aplicación para un inquilino requerido aquí, compruebe si tiene suficientes derechos (administrador del sistema) para hacerlo.

Hay un problema conocido en esta interfaz de usuario que indica que para cualquier inquilino solo están visibles las 10 aplicaciones principales. Cuando cree la aplicación, permanezca en esa página y marque la dirección URL. No es necesario que vaya a la página de listado de la aplicación y busque la aplicación que ha creado. Puede visitar esta URL con marcador directamente y actualizar o eliminar la aplicación cuando sea necesario.

Es posible que la aplicación JWT no aparezca correctamente en la lista. Por lo tanto, se recomienda anotar o marcar la URL al crear la aplicación JWT.

## La ejecución de la configuración deja de funcionar {#running-configuration-stops-working}

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

Si un agente de replicación (que se estaba publicando en el portal de marca correctamente) detiene el procesamiento de los trabajos de publicación, compruebe los registros de replicación. AEM tiene incorporado un reintento automático, por lo que si falla una publicación de un recurso en particular, se volverá a intentar automáticamente. Si hay algún problema intermitente, como un error de red, podría suceder durante el reintento.

Si hay errores de publicación continuos y la cola está bloqueada, debe comprobar **[!UICONTROL conexión de prueba]** e intentar resolver los errores que se están notificando.

En función de los errores, se le aconseja que registre un ticket de asistencia técnica para que el equipo de ingeniería de Brand Portal pueda ayudarle a resolver los problemas.


## Configure los agentes de replicación para evitar el error de tiempo de espera de conexión {#connection-timeout}

Normalmente, el trabajo de publicación falla con un error de tiempo de espera si hay varias solicitudes pendientes en la cola de replicación. Para resolver este problema, asegúrese de que los agentes de replicación están configurados para evitar el tiempo de espera.

Realice los siguientes pasos para configurar los agentes de replicación:
1. Inicie sesión en la instancia de creación de AEM Assets.
1. En el panel **Herramientas**, vaya a **[!UICONTROL Implementación]** > **[!UICONTROL Replicación]**.
1. En la página Replicación, haga clic en **[!UICONTROL Agentes en el autor]**. Puede ver los cuatro agentes de replicación del inquilino de Brand Portal.
1. Haga clic en la dirección URL del agente de replicación para abrir los detalles del agente.
1. Haga clic en **[!UICONTROL Editar]** para modificar la configuración del agente de replicación.
1. En Configuración del agente, haga clic en la ficha **[!UICONTROL Extended]**.
1. Active la casilla de verificación **[!UICONTROL Cerrar conexión]**.
1. Repita los pasos 4 a 7 para configurar los cuatro agentes de replicación.
1. Reinicie el servidor.