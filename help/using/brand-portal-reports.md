---
title: Trabajar con informes
seo-title: Trabajar con informes
description: Los administradores de AEM Assets Brand Portal pueden ver el informe sobre el uso de Brand Portal y crear, gestionar y ver informes sobre recursos descargados, caducados, publicados y compartidos mediante Brand Portal.
seo-description: Los administradores de AEM Assets Brand Portal pueden ver el informe sobre el uso de Brand Portal y crear, gestionar y ver informes sobre recursos descargados, caducados, publicados y compartidos mediante Brand Portal.
uuid: dc 4 e 5275-a 614-4 b 95-8 c 70-2 b 7 e 470 c 50 a 7
content-type: referencia
topic-tags: administración
products: SG_ EXPERIENCEMANAGER/Brand_ Portal
discoiquuid: 7683074 f-b 6 ea -42 e 0-a 411-3 b 13 eb 88 d 1 f 2
translation-type: tm+mt
source-git-commit: 32c3cdb8e3fafd74cfb36e6bcfe0811e7152b2d0

---


# Trabajar con informes {#work-with-reports}

La capacidad de generación de informes es fundamental para evaluar [!DNL Brand Portal] el uso y saber cómo los usuarios internos y externos interactúan con los recursos aprobados. Los administradores pueden ver [!DNL Brand Portal] el informe de uso, que siempre está disponible en la página Informes de recursos. Sin embargo, los informes de inicios de sesión de usuario y recursos descargados, caducados, publicados y compartidos mediante vínculos pueden generarse y verse desde la página Informes de recursos. Estos informes son útiles para analizar la implementación de recursos, lo que le permite extraer métricas de éxito clave para medir la adopción de los recursos aprobados dentro y fuera de su organización.

La interfaz de administración de informes es intuitiva e incluye opciones y controles precisos para acceder a los informes guardados. Puede ver, descargar o eliminar informes de la página Informes de recursos, donde se enumeran todos los informes previamente generados.

## Ver informes {#view-reports}

Para ver un informe, siga estos pasos:

1. En la barra de herramientas de la parte superior, toque o haga clic en [!DNL AEM] el logotipo para acceder a las herramientas administrativas.

   ![](assets/aemlogo.png)

2. En el panel de herramientas administrativas, haga clic **en Crear/Administrar informes** para abrir** Informes de recursos** página.

   ![](assets/access-asset-reports.png)

3. Informe **de uso** de acceso y otros informes generados desde la página Informes de recursos.

   >[!NOTE]
   >
   >El informe de uso está presente de forma predeterminada en [!DNL Brand Portal]. No se puede crear ni eliminar. Sin embargo, puede crear, descargar y eliminar los informes Descargar, Caducidad, Publicar, Compartir vínculos e Inicios de sesión de usuario.

   Para ver un informe, toque o haga clic en el vínculo del informe. También puede seleccionar el informe y tocar/hacer clic en el icono Ver de la barra de herramientas.

   **El informe de uso** muestra información sobre el número de [!DNL Brand Portal] usuarios actuales, el espacio de almacenamiento ocupada por todos los recursos y el recuento total de recursos en [!DNL Brand Portal]. El informe también muestra la capacidad permitida para cada una de estas métricas de información.

   ![](assets/usage-report.png)

   **Informe Inicios** de sesión de usuario proporciona información sobre los usuarios que [!DNL Brand Portal]iniciaron sesión. El informe muestra nombres de pantalla, ID de correo electrónico, personas (administrador, visor, editor, invitado), grupos, último inicio de sesión, estado de actividad e inicio de sesión de cada usuario desde [!DNL Brand Portal] la implementación 6.4.2 hasta el momento de generación de informes.

   ![](assets/user-logins.png)

   **Descargue** listas de informes y detalles sobre todos los recursos descargados en una fecha y un intervalo de tiempo específicos.

   ![](assets/download-report.png)

   >[!NOTE]
   >
   >Los recursos** Descargar** muestran solamente los recursos que se seleccionaron y descargaron de forma individual [!DNL Brand Portal]. Si un usuario ha descargado una carpeta que contiene recursos, el informe no mostrará la carpeta ni los recursos dentro de ella.

   **El informe de caducidad** enumera y detalla todos los recursos que caducaron en un intervalo de tiempo específico.

   ![](assets/expiration-report.png)

   **Publicar** listas de informes y proporciona información sobre todos los recursos publicados en [!DNL AEM][!DNL Brand Portal] un intervalo de tiempo especificado.

   ![](assets/publish-report.png)

   >[!NOTE]
   >
   >Publicar informe no muestra información sobre los fragmentos de contenido, ya que los fragmentos de contenido no se pueden publicar en [!DNL Brand Portal].

   **El informe Compartir vínculos** enumera todos los recursos compartidos mediante vínculos desde [!DNL Brand Portal] la interfaz en un intervalo de tiempo específico. El informe también informa cuando se ha compartido el recurso mediante un vínculo, por qué usuario, cuándo caduca el vínculo y el número de vínculos compartidos para el inquilino (y los usuarios con los que se ha compartido el vínculo del recurso). Las columnas del informe Compartir vínculos no se pueden personalizar.

   ![](assets/link-share-report.png)

   >[!NOTE]
   >
   >El informe Compartir vínculos no muestra los usuarios que tienen acceso al recurso compartido mediante el vínculo o que han descargado el recurso a través del vínculo.
   >
   >
   >Para rastrear las descargas a través del vínculo compartido, debe generar informes descargados después de seleccionar **Solo descargas** de vínculos compartidos en **la** página Crear informe. Sin embargo, el usuario (descargado por) es anónimo en este caso.

## Generar informes {#generate-reports}

Los administradores pueden generar y administrar los siguientes informes estándar, una vez generados, se guardan para [obtener acceso](../using/brand-portal-reports.md#main-pars-header) posteriormente:

* Inicios de sesión de usuario
* Descargar
* Vencimiento
* Publicación
* Vínculos compartidos

Las columnas del informe de descarga, caducidad y publicación pueden personalizarse para su visualización. Para generar un informe, siga estos pasos:

1. Desde la barra de herramientas en la parte superior, toque o haga clic en [!DNL AEM] el logotipo para acceder a las herramientas administrativas.

   ![](assets/aemlogo.png)

2. En el panel de herramientas administrativas, toque o haga clic **en Crear/Administrar informes** para abrir** Informes de recursos** página.

   ![](assets/asset-reports.png)

3. En la página Informes de recursos, toque o haga clic **en Crear**.
4. En la página **Crear informe** , seleccione un informe para crear y toque o haga clic **en Siguiente**.

   ![](assets/crete-report.png)

5. Configure los detalles del informe. Especifique el título, la descripción, la estructura de carpetas (donde el informe debe ejecutar y generar estadísticas) y el intervalo de fechas para **los informes de descarga**, **caducidad** y **publicación** .

   ![](assets/create-report-page.png)

   En cambio, **Compartir informe** solo necesita los parámetros título, descripción y intervalo de fechas.

   ![](assets/create-link-share-report.png)

   >[!NOTE]
   >
   >Los caracteres especiales # y % en el título del informe se reemplazan por un guión (-) en la generación de informes.

6. Toque o haga clic **en Siguiente**, para configurar las columnas de los informes de descarga, caducidad y publicación.
7. Seleccione o anule la selección de las casillas adecuadas según sea necesario. Por ejemplo, para ver los nombres de los usuarios (que descargaron recursos) en **Descargar** informe, seleccione **Descargado por**. La siguiente imagen ilustra la selección de columnas predeterminadas en Descargar informe.

   ![](assets/createdownloadreport.png)

   También puede agregar columnas personalizadas a estos informes para ver más datos para los requisitos personalizados.

   Para agregar columnas personalizadas a los informes de descarga, publicación o caducidad, siga estos pasos:

   1. Para mostrar una columna personalizada, toque o haga clic **en Agregar** dentro **de columnas personalizadas**.
   2. Especifique el nombre de la columna en **el campo Nombre** de columna.
   3. Seleccione la propiedad a la que debe asignarse la columna, utilizando el selector de propiedades.

      ![](assets/property-picker.png)Como alternativa, escriba la ruta en el campo de ruta de propiedad.

      ![](assets/property-path.png)

      Para agregar más columnas personalizadas, toque y haga clic **en Agregar** y repita los pasos 2 y 3.

8. Toque o haga clic en **Crear**. Un mensaje notifica que se ha iniciado la generación de informes.

## Descargar informes {#download-reports}

Para guardar y descargar un informe como archivo. csv, realice una de las siguientes acciones:

* Seleccione un informe en la página Informes de recursos y toque o haga clic **en Descargar** de la barra de herramientas en la parte superior.

![](assets/download-asset-report.png)

* Desde la página Informes de recursos, abra un informe. Seleccione **la** opción Descargar desde la parte superior de la página del informe.

![](assets/download-report-fromwithin.png)

## Eliminar informes {#delete-reports}

Para eliminar un informe existente, seleccione el informe desde **la página Informes** de recursos y toque o haga clic **en Eliminar** de la barra de herramientas en la parte superior.

>[!NOTE]
>
>**El informe de uso** no se puede eliminar.