---
title: Administrar configuraciones generales del usuario
seo-title: Administrar configuraciones generales del usuario
description: Configurar aceleración de descarga, inteligente pública [! Creación de UICONTROL], public [! Creación de UICONTROL] y permitir que los usuarios administradores eliminen recursos de inquilinos.
seo-description: Configurar aceleración de descarga, inteligente pública [! Creación de UICONTROL], public [! Creación de UICONTROL] y permitir que los usuarios administradores eliminen recursos de inquilinos.
uuid: 3 c 46 cd 7 c-c 38 b -4 bc 7-b 566-93 f 977 bc 8227
contentOwner: mgulati
topic-tags: administración
content-type: referencia
products: SG_ EXPERIENCEMANAGER/Brand_ Portal
discoiquuid: f 4 c 237 bc-f 6 a 4-4 bc 4-af 56-3 d 9 c 3027 daf 4
translation-type: tm+mt
source-git-commit: ea7fdd2df0696ed309227fa77e3f79d0141bcb58

---


# Administrar configuraciones generales del usuario {#administer-general-tenant-configurations}

[!DNL AEM] Los recursos [!DNL Brand Portal] permiten a las organizaciones configurar las siguientes capacidades para inquilinos específicos:

* Eliminación de recursos por administradores
* Creación de [!UICONTROL colecciones] públicas por usuarios no administradores
* Creación de [!UICONTROL colecciones] inteligentes públicas por usuarios no administradores
* Aceleración de descarga
* Jerarquía principal de carpetas compartidas visibles para usuarios no administradores

Estas configuraciones se han proporcionado como **configuraciones de Configuración** general en el panel de herramientas administrativas.

![](assets/general-configs.png)

**** Una configuración para permitir a los administradores eliminar recursos. [!DNL Brand Portal] (El valor predeterminado es habilitado)

**Configuración B** para permitir que los usuarios no administradores creen [!UICONTROL colecciones públicas]. (El valor predeterminado es habilitado)

**Configuración C** para permitir que los usuarios no administradores creen colecciones inteligentes [!UICONTROL públicas]. (El valor predeterminado es habilitado)

**Configuración D** para permitir la aceleración de descarga de recursos descargados del portal y de los vínculos compartidos. (El valor predeterminado está deshabilitado)

**Configuración E** para mostrar la jerarquía de carpetas (desde la raíz) de carpetas compartidas a usuarios no administradores (editores, usuarios invitados, usuarios invitados). (El valor predeterminado está deshabilitado)

## Habilitar/deshabilitar configuraciones generales {#enable-disable-general-configurations}

Para habilitar o deshabilitar cada una de estas configuraciones:

1. Inicie sesión con privilegios de administrador.
2. Seleccione [!DNL AEM] el logotipo para acceder a las herramientas administrativas, desde la barra de herramientas situada en la parte superior.
3. En el panel de herramientas administrativas, seleccione **General** para abrir la página **Configuración** general.
4. Use el conmutador correspondiente para habilitar/deshabilitar cualquiera de las configuraciones Generales.
5. **Guarde los cambios.**
6. Cierre la sesión para que los cambios surtan efecto.

## Permitir a los usuarios administradores eliminar recursos de [!DNL Brand Portal]{#allow-admin-users-to-delete-assets-from-brand-portal}

**Permitir que los usuarios eliminen** la configuración permite a las organizaciones permitir (o restringir) que los usuarios con privilegios de administrador puedan eliminar recursos y carpetas.[!DNL Brand Portal]

## Permitir la creación de colecciones públicas por usuarios que no son administradores {#allow-public-collections-creation-by-non-admins}

[Permitir la creación [!UICONTROL de colecciones]públicas] (./using/brand-portal-share-[!UICONTROL collection]. md # main-pars-text -1915052376) controla si los usuarios no administradores pueden crear [!UICONTROL colecciones públicas]activadas [!DNL Brand Portal]. La configuración está habilitada de forma predeterminada. Al deshabilitar las organizaciones de configuración, pueden evitarse tener varias [!UICONTROL colecciones públicas]en su portal para poder guardar el espacio del sistema.

## Permitir la creación de colecciones inteligentes públicas por usuarios que no son administradores {#allow-public-smart-collections-creation-by-non-admins}

[Permitir la configuración de creación](../using/brand-portal-searching.md#main-pars-header-500620467) de colecciones inteligentes públicas controla si los usuarios no administradores pueden guardar sus búsquedas como [!UICONTROL colecciones inteligentes] y hacerlas públicas para dicho inquilino. La configuración está habilitada de forma predeterminada. Al deshabilitar las organizaciones de configuración, puede evitar tener un gran número de colecciones inteligentes [!UICONTROL públicas] creadas por usuarios no administradores en [!DNL Brand Portal]la organización.

## Permitir aceleración de descarga {#allow-download-acceleration}

[Permitir la configuración de aceleración](../using/accelerated-download.md) de descarga permite a las organizaciones permitir descargas aceleradas de recursos y [!DNL Brand Portal] vínculos compartidos mediante la integración con IBM Aspera Connect que es una aplicación a petición. La aplicación utiliza tecnología patentada para eliminar las sobrecargas TCP.

## Habilitar la jerarquía de carpetas {#enable-folder-hierarchy}

[Habilitar la configuración de jerarquía](../using/brand-portal-sharing-folders.md#non-admin-user-access-to-shared-folders) de carpetas permite a los administradores controlar cómo los usuarios no administradores (editores, usuarios invitados y usuarios invitados) ven las carpetas compartidas tras iniciar sesión.
