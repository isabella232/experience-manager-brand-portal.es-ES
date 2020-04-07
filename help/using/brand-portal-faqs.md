---
title: Preguntas frecuentes
seo-title: null
description: Obtenga una visión detallada de las preguntas más frecuentes en el portal de marcas Adobe Experience Manager Assets.
seo-description: null
uuid: null
content-type: reference
contentOwner: Vishabh Gupta
topic-tags: frequently-asked-questions
products: SG_EXPERIENCEMANAGER/Brand_Portal
discoiquuid: null
translation-type: tm+mt
source-git-commit: 9169407bbbfabd94be31c89c028be64e55afc064

---


# Preguntas frecuentes {#frequently-asked-questions}

Las preguntas más frecuentes de Brand Portal se centran en las consultas y los problemas que pueden encontrar los usuarios finales al trabajar con la última versión de AEM Assets Brand Portal 6.4.5 o versiones anteriores.


## Preguntas más frecuentes sobre Brand Portal 6.4.6 {#faqs-bp646}

**Ques. El punto final (`https://legacy-oauth.cloud.adobe.io/login`) de OAuth heredado no funciona. ¿Cuál podría ser la razón posible?**

**Ans.** La configuración OAuth heredada está en desuso. Debe actualizar las instancias de creación de Recursos AEM al Service Pack más reciente y configurarlas con la E/S de Adobe. Consulte [Configuración de AEM Assets con Brand Portal](configure-aem-assets-with-brand-portal.md) para obtener más información. Sin embargo, para que la configuración OAuth heredada funcione hasta que se actualice, actualice el punto final OAuth heredado a `https://hypnosisprod.ethos11-prod-or1.ethos.adobe.net/`.

**Ques. No puedo publicar los recursos de la carpeta de contribución de Brand Portal en Recursos AEM después de actualizar a Adobe I/O. Mi instancia de autor se encuentra en AEM 6.5.4. ¿Cuál podría ser la razón posible?**

**Ans.** Sí, se conoce un problema al publicar los recursos de la carpeta de contribución en Recursos AEM en AEM 6.5.4 con Adobe I/O. Este problema se solucionará en el próximo Service Pack.

Para una corrección inmediata en AEM 6.5.4, se recomienda [descargar la revisión](https://www.adobeaemcloud.com/content/marketplace/marketplaceProxy.html?packagePath=/content/companies/public/adobe/packages/cq650/hotfix/cq-6.5.0-hotfix-33041) e instalarla en la instancia de creación de AEM.


## Preguntas más frecuentes sobre Brand Portal 6.4.5 {#faqs-bp645}

**Ques. ¿Cuál es el cambio más importante en la versión 6.4.5 de Brand Portal?**

**Ans.** AEM Assets Brand Portal 6.4.5 es una versión de funciones que permite a los usuarios de Brand Portal cargar contenido desde la instancia de Brand Portal y publicar la carpeta Contribution en AEM Assets sin necesidad de derechos de administrador.
Para obtener más información, consulte [Asset Sourcing en Brand Portal](brand-portal-asset-sourcing.md).



**Ques. ¿Perderé el acceso a los recursos, funciones o configuraciones existentes que haya creado?**

**Ans.** Todas las funciones y configuraciones existentes permanecen intactas. Los usuarios finales no se ven afectados y el contenido permanece intacto.



**Ques. ¿Cuándo me muevo a la nueva versión de Brand Portal?**

**Ans.** Brand Portal 6.4.5 se puso en marcha en octubre de 2019. Y se espera que la próxima versión de Brand Portal se publique en el tercer trimestre de 2020.
Para actualizaciones y cambios de versión, se recomienda realizar un seguimiento de las [Notas](brand-portal-release-notes.md) de la versión y de [las Novedades de Brand Portal](whats-new.md).



**Ques. ¿Se verán afectados mis usuarios?**

**Ans.** La versión de Brand Portal 6.4.5 se incluye exclusivamente en Brand Portal, por lo que no afecta a los usuarios finales.



**Ques. ¿Se requiere alguna acción por mi parte como usuario de Brand Portal?**

**Ans.** La versión 6.4.5 de Brand Portal incluye una nueva función denominada Asset Sourcing. El administrador de AEM debe configurar la función de fuente de recursos en Recursos AEM para habilitar la función para los usuarios de Brand Portal. Para obtener más información, consulte [Activar fuentes](brand-portal-configure-asset-sourcing.md)de recursos.



**Ques. ¿Quién puede crear una carpeta de contribución?**

**Ans.** Cualquier usuario de AEM que tenga permisos para crear una nueva carpeta en Recursos AEM puede crear una carpeta **de contribución** . Para crear una carpeta **Contribution** , cree una nueva carpeta de tipo **Asset Contribution**.
Esta carpeta se comparte con los usuarios activos de Brand Portal para obtener contribución.



**Ques. ¿Qué contiene una carpeta Contribution?**

**Ans.** La carpeta **Contribution** contiene dos subcarpetas **NUEVO** y **COMPARTIDO**. Inicialmente, la carpeta NEW está en blanco y la carpeta SHARED contiene el contenido de referencia (recursos reutilizables) para los usuarios de Brand Portal.
Los usuarios de Brand Portal acceden a la carpeta **Contribution** y cargan contenido en la carpeta **NEW** .



**Ques.  ¿Puedo modificar el nombre de una carpeta de contribución existente?**

**Ans.** **No**, no puede modificar el nombre de una carpeta de **contribución** existente.



**Ques. ¿Cuáles son los requisitos de activos con contribución de r.t?**

**Ans.** El **breve** documento adjunto a la carpeta **Contribution** y el contenido de referencia (recursos reutilizables) cargados en la carpeta **SHARED** ayuda al usuario de Brand Portal a comprender la necesidad de contribución y expectativas como colaborador, y se le denomina colectivamente como los requisitos de recursos.



**Ques. ¿Puedo cargar recursos en cualquier carpeta permitida?**

**Ans.** No todas las carpetas permitidas. Un usuario de Brand Portal solo puede cargar contenido en la carpeta **Contribution** que comparte el administrador de AEM o Brand Portal.



**Ques. ¿Cómo puedo obtener acceso a una carpeta de contribución?**

**Ans.** Solo puede acceder a una carpeta **de contribución** si se ha compartido con usted. Recibirá una notificación por correo electrónico/pulso cada vez que se comparta una carpeta de contribución con usted. Puede acceder a la carpeta Contribution mediante el vínculo compartido en el correo electrónico o iniciar sesión en la instancia de Brand Portal y navegar hasta el icono de campana para recibir notificaciones a fin de acceder a la carpeta Contribution.

>[!NOTE]
>
>Si no es un usuario de Brand Portal, solicite al administrador de AEM que cree su usuario en la consola de administración de AEM y añada su perfil al archivo de configuración de usuario de la lista de usuarios de Brand Portal. Consulte, [Añadir usuario](brand-portal-configure-asset-sourcing.md)de Brand Portal.



**Ques. ¿Cuál es el formato del archivo CSV para la importación del usuario?**

**Ans.** El formato es el mismo que el que admite la Consola de administración para la importación masiva de usuarios. El correo electrónico, el nombre y los apellidos son obligatorios.



**Ques. ¿Qué rellena la lista de usuarios (colaboradores de Brand Portal) en la lista desplegable de usuarios de contribución de recursos?**

**Ans.** Los usuarios de la lista desplegable se rellenan desde el archivo de configuración de usuario de Brand Portal (.csv) cargado en AEM.



**Ques. ¿Dónde puedo ver el estado de los trabajos de importación y publicación?**

**Ans.** En AEM, puede ver el estado de una importación en la página de trabajo **asincrónica** . En Brand Portal, puede ver el estado de un trabajo de publicación en **[!UICONTROL Herramientas > Estado]** de contribución de recursos.



**Ques. ¿Cuál es la frecuencia de un trabajo de importación que se ejecuta periódicamente en AEM?**

**Ans.** En AEM, las encuestas se ejecutan cada 5 minutos.



**Ques. ¿Existe algún umbral sobre el número de veces que se puede publicar una carpeta desde Brand Portal en Recursos AEM?**

**Ans.** No, todos los recursos de la carpeta **NEW** se publican en Recursos AEM, independientemente de que se hayan publicado anteriormente. Cada vez que se publica una carpeta de **contribución** de Brand Portal en Recursos AEM, se anula el contenido de la carpeta **NEW** .



**Ques. ¿Cómo cargar nuevos recursos en una carpeta de contribución?**

**Ans.** Consulte la documentación detallada para la [carga de recursos en la carpeta](brand-portal-upload-assets-to-contribution-folder.md)Contribution.



**Ques. ¿No veo miniaturas o previsualizaciones en los recursos cargados en la carpeta NEW por un usuario de Brand Portal?**

**Ans.** Está diseñado de la misma manera, ya que no se está ejecutando ningún flujo de trabajo en el extremo de Brand Portal.



**Ques. ¿Qué sucede si se publica una carpeta de Recursos AEM en Brand Portal que está en proceso de cambio?**

**Ans.** En AEM, los registros se mantienen cada vez que se publica una carpeta en Brand Portal. En el momento de la publicación, todos los recursos que no se publican en Brand Portal se colocan en una cola de replicación. Los recursos agregados a la carpeta después de activar el trabajo de publicación no se publican en Brand Portal. Cuando el usuario de AEM publica de nuevo la carpeta, solo se publican en Brand Portal los recursos que no se hayan publicado anteriormente (que ya están en la cola de replicación).
Esto se aplica a cualquier carpeta publicada desde Recursos AEM a Brand Portal y a la carpeta COMPARTIDA dentro de una carpeta Contribution.



**Ques. ¿Con quién puedo ponerme en contacto?**

**Ans.** Póngase en contacto con el administrador de cuentas de Adobe o con el servicio de asistencia al cliente.


>[!NOTE]
>
>La programación de versiones es provisional y está sujeta a cambios. Póngase en contacto con el administrador de cuentas de Adobe o con el servicio de asistencia al cliente para obtener la programación de versiones actualizada.




## Asistencia y acceso al producto (sitios restringidos) {#product-access-and-support-restricted-sites}

Estos sitios solo están disponibles para los clientes. Si es un cliente y necesita acceso, póngase en contacto con su administrador de cuentas de Adobe.

* [](https://daycare.day.com) Acceso [al producto](https://login.marketing.adobe.com)

* [Servicio de atención al cliente de Adobe](https://helpx.adobe.com/contact.html)
