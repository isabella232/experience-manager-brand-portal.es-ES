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
source-git-commit: 068ce845c51de48fb677f7bd09a2f6d20ff6f1a5

---


# Administrar configuraciones generales del usuario {#administer-general-tenant-configurations}

AEM Assets Brand Portal permite a las organizaciones configurar las siguientes capacidades para inquilinos específicos:

* Eliminación de recursos por administradores
* Creación de colecciones públicas por usuarios no administradores
* Creación de colecciones inteligentes públicas por usuarios no administradores
* Aceleración de descarga
* Jerarquía principal de carpetas compartidas visibles para usuarios no administradores

Estas configuraciones se han proporcionado como **[!UICONTROL configuraciones de Configuración]** general en el panel de herramientas administrativas.

![](assets/general-configs.png)

**** Una configuración que permite a los administradores eliminar recursos de Brand Portal. (El valor predeterminado es habilitado)

**Configuración B** para permitir que los usuarios no administradores creen colecciones públicas. (El valor predeterminado es habilitado)

**Configuración C** para permitir que los usuarios no administradores creen colecciones inteligentes públicas. (El valor predeterminado es habilitado)

**Configuración D** para permitir la aceleración de descarga de recursos descargados del portal y de los vínculos compartidos. (El valor predeterminado está deshabilitado)

**Configuración E** para mostrar la jerarquía de carpetas (desde la raíz) de carpetas compartidas a usuarios no administradores (editores, usuarios invitados, usuarios invitados). (El valor predeterminado está deshabilitado)

## Habilitar/deshabilitar configuraciones generales {#enable-disable-general-configurations}

Para habilitar o deshabilitar cada una de estas configuraciones:

1. Inicie sesión con privilegios de administrador.
2. Seleccione el logotipo de AEM para acceder a las herramientas administrativas, desde la barra de herramientas situada en la parte superior.
3. En el panel de herramientas administrativas, seleccione **[!UICONTROL General]** para abrir la página **[!UICONTROL Configuración]** general.
4. Use el conmutador correspondiente para habilitar/deshabilitar cualquiera de las configuraciones Generales.
5. **[!UICONTROL Guarde los cambios.]**
6. Cierre la sesión para que los cambios surtan efecto.

## Permitir que los usuarios administradores eliminen recursos de Brand Portal {#allow-admin-users-to-delete-assets-from-brand-portal}

**[!UICONTROL Permitir que los usuarios cierren]** la configuración permite a las organizaciones permitir (o restringir) que los usuarios con privilegios de administrador eliminen recursos y carpetas de Brand Portal.

## Permitir la creación de colecciones públicas por usuarios que no son administradores {#allow-public-collections-creation-by-non-admins}

[[! La](../using/brand-portal-share-collection.md#main-pars-text-1915052376) configuración de UICONTROL Permitir colecciones públicas controla si los usuarios no administradores pueden crear colecciones públicas en Brand Portal. La configuración está habilitada de forma predeterminada. Al deshabilitar las organizaciones de configuración, pueden evitarse tener varias colecciones públicas en su portal para poder guardar el espacio del sistema.

## Permitir la creación de colecciones inteligentes públicas por usuarios que no son administradores {#allow-public-smart-collections-creation-by-non-admins}

[[! La configuración de UICONTROL permite la](../using/brand-portal-searching.md#main-pars-header-500620467) configuración de colecciones inteligentes públicas, ya sea que los usuarios no administradores puedan guardar sus búsquedas como colecciones inteligentes y hacerlas públicas para dicho inquilino. La configuración está habilitada de forma predeterminada. Al deshabilitar las organizaciones de configuración, puede evitar tener un gran número de colecciones inteligentes públicas creadas por usuarios no administradores en Brand Portal de la organización.

## Permitir aceleración de descarga {#allow-download-acceleration}

[[! La configuración de UICONTROL Permitir aceleración de](../using/accelerated-download.md) descarga permite a las organizaciones permitir descargas aceleradas de recursos desde Brand Portal y vínculos compartidos, mediante la integración con IBM Aspera Connect que es una aplicación de instalación a petición. La aplicación utiliza tecnología patentada para eliminar las sobrecargas TCP.

## Habilitar la jerarquía de carpetas {#enable-folder-hierarchy}

[[! La configuración de Habilitar jerarquía](../using/brand-portal-sharing-folders.md#non-admin-user-access-to-shared-folders) de carpetas permite a los administradores controlar cómo los usuarios no administradores (editores, usuarios invitados y usuarios invitados) ven las carpetas compartidas tras iniciar sesión.
