---
title: Acelerar las descargas de Brand Portal
seo-title: Acelerar las descargas de Brand Portal
description: Mejore el rendimiento de las descargas desde Brand Portal y los vínculos compartidos.
seo-description: Mejore el rendimiento de las descargas desde Brand Portal y los vínculos compartidos.
uuid: 2871137e-6471-49a7-872a-841bd92543d1
contentOwner: mgulati
topic-tags: download-install
content-type: referencia
products: SG_EXPERIENCEMANAGER/Brand_Portal
discoiquuid: 301f7a0b-5527-4aac-b731-bfc145feed0c0
translation-type: tm+mt
source-git-commit: fb8243ea896d39b324a69ea534271ee3015c076f

---


# Acelerar las descargas de Brand Portal {#guide-to-accelerate-downloads-from-brand-portal}

Brand Portal permite mejorar el rendimiento de descarga de archivos de recursos de gran tamaño mediante la integración con IBM Aspera Connect, una aplicación de instalación bajo demanda. La aplicación utiliza tecnología patentada para eliminar los sobrecargos TCP y ayuda a mejorar la velocidad de transferencia de los archivos de recursos. Esta integración garantiza una mejor experiencia de descarga.

>[!NOTE]
>
>La velocidad de descarga varía para los usuarios, ya que depende de factores como el ancho de banda de la red, la latencia del servidor y la ubicación geográfica de los clientes.

Si está activada, los usuarios de Brand Portal pueden reducir considerablemente el tiempo necesario para descargar los archivos de recursos deseados desde Brand Portal o a través de un vínculo compartido mediante la instalación del cliente de Aspera Connect.

![](assets/enable-fast-file-download.png)

## Requisitos previos para acelerar la descarga de archivos {#prerequisites-to-accelerate-file-download}

Para descargar los archivos más rápidamente, asegúrese de lo siguiente:

* **[!UICONTROL Habilite la aceleración]** de descarga (que está deshabilitada de forma predeterminada) desde Configuración  general en el panel Herramientas administrativas.
* El puerto 33001 (TCP y UDP) está abierto en el servidor de seguridad. Para obtener más información sobre los requisitos previos, consulte la documentación [del cliente de](https://downloads.asperasoft.com/en/documentation/8)Aspera Connect.
* Instale Aspera Connect con privilegios de administrador.
* Para obtener compatibilidad con plataformas del cliente de transferencia Aspera, consulte Matriz [de compatibilidad con plataformas](https://www.asperasoft.com/company/support/transfer-clients/)Aspera Connect.

## Descargar dominios {#download-domains}

A continuación se muestran los dominios de descarga de diferentes regiones geográficas:

| Código de región | Dominio |
|---|---|
| NA OR1 | downloads-na1.brand-portal.adobe.com |
| NA VA5 | downloads-na2.brand-portal.adobe.com |
| EMEA LON5 | downloads-emea1.brand-portal.adobe.com |
| APAC SIN2 | downloads-apac1.brand-portal.adobe.com |

## Sample download performance using file accelerator {#expected-download-performance-using-file-accelerator}

La siguiente tabla muestra el rendimiento de descarga de un archivo de 2 GB mediante el acelerador de descargas de archivos de Aspera Connect:

*The observed results do vary due to factors such as network bandwidth, server latency, and client location, considering Brand Portal server is at Oregon (United States).**

| Client location | Latency between client and server (milliseconds) | Speed with Aspera Connect File Transfer Accelerator (MBps) | Time taken to download 2 GB file with  Aspera File Transfer Accelerator (seconds) |
|---------------------------|-----------------------------------|---------------------------------------------|-------------------------------------------------------------------------|
| U.S. West (N. California) | 18 | 36 | 57 |
| U.S. West (Oregon) | 42 | 36 | 57 |
| U.S. East (N. Virginia) | 85 | 35 | 58 |
| APAC (Tokyo) | 124 | 36 | 57 |
| Noida (India) | 275 | 13.36 | 153 |
| Sídney | 175 | 29 | 70 |
| Londres | 179 | 35 | 58 |
| Singapur | 196 | 34 | 60 |

## Descargar flujo de trabajo mediante el acelerador de archivos {#download-workflow-using-file-accelerator}

To download assets faster from Brand Portal:

1. Inicie sesión en Brand Portal con un navegador compatible.
2. Busque y seleccione el archivo, la carpeta o la colección de recursos que desee descargar. Toque o haga clic en la opción de descarga.
Aparece el cuadro de diálogo Descargar con la opción [Activar aceleración] de descarga seleccionada.
   ![](assets/download-assetsbp.png)

   >[!NOTE]
   >
   >Actualmente no se admite la funcionalidad de enviar notificaciones por correo electrónico con el vínculo para descargar recursos mientras se habilitan las descargas más rápidas.

   ![](assets/fast-download-emailchk.png)

3. Toque o haga clic en la opción **[!UICONTROL Descargar]** .
Para acelerar la experiencia de descarga en la cuenta de inquilino de Brand Portal, debe tener instalada la aplicación cliente Aspera Connect en el sistema.

4. **Descargar Aspera Connect Client** Si el cliente de Aspera Connect no está instalado en el sistema o el cliente de Aspera Connect instalado no está actualizado, se mostrará un mensaje en la página del navegador desde la que podrá descargar el cliente de Aspera Connect específico del sistema seleccionando **[!UICONTROL Descargar la versión]** más reciente.

   ![](assets/aspera-not-launched.png)

   Para descargar la versión más reciente de Aspera Connect desde [https://downloads.asperasoft.com/connect2/](https://downloads.asperasoft.com/connect2/), seleccione **[!UICONTROL Descargar ahora]** y siga las instrucciones.

5. **Instalación de Aspera Connect Client** Para instalar la configuración del cliente de IBM Aspera Connect, ejecute la configuración desde el archivo .msi de la aplicación cliente IBM Aspera Connect y siga el asistente de instalación.

6. Una vez que el cliente se haya instalado correctamente, actualice la página del explorador e inicie los pasos de descarga de nuevo o seleccione **[!UICONTROL Reiniciar]** en el cuadro de diálogo **[!UICONTROL Descargar]** recurso (paso 2).
Al utilizar Aspera Connect por primera vez, el navegador solicita que se abra el vínculo mediante **[!UICONTROL IBM Aspera Connect]**. Para omitir este cuadro de diálogo en el futuro, habilite **[!UICONTROL Recordar mi selección para los vínculos]** FASP.

   >[!NOTE]
   >
   >Este mensaje es diferente en los distintos navegadores.

7. Un cuadro de diálogo confirma si se debe continuar con la transferencia o no. Seleccione **[!UICONTROL Permitir]** que comience.
Para omitir este cuadro de diálogo en el futuro, habilite **[!UICONTROL Usar mi opción para todas las conexiones con este host]**.
Comienza la descarga. Un cuadro de diálogo muestra el progreso de la descarga. Utilice el cuadro de diálogo para **[!UICONTROL pausar]**, **[!UICONTROL reanudar]** o **[!UICONTROL cancelar]** la descarga.
La aplicación Aspera Connect proporciona una ventana de actividad en el sistema donde el usuario puede ver y administrar todas las sesiones de transferencia. Para obtener más información, consulte la documentación [del cliente de](https://downloads.asperasoft.com/en/documentation/8)Aspera Connect.

![](assets/aspera-activity-window.png)

On successful completion of the download, a dialog box shows the location where assets are downloaded to user's system. Si hay un error, muestra un error.

>[!NOTE]
>
>Existe una limitación conocida en la aplicación cliente de Aspera Connect de que no aparece ningún mensaje para seleccionar la ubicación de descarga si **[!UICONTROL Preguntarme siempre dónde guardar los archivos]** descargados está habilitado en la ficha [!UICONTROL Transferencias] en [!UICONTROL Preferencias]. Antes de comenzar la descarga, especifique la ubicación en el cuadro de texto **[!UICONTROL Guardar los archivos descargados en]**.

## Using file accelerator on Microsoft Edge browser {#using-file-accelerator-on-microsoft-edge-browser}

Microsoft Edge runs in Enhanced Protected Mode (EPM) preventing communication with the Aspera Connect server, while on same private network or with a Trusted Site. Por lo tanto, aparece una ventana emergente cada vez que se establece una conexión con el servidor.

![](assets/switchapps-msedge.png)

To use accelerated download functionality on Microsoft Edge, remove the Brand Portal site from the trusted site list.

1. Open the Control Panel (press Window key + X, then select Control Panel).********
2. Go to Network and Internet &gt; Internet Options. **** Click the Security tab.****
3. Haga clic en la zona **[!UICONTROL Sitios de]** confianza y, a continuación, haga clic en **[!UICONTROL Sitios]**.
4. Remove Brand Portal site from the list.

## Aspera Connect client Preferences {#aspera-connect-client-preferences}

There are a few useful preferences which can be set in IBM Aspera Connect Client preference by right clicking the icon and selecting Preferences.****

![](assets/download_assets_frombrandportalimg19.png)

Puede establecer la ubicación de descarga predeterminada.

![](assets/aspera-preferences.png)

Also, the Aspera Connect client can be marked to automatically start on system startup so that the connect client is running and available for the download to begin faster.

![](assets/aspera-automaticallylaunch.png)

## Troubleshoot issues with download acceleration {#troubleshoot-issues-with-download-acceleration}

If download acceleration is not working for you, follow these steps to troubleshoot:

1. Check that ports are not blocked, by visiting https://test-connect.asperasoft.com from your machine.[](https://test-connect.asperasoft.com/)

   If ports are not OK, then reach out to your network team and ensure that Ports 33001 (both TCP &amp; UDP) are not blocked in the firewall.

2. Si los puertos están bien, compruebe si la red no es lenta, midiendo el ancho de banda disponible mediante [https://www.speedtest.net/](https://www.speedtest.net/).

   Si el ancho de banda es de unos pocos (1-10 Mbps) o en kbps, utilice las preferencias de Aspera e intente limitar el ancho de banda igual al ancho de banda disponible.

3. Para confirmar si las descargas del servidor de demostración de Aspera están funcionando, utilice [https://demo.asperasoft.com/aspera/user](https://demo.asperasoft.com/aspera/user).\
   (inicio de sesión:  asperaweb , contraseña:  demoaspera )

4. Si ninguno de los pasos de solución de problemas anteriores funciona, anule la selección de la opción Activar aceleración de descarga y utilice la descarga normal.
