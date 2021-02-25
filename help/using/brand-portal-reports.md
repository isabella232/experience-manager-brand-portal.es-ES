---
title: Trabajar con informes
seo-title: Trabajar con informes
description: Los administradores de AEM Assets Brand Portal pueden crear informes de vista sobre el uso de Brand Portal y crear, administrar y vista de informes sobre los recursos descargados, caducados, publicados y compartidos a través de Brand Portal.
seo-description: Los administradores de AEM Assets Brand Portal pueden crear informes de vista sobre el uso de Brand Portal y crear, administrar y vista de informes sobre los recursos descargados, caducados, publicados y compartidos a través de Brand Portal.
uuid: dc4e5275-a614-4b95-8c70-2b7e470c50a7
content-type: reference
topic-tags: administration
products: SG_EXPERIENCEMANAGER/Brand_Portal
discoiquuid: 7683074f-b6ea-42e0-a411-3b13eb88d1f2
translation-type: tm+mt
source-git-commit: 0e26e6ae38d7b62576bc1751965a71168ad8faf5
workflow-type: tm+mt
source-wordcount: '1023'
ht-degree: 2%

---


# Trabajar con informes {#work-with-reports}

La función de sistema de informes es fundamental para evaluar el uso de Brand Portal y para saber cómo interactúan los usuarios internos y externos con los recursos aprobados. Los administradores pueden realizar vistas en el informe Uso de Brand Portal, que siempre está disponible en la página Informes de recursos. Sin embargo, los informes de inicios de sesión de usuario y recursos descargados, caducados, publicados y compartidos mediante vínculos pueden generarse y verse desde la página Informes de recursos. Estos informes son útiles para analizar la implementación de recursos, lo que le permite derivar métricas de éxito clave para medir la adopción de recursos aprobados dentro y fuera de la organización.

La interfaz de administración de informes es intuitiva e incluye opciones y controles detallados para acceder a los informes guardados. Puede vista, descargar o eliminar informes desde la página Informes de recursos, donde se muestran todos los informes generados anteriormente.

## Informes de vista {#view-reports}

Para vista de un informe, siga estos pasos:

1. En la barra de herramientas de la parte superior, toque o haga clic en el logotipo de AEM para acceder a las herramientas administrativas.

   ![](assets/aemlogo.png)

1. En el panel Herramientas administrativas, haga clic en **[!UICONTROL Crear/administrar informes]** para abrir la página **[!UICONTROL Informes de recursos]**.

   ![](assets/access-asset-reports.png)

1. Acceda al informe **[!UICONTROL Uso]** y a otros informes generados desde la página Informes de recursos.

   >[!NOTE]
   >
   >El informe de uso es un informe predeterminado generado en Brand Portal. No se puede crear ni eliminar. Sin embargo, puede crear, descargar y eliminar los informes de descarga, caducidad, publicación, uso compartido de vínculos e inicios de sesión de usuario.

   Para vista de un informe, haga clic en el vínculo del informe. Como alternativa, seleccione el informe y toque o haga clic en el icono de Vista en la barra de herramientas.

   **[!UICONTROL Los]** informes de uso muestran información sobre el número de usuarios activos de Brand Portal, el espacio de almacenamiento ocupado por todos los recursos y el recuento total de recursos en Brand Portal. Los usuarios del portal de marca que no están asignados a ningún perfil de producto en el Admin Console se consideran usuarios inactivos y no se reflejan en el **[!UICONTROL Informe de uso]**.
El informe también muestra la capacidad permitida para cada una de estas métricas de información.

   ![](assets/usage-report.png)

   **[!UICONTROL El informe]** Registros de usuario proporciona información sobre los usuarios que iniciaron sesión en Brand Portal. El informe muestra los nombres para mostrar, los ID de correo electrónico, las personas (administrador, visor, editor, invitado), los grupos, el último inicio de sesión, el estado de la actividad y el recuento de inicio de sesión de cada usuario desde la implementación de Brand Portal 6.4.2 hasta el momento de la generación del informe.

   ![](assets/user-logins.png)

   **** Descargue listas de informes y detalles sobre todos los recursos descargados en un intervalo de fecha y hora específico.

   ![](assets/download-report.png)

   >[!NOTE]
   >
   >El informe **[!UICONTROL Descargar]** recursos muestra solamente los recursos que se seleccionaron y descargaron de forma individual desde Brand Portal. Si un usuario ha descargado una carpeta que contiene recursos, el informe no muestra la carpeta ni los recursos que contiene.

   **** CaducidadInforme lista y detalla todos los recursos que han caducado en un intervalo de tiempo específico.

   ![](assets/expiration-report.png)

   **** Publicar listas de informes y proporciona información sobre todos los recursos que se publican de AEM a Brand Portal en un intervalo de tiempo específico.

   ![](assets/publish-report.png)

   >[!NOTE]
   >
   >Publicar informe no muestra información sobre fragmentos de contenido, ya que los fragmentos de contenido no se pueden publicar en Brand Portal.

   **[!UICONTROL Los]** informes de Uso compartido de vínculos muestran todos los recursos compartidos a través de los vínculos de la interfaz de Brand Portal en un intervalo de tiempo específico. El informe también indica cuándo se compartió el recurso mediante un vínculo, por qué usuario, cuándo caduca el vínculo y el número de vínculos compartidos para el inquilino (y los usuarios con los que se compartió el vínculo del recurso). Las columnas del informe de uso compartido de vínculos no se pueden personalizar.

   ![](assets/link-share-report.png)

   >[!NOTE]
   >
   >El informe de uso compartido de vínculos no muestra a los usuarios que tienen acceso al recurso compartido a través del vínculo o que han descargado el recurso a través del vínculo.
   >
   >Para rastrear las descargas a través del vínculo compartido, debe generar un informe de descarga después de seleccionar la opción **[!UICONTROL Solo vincular descargas]** en la página **[!UICONTROL Crear informe]**. Sin embargo, el usuario (descargado por) es anónimo en este caso.

## Generar informes {#generate-reports}

Los administradores pueden generar y administrar los siguientes informes estándar, una vez generados, se guardan para [obtener acceso a ellos](../using/brand-portal-reports.md#main-pars-header) más adelante:

* Inicios de sesión de usuario
* Descargar
* Vencimiento
* Publicación
* Vínculos compartidos

Las columnas del informe Descargar, Caducidad y Publicar se pueden personalizar para su visualización. Para generar un informe, siga estos pasos:

1. En la barra de herramientas de la parte superior, toque o haga clic en el logotipo de AEM para acceder a las herramientas administrativas.

1. En el panel Herramientas administrativas, toque o haga clic **[!UICONTROL Crear/Administrar informes]** para abrir la página **[!UICONTROL Informes de recursos]**.

   ![](assets/asset-reports.png)

1. En la página Informes de recursos, pulse o haga clic en **[!UICONTROL Crear]**.
1. En la página **[!UICONTROL Crear informe]**, seleccione un informe para crear y toque o haga clic en **[!UICONTROL Siguiente]**.

   ![](assets/crete-report.png)

1. Configure los detalles del informe. Especifique el título, la descripción, la estructura de carpetas (donde el informe necesita ejecutar y generar estadísticas) y el intervalo de fechas para los informes **[!UICONTROL Descargar]**, **[!UICONTROL Caducidad]** y **[!UICONTROL Publicar]**.

   ![](assets/create-report-page.png)

   Mientras que **[!UICONTROL Informe de uso compartido de vínculos]** solo necesita los parámetros de título, descripción e intervalo de fechas.

   ![](assets/create-link-share-report.png)

   >[!NOTE]
   >
   >Los caracteres especiales # y % en el título del informe se sustituyen por un guión (-) en la generación del informe.

1. Toque o haga clic **[!UICONTROL Siguiente]** para configurar las columnas de los informes Descargar, Caducidad y Publicar.
1. Seleccione o anule la selección de las casillas de verificación correspondientes según sea necesario. Por ejemplo, para asignar nombres de vista a los usuarios (que descargaron recursos) en el informe **[!UICONTROL Descargar]**, seleccione **[!UICONTROL Descargado por]**. La siguiente imagen ilustra la selección de columnas predeterminadas en el informe Descargar.

   ![](assets/createdownloadreport.png)

   También puede agregar columnas personalizadas a estos informes para mostrar más datos para sus requisitos personalizados.

   Para agregar columnas personalizadas al informe Descargar, Publicar o Caducidad, siga estos pasos:

   1. Para mostrar una columna personalizada, toque o haga clic **[!UICONTROL Añadir]** dentro de [!UICONTROL Columnas personalizadas].
   1. Especifique el nombre de la columna en el campo **[!UICONTROL Nombre de columna]**.
   1. Seleccione la propiedad a la que debe asignarse la columna mediante el selector de propiedades.

      ![](assets/property-picker.png)
También puede escribir la ruta en el campo de ruta de la propiedad.

      ![](assets/property-path.png)

      Para agregar más columnas personalizadas, toque o haga clic **Añadir** y repita los pasos 2 y 3.

1. Toque o haga clic en **[!UICONTROL Crear]**. Un mensaje notifica que se ha iniciado la generación de informes.

## Descargar informes {#download-reports}

Para guardar y descargar un informe como archivo .csv, realice una de las siguientes acciones:

* Seleccione un informe en la página Informes de recursos y toque o haga clic en **[!UICONTROL Descargar]** en la barra de herramientas de la parte superior.

![](assets/download-asset-report.png)

* En la página Informes de recursos, abra un informe. Seleccione la opción **[!UICONTROL Descargar]** en la parte superior de la página del informe.

![](assets/download-report-fromwithin.png)

## Eliminar informes {#delete-reports}

Para eliminar un informe existente, seleccione el informe en la página **[!UICONTROL Informes de recursos]** y toque o haga clic **[!UICONTROL Eliminar]** en la barra de herramientas de la parte superior.

>[!NOTE]
>
>**[!UICONTROL No se puede eliminar]** el informe de usuario.
