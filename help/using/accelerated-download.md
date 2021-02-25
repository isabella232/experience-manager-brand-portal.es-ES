---
title: Acelerar las descargas de Brand Portal
seo-title: Acelerar las descargas de Brand Portal
description: Mejore el rendimiento de las descargas desde Brand Portal y los vínculos compartidos.
seo-description: Mejore el rendimiento de las descargas desde Brand Portal y los vínculos compartidos.
uuid: 2871137e-6471-49a7-872a-841bd92543d1
contentOwner: mgulati
topic-tags: download-install
content-type: reference
products: SG_EXPERIENCEMANAGER/Brand_Portal
discoiquuid: 301f7a0b-5527-4aac-b731-bfc145fed0c0
translation-type: tm+mt
source-git-commit: fab0855e8d30e7b6ddf9b4ae5b2ce1fb627c81ce
workflow-type: tm+mt
source-wordcount: '1049'
ht-degree: 3%

---


# Acelerar las descargas de Brand Portal {#guide-to-accelerate-downloads-from-brand-portal}

El portal de marca Adobe Experience Manager Assets permite mejorar el rendimiento de descarga de archivos de recursos de gran tamaño mediante la integración con IBM Aspera Connect, una aplicación de instalación bajo demanda. La aplicación utiliza tecnología patentada para eliminar los sobrecargos TCP y ayuda a mejorar la velocidad de transferencia de los archivos de recursos. Esta integración garantiza una mejor experiencia de descarga.

>[!NOTE]
>
>La velocidad de descarga varía para los usuarios, ya que depende de factores como el ancho de banda de la red, la latencia del servidor y la ubicación geográfica de los clientes.

La configuración **[!UICONTROL Descarga rápida]** está habilitada de forma predeterminada, lo que reduce considerablemente el tiempo necesario para descargar los archivos de recursos deseados desde Brand Portal.

![](assets/download-settings-new.png)

## Requisitos previos para acelerar la descarga de archivos {#prerequisites-to-accelerate-file-download}

Para descargar los archivos más rápidamente, asegúrese de lo siguiente:

* Vaya a **[!UICONTROL Herramientas]** > **[!UICONTROL Descargar]** y verifique que la configuración de **[!UICONTROL Descarga rápida]** esté habilitada en **[!UICONTROL Configuración de descarga]**.
* Asegúrese de que el puerto 33001 (TCP y UDP) esté abierto en el servidor de seguridad. Para obtener más información sobre los requisitos previos, consulte la [documentación del cliente de IBM Aspera Connect](https://downloads.asperasoft.com/en/documentation/8).
* [Instale IBM Aspera Connect 3.9.9](https://www.ibm.com/support/knowledgecenter/SSXMX3_3.9.9/kc/connect_welcome.html) en la extensión de su navegador mediante privilegios de administrador.
* Para obtener compatibilidad con plataformas del cliente de transferencia Aspera, consulte [Matriz de soporte de plataformas IBM Aspera Connect](https://www.asperasoft.com/company/support/transfer-clients/).

## Descargar dominios {#download-domains}

A continuación se muestran los dominios de descarga de diferentes regiones geográficas:

| Código de región | Dominio |
|---|---|
| NA OR1 | downloads-na1.brand-portal.adobe.com |
| NA VA5 | downloads-na2.brand-portal.adobe.com |
| EMEA LON5 | downloads-emea1.brand-portal.adobe.com |
| APAC SIN2 | downloads-apac1.brand-portal.adobe.com |

## Ejemplo de rendimiento de descarga mediante el acelerador de archivos {#expected-download-performance-using-file-accelerator}

La siguiente tabla muestra el rendimiento de descarga de un archivo de 2 GB mediante el acelerador de descargas de archivos de Aspera Connect:

*Los resultados observados varían debido a factores como el ancho de banda de la red, la latencia del servidor y la ubicación del cliente, teniendo en cuenta que el servidor de Brand Portal se encuentra en Oregon (Estados Unidos).*

| Ubicación del cliente | Latencia entre cliente y servidor (milisegundos) | Velocidad con el acelerador de transferencia de archivos Aspera Connect (MBps) | Tiempo necesario para descargar un archivo de 2 GB con el acelerador de transferencia de archivos de Aspera (segundos) |
|---------------------------|-----------------------------------|---------------------------------------------|-------------------------------------------------------------------------|
| Oeste de EE.UU. (N. California) | 18 | 36 | 57 |
| Oeste de EE.UU. (Oregón) | 42 | 36 | 57 |
| U.S. East (N. Virginia) | 85 | 35 | 58 |
| APAC (Tokio) | 124 | 36 | 57 |
| Adobe (India) | 275 | 13,36 | 153 |
| Sídney | 175 | 29 | 70 |
| Londres | 179 | 35 | 58 |
| Singapur | 196 | 34 | 60 |

## Descargar flujo de trabajo mediante el acelerador de archivos {#download-workflow-using-file-accelerator}

Para descargar recursos más rápido desde Brand Portal:

1. Inicie sesión en el inquilino de Brand Portal. De forma predeterminada, se abre la vista **[!UICONTROL Archivos]**, que contiene todos los recursos y carpetas publicados.

   Realice una de las acciones siguientes:

   * Seleccione los recursos o las carpetas que desee descargar. En la barra de herramientas de la parte superior, haga clic en el icono **[!UICONTROL Descargar]**.

      ![select-multiple-assets](assets/select-assets-new.png)

   * Para descargar representaciones de recursos específicas de un recurso, pase el puntero sobre el recurso y haga clic en el icono **[!UICONTROL Descargar]** disponible en las miniaturas de acción rápida.

      ![select-asset](assets/select-asset.png)

1. Se abre el cuadro de diálogo **[!UICONTROL Descargar]** con todos los recursos seleccionados.

   Para conservar la jerarquía de carpetas de Brand Portal al descargar recursos, active la casilla de verificación **[!UICONTROL Crear carpeta independiente para cada recurso]**.

   El botón de descarga refleja el recuento de los elementos seleccionados. Una vez que haya terminado de aplicar las reglas, haga clic en **[!UICONTROL Descargar elementos]**. Para obtener más información sobre cómo aplicar reglas, consulte [descarga de recursos](../using/brand-portal-download-assets.md#download-assets).

   ![download-dialog](assets/download-dialog-box-new.png)

1. De forma predeterminada, la configuración **[!UICONTROL Descarga rápida]** está habilitada en la **[!UICONTROL Configuración de descarga]**. Por lo tanto, aparece un cuadro de confirmación para descargar recursos con IBM Aspera Connect.

   Si está descargando los recursos por primera vez y no tiene instalado IBM Aspera Connect en su explorador o la versión existente no está actualizada, le pedirá que [instale el acelerador de descargas de Aspera](https://www.ibm.com/support/knowledgecenter/SSXMX3_3.9.9/kc/connect_welcome.html).

   ![](assets/aspera-not-launched.png)

1. **Instalación de Aspera Connect Client**

   Para instalar la configuración del cliente de IBM Aspera Connect, ejecute la instalación desde el archivo .msi de la aplicación cliente IBM Aspera Connect y siga el asistente de instalación.

   ![](assets/aspera-download-1.png)

1. Una vez que el cliente se haya instalado correctamente, actualice la página del explorador e inicie los pasos de descarga de nuevo.

1. Para continuar usando **[!UICONTROL Descarga rápida]**, haga clic en **[!UICONTROL Permitir]**. Todas las representaciones seleccionadas se descargan en una carpeta zip con IBM Aspera Connect.

   Una vez completada la descarga, un cuadro de diálogo muestra la ubicación en la que se descargan los recursos en el sistema del usuario.

   ![](assets/aspera-download-2.png)

   Si no desea utilizar IBM Aspera Connect, haga clic en **[!UICONTROL Denegar]**. Si **[!UICONTROL Fast Download]** se deniega o falla, el sistema rellena un mensaje de error. Haga clic en el botón **[!UICONTROL Descarga normal]** para continuar descargando los recursos.

>[!NOTE]
>
>Si el administrador desactiva la configuración de **[!UICONTROL Descarga rápida]**, las representaciones seleccionadas se descargan directamente en una carpeta zip sin utilizar IBM Aspera Connect.

<!-- 
On successful completion of the download, a dialog box shows the location where assets are downloaded onto the user's system. If there is a failure, it shows error.

   >[!NOTE]
   >
   >There is a known limitation in Aspera Connect client application that no prompt to select download location appears if **[!UICONTROL Always ask me where to save downloaded files]** is enabled under the tab **[!UICONTROL Transfers]** within **[!UICONTROL Preferences]**. Before any download begins, provide the location in the text box **[!UICONTROL Save downloaded files to]**.


1. Log in to Brand Portal using a supported browser.
1. Browse and select the folders or assets you want to download. From the toolbar at the top, click the **[!UICONTROL Download]** icon. the **[!UICONTROL Download]** dialog appears with the **[!UICONTROL Asset(s)]** and **[!UICONTROL Enable download acceleration]** check boxes selected by default. 

   ![](assets/download-assetsbp.png)

   >[!NOTE]
   >
   >The functionality to send email notification with the link to download assets is presently not supported while faster downloads are enabled.

   ![](assets/fast-download-emailchk.png)

1. Click **[!UICONTROL Download]**.

   To speed up the download experience on your Brand Portal tenant account, you need to have Aspera Connect client application installed in your browser's extension.

1. **Download Aspera Connect Client**

   If Aspera Connect client is not installed on your system or the existing Aspera Connect client is out of date, a prompt is displayed on the browser page from where you can download the system-specific Aspera Connect client by selecting **[!UICONTROL Download Latest Version]**.

   ![](assets/aspera-not-launched.png)

   To download the latest version of Aspera Connect from [https://downloads.asperasoft.com/connect2/](https://downloads.asperasoft.com/connect2/), select **[!UICONTROL Download Now]** and follow the instructions.

1. **Install Aspera Connect Client**

   To install IBM Aspera Connect client setup, run the setup from  .msi  file of IBM Aspera Connect client application and follow the installation wizard.

1. Once the client is successfully installed, refresh the browser page and initiate the download steps again.

   When using Aspera Connect for the first time, the browser prompts to open the link using **[!UICONTROL IBM Aspera Connect]**. To skip this dialog in future, enable **[!UICONTROL Remember my choice for FASP links]**.

   >[!NOTE]
   >
   >This message is different on the different browsers.

1. A dialog box confirms whether to proceed the transfer or not. Select **[!UICONTROL Allow]** to begin.
To skip this dialog in future, enable **[!UICONTROL Use my choice for all connections with this host]**.
Download begins. A dialog box shows the progress of the download. Use the dialog box to **[!UICONTROL pause]**, **[!UICONTROL resume]**, or **[!UICONTROL cancel]** the download.
Aspera Connect application provides an Activity Window on the system where user can view and manage all transfer sessions. For more information, refer [Aspera Connect Client documentation](https://downloads.asperasoft.com/en/documentation/8).

![](assets/aspera-activity-window.png)

On successful completion of the download, a dialog box shows the location where assets are downloaded onto the user's system. If there is a failure, it shows error.

   >[!NOTE]
   >
   >There is a known limitation in Aspera Connect client application that no prompt to select download location appears if **[!UICONTROL Always ask me where to save downloaded files]** is enabled under the tab **[!UICONTROL Transfers]** within **[!UICONTROL Preferences]**. Before any download begins, provide the location in the text box **[!UICONTROL Save downloaded files to]**.
-->

## Uso del acelerador de archivos en el navegador Microsoft Edge {#using-file-accelerator-on-microsoft-edge-browser}

Microsoft Edge se ejecuta en modo protegido mejorado (EPM) para evitar la comunicación con el servidor de Aspera Connect, en la misma red privada o con un sitio de confianza. Por lo tanto, aparece una ventana emergente cada vez que se establece una conexión con el servidor.

![](assets/switchapps-msedge.png)

Para utilizar la funcionalidad de descarga acelerada en Microsoft Edge, elimine el sitio de Brand Portal de la lista del sitio de confianza.

1. Abra el Panel de control de Campaign (**[!UICONTROL Tecla de ventana + X]**, luego seleccione **[!UICONTROL Panel de control de Campaign]**).
1. Vaya a **[!UICONTROL Red e Internet]** > **[!UICONTROL Opciones de Internet]**. Haga clic en la ficha **[!UICONTROL Seguridad]**.
1. Haga clic en la **[!UICONTROL zona de sitios de confianza]** y, a continuación, haga clic en **[!UICONTROL Sitios]**.
1. Elimine el sitio de Brand Portal de la lista.

## Preferencias del cliente de Aspera Connect {#aspera-connect-client-preferences}

Existen algunas preferencias útiles que se pueden establecer en la preferencia del cliente de IBM Aspera Connect haciendo clic con el botón derecho en el icono y seleccionando **[!UICONTROL Preferencias]**.

![](assets/download_assets_frombrandportalimg19.png)

Puede establecer la ubicación de descarga predeterminada.

![](assets/aspera-preferences.png)

Además, el cliente de Aspera Connect se puede marcar para que se active el inicio automáticamente al iniciar el sistema, de modo que el cliente de Connect se esté ejecutando y esté disponible para que la descarga comience más rápido.

![](assets/aspera-automaticallylaunch.png)

## Solución de problemas con la aceleración de descarga {#troubleshoot-issues-with-download-acceleration}

Si la aceleración de la descarga no funciona correctamente, siga estos pasos para solucionar el problema:

1. Compruebe que los puertos no están bloqueados, visitando [https://test-connect.asperasoft.com](https://test-connect.asperasoft.com/) desde su equipo.

   Si los puertos no están bien, póngase en contacto con el equipo de red y asegúrese de que los puertos 33001 (tanto TCP como UDP) no estén bloqueados en el servidor de seguridad.

1. Si los puertos están bien, compruebe si la red no es lenta, midiendo el ancho de banda disponible mediante [https://www.speedtest.net/](https://www.speedtest.net/).

   Si el ancho de banda es de unos pocos (1-10 Mbps) o en kbps, utilice las preferencias de Aspera e intente limitar el ancho de banda igual al ancho de banda disponible.

1. Para confirmar si las descargas del servidor de demostración de Aspera están funcionando, utilice [https://demo.asperasoft.com/aspera/user](https://demo.asperasoft.com/aspera/user).\
   (inicio de sesión:  asperaweb , contraseña:  demoaspera )

1. Si ninguno de los pasos de solución de problemas anteriores funciona, anule la selección de la opción Activar aceleración de descarga y utilice la descarga normal.
