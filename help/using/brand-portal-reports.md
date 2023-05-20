---
title: Trabajar con informes
seo-title: Work with reports
description: Los administradores de Experience Manager Assets Brand Portal pueden ver informes sobre el uso de Brand Portal y crear, administrar y ver informes sobre los recursos descargados, caducados, publicados y compartidos a través de Brand Portal.
seo-description: Experience Manager Assets Brand Portal Administrators can view report about Brand Portal usage, and create, manage, and view reports around assets downloaded, expired, published, and link shared through Brand Portal.
uuid: dc4e5275-a614-4b95-8c70-2b7e470c50a7
content-type: reference
topic-tags: administration
products: SG_EXPERIENCEMANAGER/Brand_Portal
discoiquuid: 7683074f-b6ea-42e0-a411-3b13eb88d1f2
role: Admin
exl-id: 03d0292c-23c2-4ea0-9781-eb27768e6c33
source-git-commit: 955cd8afe939ff47e9f08f312505e230e2f38495
workflow-type: tm+mt
source-wordcount: '996'
ht-degree: 2%

---

# Trabajar con informes {#work-with-reports}

La capacidad de creación de informes es fundamental para evaluar el uso de Brand Portal y conocer cómo los usuarios internos y externos interactúan con los recursos aprobados. Los administradores pueden ver el Informe de uso de Brand Portal, que siempre está disponible en la página Informes de recursos. Sin embargo, los informes de inicios de sesión de usuarios y recursos descargados, caducados, publicados y compartidos a través de vínculos se pueden generar y ver desde la página Informes de recursos. Estos informes son útiles para analizar la implementación de recursos, lo que le permite derivar métricas de éxito clave para medir la adopción de recursos aprobados dentro y fuera de la organización.

La interfaz de administración de informes es intuitiva e incluye opciones y controles específicos para acceder a los informes guardados. Puede ver, descargar o eliminar informes desde la página Informes de recursos, en la que se muestran todos los informes generados anteriormente.

## Ver informes {#view-reports}

Para ver un informe, siga estos pasos:

1. En la barra de herramientas de la parte superior, pulse o haga clic en el logotipo del Experience Manager para acceder a las herramientas administrativas.

   ![](assets/aemlogo.png)

1. En el panel Herramientas administrativas, haga clic en **[!UICONTROL crear/administrar informes]** para abrir **[!UICONTROL los informes]** de recursos página.

   ![](assets/access-asset-reports.png)

1. Acceda al **[!UICONTROL Informe de uso]** y otros informes generados desde los informes de recursos página.

   >[!NOTE]
   >
   >El informe de uso es un informe predeterminado generado en Brand portal. No se puede crear ni eliminar. Sin embargo, puede crear, descargar y eliminar los informes de inicios de sesión de descarga, caducidad, Publish, vínculo compartido y usuario.

   Para vista un informe, haga clic en el vincular del informe. De lo contrario, seleccione el informe y pulse o haga clic en el icono de Ver desde la barra de herramientas.

   **[!UICONTROL Informe de uso]** muestra información sobre la cantidad de usuarios activos de Brand Portal, el espacio de almacenamiento ocupado por todos los recursos y el recuento total de recursos en Brand Portal. Los usuarios de Brand Portal que no están asignados a ningún perfil de producto en el Admin Console se consideran usuarios inactivos y no se reflejan en la variable **[!UICONTROL Informe de uso]**.
El informe también muestra la capacidad permitida para cada una de estas métricas de información.

   ![](assets/usage-report.png)

   **[!UICONTROL Inicios de sesión de usuario]** Este informe proporciona información sobre los usuarios que iniciaron sesión en Brand Portal. El informe muestra los nombres para mostrar, los ID de correo electrónico, los perfiles (administrador, visor, editor, invitado), los grupos, el último inicio de sesión, el estado de actividad y el recuento de inicios de sesión de cada usuario desde la implementación de Brand Portal 6.4.2 hasta el momento de la generación del informe.

   ![](assets/user-logins.png)

   **[!UICONTROL Descargar]** lista de informes y detalles sobre todos los recursos descargados en un intervalo de fecha y hora específico.

   ![](assets/download-report.png)

   >[!NOTE]
   >
   >Los activos **[!UICONTROL Descargar]** El informe muestra solo los recursos seleccionados y descargados individualmente desde Brand Portal. Si un usuario ha descargado una carpeta que contiene recursos, el informe no muestra la carpeta ni los recursos dentro de la carpeta.

   **[!UICONTROL Caducidad]** El informe enumera y detalla todos los recursos que caducaron en un lapso de tiempo específico.

   ![](assets/expiration-report.png)

   **[!UICONTROL Publish]** El informe muestra y proporciona información sobre todos los recursos publicados de Experience Manager Assets en Brand Portal en un lapso de tiempo específico.

   ![](assets/publish-report.png)

   >[!NOTE]
   >
   >Publicar informe no muestra información sobre los fragmentos de contenido, ya que estos no se pueden publicar en Brand Portal.

   **[!UICONTROL Informe de vínculos compartidos]** enumera todos los recursos compartidos a través de vínculos desde la interfaz de Brand Portal en un lapso de tiempo específico. El informe también informa de cuándo se compartió el recurso mediante un vínculo, por qué usuario, cuándo caduca el vínculo y el número de vínculos compartidos para el inquilino (y los usuarios con los que se compartió el vínculo del recurso). Las columnas del informe de vínculos compartidos no se pueden personalizar.

   ![](assets/link-share-report.png)

   >[!NOTE]
   >
   >El informe Compartir vínculos no muestra los usuarios que tienen acceso al recurso compartido mediante el vínculo o que lo han descargado a través del vínculo.
   >
   >Para rastrear descargas a través del vínculo compartido, debe generar el informe de descarga después de seleccionar **[!UICONTROL Solo descargas de Link Share]** opción activada **[!UICONTROL Crear informe]** página. Sin embargo, el usuario (Descargado por) es anónimo en este caso.

## Generación de informes {#generate-reports}

Los administradores pueden generar y administrar los siguientes informes estándar. Una vez generados, se guardan para [accedido](../using/brand-portal-reports.md#main-pars-header) más tarde:

* Inicios de sesión de usuario
* Descargar
* Vencimiento
* Publicación
* Vínculos compartidos

Las columnas del informe de descarga, caducidad y Publish se pueden personalizar para su visualización. Para generar un informe, seguir estos pasos:

1. En la barra de herramientas de la parte superior, pulse o haga clic en el logotipo del Experience Manager para acceder a las herramientas administrativas.

1. En el panel de herramientas administrativas, pulse o haga clic en **[!UICONTROL Crear/administrar informes]** para abrir **[!UICONTROL Informes de recursos]** página.

   ![](assets/asset-reports.png)

1. En la página Informes de recursos, pulse o haga clic en **[!UICONTROL Crear]**.
1. Desde el **[!UICONTROL Crear informe]** , seleccione un informe para crear y pulse o haga clic en él **[!UICONTROL Siguiente]**.

   ![](assets/crete-report.png)

1. Configure los detalles del informe. Especifique el título, la descripción, la estructura de carpetas (donde informe debe ejecutar y generar estadísticas) y intervalo de fecha para la descarga, caducidad e informes de **[!UICONTROL Publish]** . **** ****

   ![](assets/create-report-page.png)

   Mientras que, **[!UICONTROL Informe de vínculos compartidos]** solo necesita los parámetros título, descripción e intervalo de fechas.

   ![](assets/create-link-share-report.png)

   >[!NOTE]
   >
   >Los caracteres especiales # y % del título del informe se sustituyen por un guión (-) en la generación del informe.

1. Pulse o haga clic en **[!UICONTROL Siguiente]**, para configurar las columnas de los informes Descargar, Caducidad y Publicar.
1. Seleccione o anule la selección de las casillas de verificación adecuadas según sea necesario. Por ejemplo, para ver los nombres de los usuarios (que descargaron recursos) en **[!UICONTROL Descargar]** informe, seleccione **[!UICONTROL Descargado por]**. La siguiente imagen ilustra la selección de columnas predeterminadas en Descargar informe.

   ![](assets/createdownloadreport.png)

   También puede agregar columnas personalizadas a estos informes para mostrar más datos para sus requisitos personalizados.

   Para agregar columnas personalizadas para descargar, Publish o un informe de caducidad, seguir estos pasos:

   1. Para mostrar una columna personalizada, toque o haga clic **[!UICONTROL en Añadir]** dentro de [!UICONTROL  las columnas ] personalizadas.
   1. Especifique el nombre de la columna en **[!UICONTROL el campo nombre]** de columna.
   1. Seleccione la Propiedad a la que debe asignarse la columna, utilizando el selector de Propiedad.

      ![](assets/property-picker.png)De forma alternativa, escriba la ruta en el campo Propiedad ruta de acceso.

      ![](assets/property-path.png)

      Para agregar más columnas personalizadas, toque o haga clic en **Añadir** y repita los pasos 2 y 3.

1. Toque o haga clic en **[!UICONTROL Crear]**. Un mensaje notifica que se ha iniciado la generación del informe.

## Descargar informes {#download-reports}

Para guardar y descargar un informe como archivo .csv, siga uno de estos procedimientos:

* Seleccione un informe en la página Informes de recursos y pulse o haga clic en él **[!UICONTROL Descargar]** en la barra de herramientas de la parte superior.

![](assets/download-asset-report.png)

* En la página Informes de recursos, abra un informe. Seleccionar **[!UICONTROL Descargar]** en la parte superior de la página del informe.

![](assets/download-report-fromwithin.png)

## Eliminar informes {#delete-reports}

Para eliminar un informe existente, selecciónelo en **[!UICONTROL Informes de recursos]** y pulse o haga clic en **[!UICONTROL Eliminar]** en la barra de herramientas de la parte superior.

>[!NOTE]
>
>**[!UICONTROL Uso]** no se puede eliminar el informe.
