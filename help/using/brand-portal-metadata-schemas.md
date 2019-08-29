---
title: Uso del formulario de esquema de metadatos
seo-title: Uso del formulario de esquema de metadatos
description: Un esquema de metadatos describe el diseño de la página Propiedades y las propiedades de metadatos mostradas para los recursos que usan el esquema concreto. El esquema que aplica a un recurso determina los campos de metadatos que aparecen en la página Propiedades.
seo-description: Un esquema de metadatos describe el diseño de la página Propiedades y las propiedades de metadatos mostradas para los recursos que usan el esquema concreto. El esquema que aplica a un recurso determina los campos de metadatos que aparecen en la página Propiedades.
uuid: 1 a 944 a 3 b -5152-425 f-b 1 ea-bfe 3331 de 928
content-type: referencia
products: SG_ EXPERIENCEMANAGER/Brand_ Portal
topic-tags: administración
discoiquuid: 500 b 46 da-ef 67-46 a 0-a 069-192 f 4 b 1 a 0 eca
translation-type: tm+mt
source-git-commit: 32c3cdb8e3fafd74cfb36e6bcfe0811e7152b2d0

---


# Uso del formulario de esquema de metadatos {#use-the-metadata-schema-form}

Un esquema de metadatos describe el diseño de la página Propiedades y las propiedades de metadatos mostradas para los recursos que usan el esquema concreto. El esquema que aplica a un recurso determina los campos de metadatos que aparecen en la página Propiedades.

La página **Propiedades** de cada recurso incluye propiedades de metadatos predeterminadas según el tipo MIME del recurso. Los administradores pueden utilizar el Editor de esquemas de metadatos para modificar esquemas existentes o agregar esquemas de metadatos personalizados. [!DNL AEM] Los recursos [!DNL Brand Portal] proporcionan formularios predeterminados para recursos de distintos tipos MIME. Sin embargo, también puede agregar formularios personalizados para dichos recursos.

## Adición de un formulario de esquema de metadatos {#add-a-metadata-schema-form}

Para crear un nuevo formulario de esquema de metadatos, haga lo siguiente:

1. En la [!DNL AEM] barra de herramientas de la parte superior, haga clic en el logotipo de Adobe para acceder a las herramientas administrativas.

   ![](assets/aemlogo.png)

2. En el panel de herramientas administrativas, haga clic en **Esquemas de metadatos**.

   ![](assets/navigation-panel.png)

3. En la página **Formularios** de esquemas de metadatos, haga clic **en Crear**.

   ![](assets/create-metadata-schema-form.png)

4. En el cuadro **de diálogo Crear formulario de** esquema, especifique el título del formulario Esquema y, a continuación, haga clic **en Crear** para completar el proceso de creación del formulario.

   ![](assets/create-schema-form.png)

## Edit a metadata schema form {#edit-a-metadata-schema-form}

Puede editar un formulario de esquema de metadatos recién agregado o existente. El formulario de esquema de metadatos contiene contenido derivado de su elemento principal, incluyendo fichas y elementos de formulario dentro de fichas. Puede asignar o configurar estos elementos de formulario a un campo dentro de un nodo de metadatos.

Puede agregar fichas o elementos de formulario nuevos al formulario de esquema de metadatos. Las fichas derivadas y los elementos de formulario (desde el elemento principal) se encuentran en el estado bloqueado. No puede alterarlos en el nivel secundario.

Para editar un formulario de esquema de metadatos, haga lo siguiente:

1. En la [!DNL AEM] barra de herramientas de la parte superior, haga clic en el logotipo de Adobe para acceder a las herramientas administrativas.

   ![](assets/aemlogo.png)

2. En el panel de herramientas administrativas, haga clic en **Esquemas de metadatos**.
3. En la página **Formularios** de esquemas de metadatos, seleccione un formulario de esquema para editar sus propiedades, **por ejemplo, colección**.

   ![](assets/metadata-schema-forms.png)

   >[!NOTE]
   >
   >Las plantillas no editadas muestran un **símbolo Bloquear** antes de ellas. Si personaliza cualquiera de las plantillas, **el** símbolo Bloquear antes de la plantilla desaparece.

4. En la barra de herramientas de la parte superior, haga clic **en Editar**.

   Se abre la **página Editor** de esquemas de metadatos con la ficha **Básico** abierta a la izquierda y la ficha **Build Form** (Generar formulario) a la derecha.

5. En **la página Editor** de esquemas de metadatos, personalice la **página Propiedades** del recurso arrastrando uno o varios componentes de una lista de tipos de componente en la ficha **Generar formulario** a **la** ficha Básico.

   ![](assets/metadata-schemaeditor-page.png)

6. Para configurar un componente, selecciónelo y modifique sus propiedades en la ficha **Configuración** .

### Componentes de la ficha Build Form (Generar formulario) {#components-in-the-build-form-tab}

La ficha **Build Form** (Generar formulario) enumera los elementos que puede utilizar en el formulario de esquema. La ficha **Configuración** proporciona los atributos de cada elemento seleccionado en la ficha **Build Form** (Generar formulario). La siguiente tabla enumera los elementos de formulario disponibles en la ficha **Build Form** (Generar formulario):

| Nombre del componente | Descripción |
|---------------------|--------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------|
| Sección de encabezado | Agregue un encabezado de sección para una lista de componentes comunes. |
| Texto de una sola línea | Agregue una propiedad de texto de una sola línea. Se almacena como una cadena. |
| Varios valuetext | Agregue una propiedad de texto multivalor. Se almacena como matriz de cadenas. |
| Número | Agregue un componente numérico. |
| Fecha | Agregue un componente de fecha. |
| Lista desplegable | Agregue una lista desplegable. |
| Etiquetas estándar | Añadir una etiqueta. **Nota:** Es posible que los administradores necesiten cambiar el valor de la ruta, por `/etc/tags/mac/<tenant_id>/<custom_tag_namespace>`ejemplo, si publican el formulario de esquema de metadatos desde [!DNL AEM], donde la ruta no incluye la información del inquilino, por ejemplo `/etc/tags/<custom_tag_namespace>`. |
| Etiquetas inteligentes | Etiquetas detectadas automáticamente si ha comprado y configurado el complemento de etiquetas [!DNL AEM] inteligentes. |
| Campo oculto | Agregue un campo oculto. Se envía como parámetro POST cuando se guarda el recurso. |
| Recurso al que se hace referencia en | Agregue este componente para ver la lista de recursos a los que hace referencia el recurso. |
| Referencia de recursos | Agregue para mostrar una lista de recursos que hacen referencia al recurso. |
| Clasificación del recurso | Clasificación media de un recurso agregado de [!DNL AEM] Assets antes de publicarse [!DNL Brand Portal]. |
| Metadatos de contexto | Agregue para controlar la visualización de otras fichas de metadatos en la página Propiedades de los recursos. |

>[!NOTE]
>
>No utilice **Referencias de producto** ya que no funciona.

#### Editar el componente de metadatos {#edit-the-metadata-component}

Para editar las propiedades de un componente de metadatos en el formulario, haga clic en el componente y edite sus propiedades en la ficha **Configuración** .

* **Etiqueta de campo**: Nombre de la propiedad de metadatos que se muestra en la página Propiedades del recurso.

* **Asignar a propiedad**: El valor de esta propiedad proporciona la ruta/nombre relativo al nodo de recurso donde se guarda en el repositorio de CRX. Comienza con "**./**"porque indica que la ruta se encuentra bajo el nodo del recurso.

Los valores válidos para esta propiedad son los siguientes:

— `./jcr:content/metadata/dc:title`: Almacena el valor en el nodo de metadatos del recurso como propiedad `dc:title`.

— `./jcr:created`: Muestra la propiedad jcr en el nodo del recurso. Si configura estas propiedades en propiedades de visualización, le recomendamos que las marque como Deshabilitar Editar, ya que están protegidas. De lo contrario, el error "Los recursos no se pueden modificar" se produce al guardar las propiedades del recurso.

* **Marcador de posición**: Utilice esta propiedad para proporcionar al usuario toda información relevante acerca de la propiedad de metadatos.
* **Obligatorio**: Utilice esta propiedad para marcar una propiedad de metadatos como obligatoria en la página Propiedades.
* **Deshabilitar editar**: Utilice esta propiedad para que una propiedad de metadatos no se pueda editar en la página Propiedades.
* **Mostrar campo vacío en solo lectura**: Marque esta propiedad para mostrar una propiedad de metadatos en la página Propiedades aunque no tenga ningún valor. De forma predeterminada, cuando una propiedad de metadatos no tiene valor, no se muestra en la página Propiedades.
* **Descripción**: Utilice esta propiedad para agregar una breve descripción del componente de metadatos.
* **Eliminar icono**: Haga clic en este icono para eliminar un componente del formulario de esquema.

![](assets/delete_icon_editmetadataschemaform.png)

>[!NOTE]
>
>Todos los campos de metadatos son de solo lectura en el editor de metadatos de un recurso. Puesto que los metadatos del recurso deben editarse en [!DNL AEM] Recursos antes [!DNL Brand Portal]de publicar un recurso.

#### Agregar o eliminar una ficha del formulario de esquema {#add-or-delete-a-tab-in-the-schema-form}

El formulario de esquema predeterminado incluye las fichas **Básico** y **Avanzado** . El editor de esquemas permite agregar o eliminar una ficha.

![](assets/add_delete_tabs_metadataschemaform.png)

* Para agregar una nueva ficha en un formulario de esquema, haga clic **en +**. De forma predeterminada, la nueva ficha tiene el nombre "Sin nombre -1". Puede modificar el nombre desde la ficha **Configuración** .

![](assets/add-tab-metadata-form.png)

* Para eliminar una ficha, haga clic **en x**. Click **Save** to save the changes.

## Aplicar un esquema de metadatos a una carpeta {#apply-a-metadata-schema-to-a-folder}

[!DNL Brand Portal] permite personalizar y controlar el esquema de metadatos para que la página **Propiedades** de un recurso muestre únicamente la información específica que elija revelar. Para controlar los metadatos mostrados en la página **Propiedades** , elimine los metadatos necesarios del formulario de esquema de metadatos y aplíquelo a la carpeta específica.

Para aplicar un formulario de esquema de metadatos a una carpeta, haga lo siguiente:

1. En la [!DNL AEM] barra de herramientas de la parte superior, haga clic en el logotipo de Adobe para acceder a las herramientas administrativas.

   ![](assets/aemlogo.png)

2. En el panel de herramientas administrativas, haga clic en **Esquemas de metadatos**.

3. En la página **Formularios** de esquemas de metadatos, seleccione el formulario de esquema que desea aplicar a un recurso, por ejemplo **, vestimenta**.

   ![](assets/apply-metadata-schema-form-to-folder.png)

4. En la barra de herramientas de la parte superior, haga clic **en Aplicar a carpetas**.

5. En la **página Seleccionar** carpetas, navegue a la carpeta a la que desee aplicar el **esquema** de metadatos de ropa, por ejemplo **, Gloves**.

   ![](assets/apply_metadata_schemaformtofoldergloves.png)

6. Haga clic **en Aplicar** para aplicar el formulario de esquema de metadatos a la carpeta.

   Los metadatos disponibles en el formulario de esquema de metadatos **de vestimenta** se aplican a la carpeta **Gloves** y se muestran en la página **Propiedades** de la carpeta.

   ![](assets/folder_metadata_properties.png)

>[!NOTE]
>
>Si aplica un esquema que incluye esquemas anidados a una carpeta que contiene archivos de vídeo, es posible que las propiedades de metadatos de los archivos de vídeo no se procesen correctamente. Para garantizar que las propiedades de metadatos se procesen correctamente, elimine los esquemas anidados y aplique solo el esquema principal a la carpeta.

## Delete a metadata schema form {#delete-a-metadata-schema-form}

[!DNL Brand Portal] solo permite eliminar formularios de esquema personalizados. No permite eliminar las plantillas o formularios de esquema predeterminados. Sin embargo, puede eliminar cualquier cambio personalizado en estos formularios.

Para eliminar un formulario, seleccione un formulario y haga clic en el icono **Eliminar** .

![](assets/delete_icon_metadataschemaeditorform.png)

>[!NOTE]
>
>Después de eliminar los cambios personalizados realizados en un formulario predeterminado, el símbolo **Bloquear** vuelve a aparecer antes del nombre del formulario en la interfaz del esquema de metadatos para indicar que el formulario vuelve a su estado predeterminado.

## Formularios de esquema para tipos MIME {#schema-forms-for-mime-types}

### Adición de nuevos formularios para tipos MIME {#adding-new-forms-for-mime-types}

Además de los formularios predeterminados, puede agregar formularios personalizados para recursos de varios tipos MIME o crear un nuevo formulario con un tipo de formulario adecuado. Por ejemplo, para agregar una nueva plantilla para el **subtipo de imagen/png** , cree el formulario debajo de los formularios "image". El título del formulario de esquema es el nombre del subtipo. En este caso, el título es "png".

#### Uso de una plantilla de esquema existente para varios tipos MIME {#using-an-existing-schema-template-for-various-mime-types}

Puede utilizar una plantilla existente para un tipo MIME diferente. Por ejemplo, utilice el formulario **image/jpeg** para recursos de image/png tipo **MIME**.

En este caso, cree un nuevo nodo en `/etc/dam/metadataeditor/mimetypemappings` el repositorio de CRX. Especifique un nombre para el nodo y defina las siguientes propiedades:

| **Nombre** | **Tipo** | **Value** |
|---|---|---|
| exasumidmimetype | Cadena | image/jpeg |
| mimetypes | Cadena[] | image/png |

* **exasumdmimetype**: Nombre del formulario existente que se asignará
* **mimetypes**: Lista de tipos MIME que utilizan el formulario definido en el **atributo exasumdmimetype** .

[!DNL Brand Portal] asigna los siguientes tipos MIME y formularios de esquema:

| **Formulario de esquema** | **Tipos MIME** |
|---|---|
| image/jpeg | image/pjpeg |
| image/tiff | image/x-tiff |
| application/pdf | application/postscript |
| application/x-imageset | Multipart/Related; type=application/x-ImageSet |
| application/x-spinset | Multipart/Related; type=application/x-SpinSet |
| application/x-mixedmediaset | Multipart/Related; type=application/x-MixedMediaSet |
| video/quicktime | video/x-quicktime |
| video/mpeg 4 | video/mp4 |
| video/avi | vídeo/avi, vídeo/msvideo, video/x-msvideo |
| video/wmv | video/x-ms-wmv |
| video/flv | video/x-flv |

A continuación se muestra una lista de propiedades de metadatos predeterminadas:

* jcr:content/metadata/cq:tags
* jcr:content/metadata/dc:format
* jcr:content/metadata/dam:status
* jcr: content/metadata/videocodec
* jcr: content/metadata/audiocodec
* jcr: content/metadata/dc: title
* jcr: content/metadata/dc: description
* jcr: content/metadata/xmpmm: Instanceid
* jcr: content/metadata/xmpmm: Documentid
* jcr: content/metadata/dam: sha 1
* jcr: content/metadata/dam: Solutioncontext
* jcr: content/metadata/videobitrate
* jcr: content/metadata/audiobitrate
* jcr: content/usages/usedby
* jcr:content/jcr:lastModified
* jcr:content/metadata/prism:expirationDate
* jcr: content/ontime
* jcr: content/offtime
* jcr:content/metadata/dam:size
* jcr: content/metadata/tiff: Imagewidth
* jcr: content/metadata/tiff: Imagelength