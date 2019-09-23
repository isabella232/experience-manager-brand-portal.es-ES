---
title: Utilizar el formulario de esquema de metadatos
seo-title: Utilizar el formulario de esquema de metadatos
description: Un esquema de metadatos describe la presentación de la página Propiedades y las propiedades de metadatos que se muestran para los recursos que utilizan el esquema en particular. El esquema que se aplica a un recurso determina los campos de metadatos que aparecen en la página Propiedades.
seo-description: Un esquema de metadatos describe la presentación de la página Propiedades y las propiedades de metadatos que se muestran para los recursos que utilizan el esquema en particular. El esquema que se aplica a un recurso determina los campos de metadatos que aparecen en la página Propiedades.
uuid: 1a944a3b-5152-425f-b1ea-bfe3331de928
content-type: referencia
products: SG_EXPERIENCEMANAGER/Brand_Portal
topic-tags: administración
discoiquuid: 500b46da-ef67-46a0-a069-192f4b1a0eca
translation-type: tm+mt
source-git-commit: 068ce845c51de48fb677f7bd09a2f6d20ff6f1a5

---


# Utilizar el formulario de esquema de metadatos {#use-the-metadata-schema-form}

Un esquema de metadatos describe la presentación de la página Propiedades y las propiedades de metadatos que se muestran para los recursos que utilizan el esquema en particular. El esquema que se aplica a un recurso determina los campos de metadatos que aparecen en la página Propiedades.

La página **[!UICONTROL Propiedades]** de cada recurso incluye propiedades de metadatos predeterminadas según el tipo MIME del recurso. Los administradores pueden utilizar el Editor de esquemas de metadatos para modificar esquemas existentes o agregar esquemas de metadatos personalizados. AEM Assets Brand Portal proporciona formularios predeterminados para recursos de varios tipos MIME. Sin embargo, también puede agregar formularios personalizados para estos recursos.

## Adición de un formulario de esquema de metadatos {#add-a-metadata-schema-form}

Para crear un nuevo formulario de esquema de metadatos, haga lo siguiente:

1. En la barra de herramientas de AEM de la parte superior, haga clic en el logotipo de Adobe para acceder a las herramientas administrativas.

   ![](assets/aemlogo.png)

2. En el panel Herramientas administrativas, haga clic en Esquemas **[!UICONTROL de metadatos]**.

   ![](assets/navigation-panel.png)

3. En la página Formularios **[!UICONTROL de esquema de]** metadatos, haga clic en **[!UICONTROL Crear]**.

   ![](assets/create-metadata-schema-form.png)

4. En el cuadro de diálogo **[!UICONTROL Crear formulario]** de esquema, especifique el título del formulario de esquema y, a continuación, haga clic en **[!UICONTROL Crear]** para completar el proceso de creación del formulario.

   ![](assets/create-schema-form.png)

## Edit a metadata schema form {#edit-a-metadata-schema-form}

Puede editar un formulario de esquema de metadatos recién agregado o existente. El formulario de esquema de metadatos contiene contenido derivado de su elemento principal, incluidas fichas y elementos de formulario dentro de fichas. Puede asignar o configurar estos elementos de formulario a un campo dentro de un nodo de metadatos.

Puede agregar nuevas fichas o elementos de formulario al formulario de esquema de metadatos. Las fichas derivadas y los elementos de formulario (del elemento principal) están en estado bloqueado. No se pueden alterar a nivel secundario.

Para editar un formulario de esquema de metadatos, haga lo siguiente:

1. En la barra de herramientas de AEM de la parte superior, haga clic en el logotipo de Adobe para acceder a las herramientas administrativas.

   ![](assets/aemlogo.png)

2. En el panel Herramientas administrativas, haga clic en Esquemas **[!UICONTROL de metadatos]**.
3. En la página Formularios **[!UICONTROL de esquema de]** metadatos, seleccione un formulario de esquema para editar sus propiedades, por ejemplo, **[!UICONTROL colección]**.

   ![](assets/metadata-schema-forms.png)

   >[!NOTE]
   >
   >Las plantillas sin editar muestran un símbolo de bloqueo antes de ellas. Si personaliza cualquiera de las plantillas, desaparece el símbolo de bloqueo antes de la plantilla.

4. En la barra de herramientas de la parte superior, haga clic en **[!UICONTROL Editar]**.

   Se abre la página Editor **[!UICONTROL de esquemas de]** metadatos con la ficha **[!UICONTROL Básico]** abierta a la izquierda y la ficha **[!UICONTROL Generar formulario]** abierta a la derecha.

5. En la página Editor **[!UICONTROL de esquemas de]** metadatos, personalice la página **[!UICONTROL Propiedades]** del recurso arrastrando uno o varios componentes de una lista de tipos de componentes de la ficha **[!UICONTROL Generar formulario]** a la ficha **[!UICONTROL Básico]** .

   ![](assets/metadata-schemaeditor-page.png)

6. Para configurar un componente, selecciónelo y modifique sus propiedades en la ficha **[!UICONTROL Configuración]** .

### Componentes de la ficha Formulario de compilación {#components-in-the-build-form-tab}

La ficha **[!UICONTROL Generar formulario]** enumera los elementos que puede utilizar en el formulario de esquema. La ficha **[!UICONTROL Configuración]** proporciona los atributos de cada elemento seleccionado en la ficha **[!UICONTROL Generar formulario]** . En la tabla siguiente se muestran los elementos de formulario disponibles en la ficha **[!UICONTROL Generar formulario]** :

| Nombre del componente | Descripción |
|---------------------|--------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------|
| [!UICONTROL Sección de encabezado] | Agregue un encabezado de sección para ver una lista de componentes comunes. |
| [!UICONTROL Texto de una sola línea] | Agregue una propiedad de texto de una sola línea. Se almacena como una cadena. |
| [!UICONTROL Multi ValueText] | Agregue una propiedad de texto con varios valores. Se almacena como una matriz de cadenas. |
| [!UICONTROL Número] | Agregue un componente numérico. |
| [!UICONTROL Fecha] | Agregue un componente de fecha. |
| [!UICONTROL Lista desplegable] | Agregue una lista desplegable. |
| [!UICONTROL Etiquetas estándar] | Añadir una etiqueta. **** Nota: Es posible que los administradores necesiten cambiar el valor de la ruta, por ejemplo, `/etc/tags/mac/<tenant_id>/<custom_tag_namespace>`si publican el formulario de esquema de metadatos desde AEM, donde la ruta no incluye la información del inquilino, por ejemplo, `/etc/tags/<custom_tag_namespace>`. |
| [!UICONTROL Etiquetas inteligentes] | Etiquetas detectadas automáticamente si ha adquirido y configurado el complemento de etiquetas inteligentes de AEM. |
| [!UICONTROL Campo oculto] | Agregue un campo oculto. Se envía como parámetro POST cuando se guarda el recurso. |
| [!UICONTROL Recurso al que se hace referencia en] | Agregue este componente para ver la lista de recursos a los que hace referencia el recurso. |
| [!UICONTROL Referencia de recursos] | Agregar para mostrar una lista de recursos que hacen referencia al recurso. |
| [!UICONTROL Clasificación del recurso] | Puntuación promedio de un recurso agregado desde Recursos AEM antes de publicarse en Brand Portal. |
| [!UICONTROL Metadatos de contexto] | Agregar para controlar la visualización de otras fichas de metadatos en la página Propiedades de los recursos. |

>[!NOTE]
>
>No utilice Referencias **** del producto, ya que no es funcional.

#### Edición del componente de metadatos {#edit-the-metadata-component}

Para editar las propiedades de un componente de metadatos en el formulario, haga clic en el componente y edite sus propiedades en la ficha **[!UICONTROL Configuración]** .

* **[!UICONTROL Etiqueta]** de campo: Nombre de la propiedad de metadatos que se muestra en la página Propiedades del recurso.

* **[!UICONTROL Asignar a propiedad]**: El valor de esta propiedad proporciona la ruta/nombre relativos al nodo de recurso donde se guarda en el repositorio de CRX. Comienza con "**./**" porque indica que la ruta está debajo del nodo del recurso.

Los siguientes son los valores válidos para esta propiedad:

— [!UICONTROL `./jcr:content/metadata/dc:title`]: Almacena el valor en el nodo de metadatos del recurso como propiedad [!UICONTROL `dc:title`].

— [!UICONTROL `./jcr:created`]: Muestra la propiedad jcr en el nodo del recurso. Si configura estas propiedades en propiedades de vista, le recomendamos que las marque como Deshabilitar edición, ya que están protegidas. De lo contrario, se produce el error "Error al modificar los recursos" al guardar las propiedades del recurso.

* **[!UICONTROL Marcador de posición]**: Utilice esta propiedad para proporcionar al usuario toda la información relevante sobre la propiedad metadata.
* **[!UICONTROL Requerido]**: Utilice esta propiedad para marcar una propiedad de metadatos como obligatoria en la página Propiedades.
* **[!UICONTROL Deshabilitar Editar]**: Utilice esta propiedad para que una propiedad de metadatos no se pueda editar en la página Propiedades.
* **[!UICONTROL Mostrar campo vacío en solo]** lectura: Marque esta propiedad para mostrar una propiedad de metadatos en la página Propiedades aunque no tenga ningún valor. De forma predeterminada, cuando una propiedad de metadatos no tiene ningún valor, no se muestra en la página Propiedades.
* **[!UICONTROL Descripción]**: Utilice esta propiedad para agregar una breve descripción para el componente de metadatos.
* **[!UICONTROL Icono]** Eliminar: Haga clic en este icono para eliminar un componente del formulario de esquema.

![](assets/delete_icon_editmetadataschemaform.png)

>[!NOTE]
>
>Todos los campos de metadatos son de solo lectura en el formulario de editor de metadatos de un recurso. Puesto que los metadatos del recurso deben editarse en Recursos AEM antes de publicar un recurso en Brand Portal.

#### Agregar o eliminar una ficha del formulario de esquema {#add-or-delete-a-tab-in-the-schema-form}

El formulario de esquema predeterminado incluye las fichas **[!UICONTROL Básico]** y **[!UICONTROL Avanzado]** . El editor de esquemas permite agregar o eliminar una ficha.

![](assets/add_delete_tabs_metadataschemaform.png)

* Para agregar una nueva ficha a un formulario de esquema, haga clic en **[!UICONTROL +]**. De forma predeterminada, la nueva ficha tiene el nombre "Sin nombre-1". Puede modificar el nombre desde la ficha **[!UICONTROL Configuración]** .

![](assets/add-tab-metadata-form.png)

* Para eliminar una ficha, haga clic en **[!UICONTROL x]**. Click **[!UICONTROL Save]** to save the changes.

## Aplicación de un esquema de metadatos a una carpeta {#apply-a-metadata-schema-to-a-folder}

Brand Portal le permite personalizar y controlar el esquema de metadatos para que la página [!UICONTROL Propiedades] de un recurso muestre únicamente la información específica que elija revelar. Para controlar los metadatos mostrados en la página [!UICONTROL Propiedades] , elimine los metadatos necesarios del formulario de esquema de metadatos y aplíquelo a la carpeta específica.

Para aplicar un formulario de esquema de metadatos a una carpeta, haga lo siguiente:

1. En la barra de herramientas de AEM de la parte superior, haga clic en el logotipo de Adobe para acceder a las herramientas administrativas.

   ![](assets/aemlogo.png)

2. En el panel Herramientas administrativas, haga clic en Esquemas **[!UICONTROL de metadatos]**.

3. En la página Formularios **[!UICONTROL de esquema de]** metadatos, seleccione el formulario de esquema que desea aplicar a un recurso, por ejemplo, [!UICONTROL ropa].

   ![](assets/apply-metadata-schema-form-to-folder.png)

4. En la barra de herramientas de la parte superior, haga clic en **[!UICONTROL Aplicar a carpetas]**.

5. En la página **[!UICONTROL Seleccionar carpetas]** , navegue a la carpeta en la que desea aplicar el esquema de metadatos de **[!UICONTROL ropa]** , por ejemplo, **[!UICONTROL Guantes]**.

   ![](assets/apply_metadata_schemaformtofoldergloves.png)

6. Haga clic en **[!UICONTROL Aplicar]** para aplicar el formulario de esquema de metadatos a la carpeta.

   Los metadatos disponibles en el formulario de esquema de metadatos de **[!UICONTROL ropa]** se aplican a la carpeta **[!UICONTROL Guantes]** y están visibles en la página **[!UICONTROL Propiedades]** de la carpeta.

   ![](assets/folder_metadata_properties.png)

>[!NOTE]
>
>Si aplica un esquema que incluye esquemas anidados a una carpeta que contiene archivos de vídeo, es posible que las propiedades de metadatos de los archivos de vídeo no se representen correctamente. Para asegurarse de que las propiedades de metadatos se representan correctamente, elimine los esquemas anidados y aplique solo el esquema principal a la carpeta.

## Delete a metadata schema form {#delete-a-metadata-schema-form}

Brand Portal permite eliminar únicamente formularios de esquema personalizados. No permite eliminar los formularios o plantillas de esquema predeterminados. Sin embargo, puede eliminar cualquier cambio personalizado en estos formularios.

Para eliminar un formulario, selecciónelo y haga clic en el icono **[!UICONTROL Eliminar]** .

![](assets/delete_icon_metadataschemaeditorform.png)

>[!NOTE]
>
>Después de eliminar los cambios personalizados realizados en un formulario predeterminado, el símbolo **[!UICONTROL Bloquear]** vuelve a aparecer antes del nombre del formulario en la interfaz del esquema de metadatos para indicar que el formulario se ha revertido a su estado predeterminado.

## Formularios de esquema para tipos MIME {#schema-forms-for-mime-types}

### Adición de nuevos formularios para tipos MIME {#adding-new-forms-for-mime-types}

Además de los formularios predeterminados, puede agregar formularios personalizados para recursos de varios tipos MIME o crear un nuevo formulario con un tipo de formulario adecuado. Por ejemplo, para agregar una nueva plantilla para el subtipo **[!UICONTROL imagen/png]** , cree el formulario en los formularios de "imagen". El título del formulario de esquema es el nombre del subtipo. En este caso, el título es "png".

#### Uso de una plantilla de esquema existente para varios tipos MIME {#using-an-existing-schema-template-for-various-mime-types}

Puede utilizar una plantilla existente para otro tipo MIME. Por ejemplo, utilice el formulario **image/jpeg** para recursos de tipo MIME **image/png**.

En este caso, cree un nuevo nodo en [!UICONTROL `/etc/dam/metadataeditor/mimetypemappings`] el repositorio de CRX. Especifique un nombre para el nodo y defina las siguientes propiedades:

| **Nombre** | **Tipo** | **Value** |
|---|---|---|
| exponsedmimetype | Cadena | image/jpeg |
| mimetypes | Cadena[] | image/png |

* **exponsedmimetype**: Nombre del formulario existente que se va a asignar
* **mimetypes**: Lista de tipos MIME que utilizan el formulario definido en el atributo **exponsedmimetype**

Brand Portal asigna los siguientes tipos MIME y formularios de esquema:

| **Formulario de esquema** | **Tipos MIME** |
|---|---|
| image/jpeg | image/pjpeg |
| image/tiff | image/x-tiff |
| application/pdf | application/postscript |
| application/x-ImageSet | Multipart/Related; type=application/x-ImageSet |
| application/x-SpinSet | Multipart/Related; type=application/x-SpinSet |
| application/x-MixedMediaSet | Multipart/Related; type=application/x-MixedMediaSet |
| video/quicktime | video/x-quicktime |
| video/mpeg4 | video/mp4 |
| video/avi | video/avi, video/msvideo, video/x-msvideo |
| video/wmv | video/x-ms-wmv |
| video/flv | video/x-flv |

A continuación se muestra una lista de propiedades de metadatos predeterminadas:

* jcr:content/metadata/cq:tags
* jcr:content/metadata/dc:format
* jcr:content/metadata/dam:status
* jcr:content/metadata/videoCodec
* jcr:content/metadata/audioCodec
* jcr:content/metadata/dc:title
* jcr:content/metadata/dc:description
* jcr:content/metadata/xmpMM:InstanceID
* jcr:content/metadata/xmpMM:DocumentID
* jcr:content/metadata/dam:sha1
* jcr:content/metadata/dam:solutionContext
* jcr:content/metadata/videoBitrate
* jcr:content/metadata/audioBitrate
* jcr:content/usages/usedBy
* jcr:content/jcr:lastModified
* jcr:content/metadata/prism:expirationDate
* jcr:content/onTime
* jcr:content/offTime
* jcr:content/metadata/dam:size
* jcr:content/metadata/tiff:ImageWidth
* jcr:content/metadata/tiff:ImageLength
