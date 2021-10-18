---
title: 'Configuración y publicación de la carpeta de contribución de Experience Manager Assets a Brand Portal '
seo-title: Configure and publish contribution folder from Experience Manager Assets to Brand Portal
description: Obtenga información sobre cómo configurar y publicar una carpeta de contribución de Experience Manager Assets a Brand Portal.
seo-description: Get an insight into configuring and publishing a contribution folder from Experience Manager Assets to Brand Portal.
uuid: null
content-type: reference
contentOwner: Vishabh Gupta
topic-tags: brand-portal
products: SG_EXPERIENCEMANAGER/Brand_Portal
discoiquuid: null
exl-id: 9acad588-977a-45de-b544-f2cc8874ba12
source-git-commit: 533b2a637700770ff08c88da92892af863265902
workflow-type: tm+mt
source-wordcount: '1217'
ht-degree: 0%

---

# Configurar la carpeta de contribución en Experience Manager Assets {#configure-contribution-folder}

Para la colaboración de fuentes de recursos, los usuarios de Experience Manager Assets (administradores y usuarios no administradores con permiso) pueden crear nuevas carpetas de tipo **Contribución de recursos**, lo que garantiza que la nueva carpeta creada esté abierta al envío de recursos por parte de los usuarios de Brand Portal.  Esto déclencheur automáticamente un flujo de trabajo que crea dos subcarpetas adicionales, llamadas **SHARED** y **NEW**, dentro de la carpeta **Contribution** recién creada.

A continuación, el usuario de Experience Manager Assets define los requisitos de los recursos cargando un resumen sobre los tipos de recursos que deben agregarse a la carpeta de contribución, así como un conjunto de recursos de línea base, a la carpeta **SHARED** para garantizar que los usuarios de Brand Portal tengan la información que necesitan. A continuación, el administrador puede conceder a los usuarios activos de Brand Portal acceso a la carpeta de contribución antes de publicar la carpeta de contribución recién creada en Brand Portal.

En el siguiente vídeo se muestra cómo configurar una carpeta de contribución en Experience Manager Assets:

>[!VIDEO](https://video.tv.adobe.com/v/30547)

El usuario de Experience Manager Assets realiza las siguientes actividades al configurar una carpeta de contribución:

* [Crear carpeta de contribución](#create-contribution-folder)
* [Cargar requisitos de recursos y asignar colaboradores](#configure-contribution-folder-properties)
* [Cargar recursos de línea de base](#uplad-new-assets-to-contribution-folder)
* [Publicar carpeta de contribución de Experience Manager Assets en Brand Portal](#publish-contribution-folder-to-brand-portal)

## Crear carpeta de contribución {#create-contribution-folder}


Los administradores de Experience Manager Assets y los usuarios no administradores que tengan permiso para crear una carpeta nueva pueden crear una carpeta de contribución en Experience Manager Assets.
Para crear una carpeta de contribución, cree una nueva carpeta de tipo Contribución de recursos y asegúrese de que la nueva carpeta creada esté abierta al envío de recursos por parte de los usuarios de Brand Portal.  Esto déclencheur automáticamente un flujo de trabajo que crea dos subcarpetas adicionales, denominadas SHARED y NEW, dentro de la carpeta de contribución.


>[!NOTE]
>
>Los administradores pueden crear varias carpetas de contribución de recursos dentro de una carpeta.
>
>Una carpeta de contribución de recursos contiene carpetas NUEVAS y COMPARTIDAS para la distribución y contribución de los recursos. No cree ninguna carpeta de recursos, carpetas o contribuciones dentro de una carpeta de contribución.


Puede configurar las propiedades de la carpeta de contribución por separado, así como al crear la carpeta de contribución. En este ejemplo, configuramos las propiedades por separado.

**Para crear una carpeta de contribución:**

1. Inicie sesión en la instancia de Experience Manager Assets.

1. Vaya a **[!UICONTROL Assets]** > **[!UICONTROL Files]**. Enumera todas las carpetas existentes en el repositorio de Experience Manager Assets.

1. Haga clic en **[!UICONTROL Create]** para crear una carpeta nueva. **[!UICONTROL Se abre el cuadro de]** diálogo Crear carpeta .

1. Introduzca **[!UICONTROL Title]** y **[!UICONTROL Name]** de la carpeta y seleccione la casilla de verificación **[!UICONTROL Asset Contribution]**.
Se recomienda utilizar letras minúsculas sin ningún espacio para asignar un nombre a la carpeta.

1. Haga clic en **[!UICONTROL Crear]**. Puede ver la carpeta de contribución en el repositorio de Experience Manager Assets.

   >[!NOTE]
   >
   >Un usuario no administrador puede crear y compartir una carpeta de contribución de recursos, pero no puede modificarla ni eliminarla.


   ![](assets/create-contribution-folder.png)

1. Haga clic en para abrir la carpeta de contribución. Verá dos subcarpetas:**[!UICONTROL SHARED]** y **[!UICONTROL NEW]** se crean automáticamente dentro de la carpeta de contribución.

   ![](assets/contribution-folder.png)


## Configuración de las propiedades de la carpeta de contribución {#configure-contribution-folder-properties}

El administrador de Experience Manager Assets realiza las siguientes actividades al configurar las propiedades de una carpeta de contribución.

* **Agregar descripción**: Proporcione una descripción de alto nivel de la carpeta de contribución.
* **Cargar información**: Cargar el documento de requisitos de recursos que contiene información relacionada con los recursos.
* **Agregar colaboradores**: Agregue usuarios de Brand Portal para otorgarles acceso a la carpeta de contribución.

El requisito de recursos se refiere a los detalles proporcionados por los administradores para ayudar a los colaboradores (usuarios de Brand Portal) a comprender la necesidad y los requisitos de la carpeta de contribución. El administrador carga un documento de requisitos de recursos que contiene información breve sobre el tipo de recursos que se deben agregar a la carpeta de contribución y la información relacionada con los recursos, por ejemplo, el propósito, el tipo de imágenes, el tamaño máximo, etc.

**Para configurar las propiedades de la carpeta de contribución:**

1. Inicie sesión en la instancia de Experience Manager Assets.

1. Vaya a **[!UICONTROL Assets > Files]** y busque la carpeta de contribución.
1. Seleccione la carpeta de contribución y haga clic en **[!UICONTROL Properties]** para abrir la ventana Propiedades de la carpeta.

   ![](assets/properties.png)

   ![](assets/contribution-folder-property1.png)

1. Vaya a la pestaña **[!UICONTROL Contribución de recursos]**.
1. Introduzca **[!UICONTROL Description]** de alto nivel de la carpeta de contribución.
1. Haga clic en **[!UICONTROL Cargar resumen]** para buscar desde el equipo local y cargar un **documento de requisitos de recursos**.

   ![](assets/upload.png)

1. En el campo **[!UICONTROL Agregar usuario]**, agregue usuarios de Brand Portal con los que desee compartir la carpeta de contribución. Estos usuarios pueden acceder y cargar contenido en la carpeta de contribución a través de la interfaz de Brand Portal.
1. Haga clic en **[!UICONTROL Guardar]**.

   ![](assets/contribution-folder-property3.png)

>[!NOTE]
>
>Los resultados de la búsqueda se basan en la lista de usuarios de Brand Portal configurada en Experience Manager Assets. Asegúrese de tener la lista de usuarios de Brand Portal actualizada.

Los administradores pueden descargar el archivo `user.csv` desde [!DNL Admin Console] y utilizarlo como plantilla base para agregar usuarios de Brand Portal. Vaya a [!UICONTROL Users] y haga clic en la opción [!UICONTROL Export users list to csv] para descargar el archivo `users.csv`. La siguiente lista de usuarios de ejemplo detalla los atributos necesarios para agregar los usuarios. El único atributo obligatorio para una entrada de usuario es `Email` y todos los demás atributos son opcionales.

[Obtener archivo](assets/users.csv)

## Cargar recursos a la carpeta de contribución {#uplad-new-assets-to-contribution-folder}

Los usuarios de Brand Portal pueden descargar los requisitos de recursos para comprender la necesidad de la contribución.
A continuación, pueden crear nuevos recursos para la contribución y cargarlos en la carpeta NEW dentro de la carpeta de contribución.

>[!NOTE]
>
>Los usuarios de Brand Portal solo pueden cargar recursos en la carpeta NEW .
>
>El límite máximo de carga para cualquier inquilino de Brand Portal es **10** GB que se aplica de forma acumulativa a todas las carpetas de contribución.


Después de publicar los recursos recién creados en Experience Manager Assets, los usuarios de Brand Portal pueden eliminarlos de la carpeta NEW . En cambio, el administrador de Brand Portal puede eliminar los recursos de las carpetas NUEVO y COMPARTIDO.

Una vez alcanzado el objetivo de crear la carpeta de contribución, el administrador de Brand Portal puede eliminar la carpeta de contribución para liberar el espacio de carga para otros usuarios.

>[!NOTE]
>
>Se recomienda liberar el espacio de carga después de publicar la carpeta de contribución en Experience Manager Assets, de modo que esté disponible para los demás usuarios de Brand Portal para que contribuyan.
>
>Si es necesario ampliar el límite de carga de su inquilino de Brand Portal más allá de **10** GB, póngase en contacto con el Servicio de atención al cliente para especificar el requisito.


**Para cargar nuevos recursos:**

1. Inicie sesión en la instancia de Brand Portal.
El panel de Brand Portal refleja todas las carpetas existentes permitidas al usuario de Brand Portal junto con la carpeta de contribución recientemente compartida.

1. Seleccione la carpeta de contribución y haga clic en para abrirla. La carpeta de contribución contiene dos subcarpetas: **[!UICONTROL SHARED]** y **[!UICONTROL NEW]**.

1. Haga clic en la carpeta **[!UICONTROL NEW]**.

   ![](assets/upload-new-assets1.png)

1. Haga clic en **[!UICONTROL Crear]** > **[!UICONTROL Archivos]** para cargar archivos o carpetas individuales (.zip) que contengan varios recursos.

   ![](assets/upload-new-assets2.png)

1. Examine y cargue los recursos (archivos o carpetas) en la carpeta **[!UICONTROL NEW]**.

   ![](assets/upload-new-assets3.png)

Después de cargar todos los recursos o carpetas en la carpeta NEW , publique la carpeta de contribución en Experience Manager Assets.


## Publicar carpeta de contribución en Brand Portal {#publish-contribution-folder-to-brand-portal}

Una vez configurada la carpeta de contribución, el usuario de Experience Manager Assets (administrador/usuario no administrador) puede publicar la carpeta de contribución de Experience Manager Assets en Brand Portal. Los usuarios de Brand Portal que tengan permiso para acceder a la carpeta de contribución recibirán una notificación por correo electrónico o por pulso una vez finalizada la acción de publicación.


**Para publicar la carpeta de contribución:**

1. Inicie sesión en la instancia de Experience Manager Assets.

1. Vaya a **[!UICONTROL Assets > Archivos]** y busque la carpeta de contribución en la que desea publicar en Brand Portal.
1. Seleccione la carpeta de contribución y haga clic en **[!UICONTROL Publicación rápida]** > **[!UICONTROL Publicar en Brand Portal]**.

   ![](assets/publish-contribution-folder-to-bp.png)

   Recibirá un mensaje de éxito una vez que la carpeta de contribución se publique en Brand Portal.

Se envía una notificación por correo electrónico o por impulso a los usuarios de Brand Portal asignados a la carpeta de contribución. Los usuarios de Brand Portal pueden acceder a la carpeta de contribución y comenzar la contribución. Consulte [Cargar recursos a la carpeta de contribución y publicar en Experience Manager Assets](brand-portal-publish-contribution-folder-to-aem-assets.md).
