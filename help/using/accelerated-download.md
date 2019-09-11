---
title: Acelere las descargas de Brand Portal
seo-title: Acelere las descargas de Brand Portal
description: Mejore el rendimiento de descarga de Brand Portal y de los vínculos compartidos.
seo-description: Mejore el rendimiento de descarga de Brand Portal y de los vínculos compartidos.
uuid: 2871137 e -6471-49 a 7-872 a -841 bd 92543 d 1
contentOwner: mgulati
topic-tags: descarga de descarga
content-type: referencia
products: SG_ EXPERIENCEMANAGER/Brand_ Portal
discoiquuid: 301 f 7 a 0 b -5527-4 aac-b 731-bfc 145 alimentado 0 c 0
translation-type: tm+mt
source-git-commit: fb8243ea896d39b324a69ea534271ee3015c076f

---


# Acelere las descargas de Brand Portal {#guide-to-accelerate-downloads-from-brand-portal}

Brand Portal permite mejorar el rendimiento de descarga de archivos de recursos grandes mediante la integración con IBM Aspera Connect, que es una aplicación de instalación a petición. La aplicación utiliza tecnología patentada para eliminar sobrecargas TCP y mejorar la velocidad de transferencia de los archivos de recursos. Esta integración garantiza una mejor experiencia de descarga.

>[!NOTE]
>
>La velocidad de descarga varía para los usuarios, ya que depende de factores como ancho de banda de la red, latencia del servidor y ubicación geográfica de los clientes.

Si se habilita, los usuarios de Brand Portal pueden reducir significativamente el tiempo empleado para descargar los archivos de recursos deseados desde Brand Portal o desde el vínculo compartido instalando el cliente de Aspera Connect.

![](assets/enable-fast-file-download.png)

## Requisitos previos para acelerar la descarga de archivos {#prerequisites-to-accelerate-file-download}

Para descargar los archivos más rápidamente, asegúrese de lo siguiente:

* **[!UICONTROL Habilite Aceleración de descarga]** (deshabilitada de forma predeterminada) desde [!UICONTROL Configuración general] en el panel de herramientas administrativas.
* Puerto 33001 (tanto TCP como UDP) está abierto en el servidor de seguridad. Para obtener más información sobre los requisitos previos, consulte [Documentación del cliente de Aspera Connect](https://downloads.asperasoft.com/en/documentation/8).
* Instale Aspera Connect con privilegios de administrador.
* Para obtener compatibilidad con plataformas de Aspera Transfer client, consulte [la matriz de compatibilidad con la plataforma Aspera Connect](https://www.asperasoft.com/company/support/transfer-clients/).

## Descargar dominios {#download-domains}

A continuación se muestran los dominios de descarga para diferentes regiones geográficas:

| Código de región | Dominio |
|---|---|
| NA OR 1 | downloads-na1.brand-portal.adobe.com |
| NA VA 5 | downloads-na2.brand-portal.adobe.com |
| EMEA LON 5 | downloads-emea1.brand-portal.adobe.com |
| APAC SIN 2 | downloads-apac1.brand-portal.adobe.com |

## Rendimiento de descarga de muestra mediante el acelerador de archivos {#expected-download-performance-using-file-accelerator}

La siguiente tabla muestra el rendimiento de descarga de 2 GB mediante el acelerador de descargas de archivos Aspera Connect:

**Los resultados observados varían debido a factores como ancho de banda de la red, latencia del servidor y ubicación del cliente, teniendo en cuenta que el servidor de Brand Portal está en Oregon (Estados Unidos).*

| Ubicación del cliente | Latencia entre cliente y servidor (milisegundos) | Velocidad con el acelerador de transferencia de archivos Aspera Connect (MBPS) | Tiempo empleado para descargar el archivo 2 GB con Aspera File Transfer Accelerator (segundos) |
|---------------------------|-----------------------------------|---------------------------------------------|-------------------------------------------------------------------------|
| Estados Unidos Occidental (N. California) | 18 | 36 | 57 |
| Estados Unidos Occidental (Oregón) | 42 | 36 | 57 |
| Estados Unidos (N. Virginia) | 85 | 35 | 58 |
| APAC (Tokio) | 124 | 36 | 57 |
| Noida (India) | 275 | 13.36 | 153 |
| Sídney | 175 | 29 | 70 |
| Londres | 179 | 35 | 58 |
| Singapur | 196 | 34 | 60 |

## Descarga del flujo de trabajo mediante el acelerador de archivos {#download-workflow-using-file-accelerator}

Para descargar recursos más rápidamente desde Brand Portal:

1. Inicie sesión en Brand Portal con un navegador compatible.
2. Busque y seleccione el archivo de recurso, la carpeta o la colección que desee descargar. Toque o haga clic en la opción de descarga.
Se abre el cuadro de diálogo Descargar con [la opción Activar aceleración] de descarga seleccionada.
   ![](assets/download-assetsbp.png)

   >[!NOTE]
   >
   >La funcionalidad para enviar notificaciones por correo electrónico con el vínculo para descargar recursos no se admite en este momento mientras se habilitan las descargas más rápidas.

   ![](assets/fast-download-emailchk.png)

3. Toque o haga clic en **[!UICONTROL la opción Descargar]** .
Para acelerar la experiencia de descarga en su cuenta de usuario de Brand Portal, debe tener instalada la aplicación cliente Aspera Connect en el sistema.

4. **Descargar el cliente
de Aspera Connect** Si el cliente de Aspera Connect no está instalado en el sistema o el cliente instalado de Aspera Connect existente está obsoleto, se muestra un mensaje en la página del navegador desde el que puede descargar el cliente de Aspera Connect específico para el sistema seleccionando **[!UICONTROL Descargar última versión]**.

   ![](assets/aspera-not-launched.png)

   Para descargar la versión más reciente de Aspera Connect desde [https://downloads.asperasoft.com/connect2/](https://downloads.asperasoft.com/connect2/), seleccione **[!UICONTROL Descargar ahora]** y siga las instrucciones.

5. **Instale el cliente
de Aspera Connect** para instalar la configuración del cliente IBM Aspera Connect, ejecute la configuración del archivo. msi de la aplicación cliente IBM Aspera Connect y siga el asistente de instalación.

6. Una vez que el cliente se haya instalado correctamente, actualice la página del explorador e inicie los pasos de descarga de nuevo o seleccione **[!UICONTROL Reiniciar]** en el cuadro **[!UICONTROL de]** diálogo Descargar recurso (paso 2).
Al utilizar Aspera Connect por primera vez, las indicaciones del explorador le permiten abrir el vínculo con **[!UICONTROL IBM Aspera Connect]**. Para omitir este diálogo en el futuro, habilite **[!UICONTROL Recordar mi opción para vínculos FASCIP]**.

   >[!NOTE]
   >
   >Este mensaje es diferente en los distintos exploradores.

7. Un cuadro de diálogo confirma si se realizará la transferencia o no. Seleccione **[!UICONTROL Permitir]** para comenzar.
Para omitir este cuadro de diálogo en el futuro, habilite **[!UICONTROL Utilizar mi opción para todas las conexiones con este host]**.
Comienza la descarga. Un cuadro de diálogo muestra el progreso de la descarga. Utilice el cuadro de diálogo para **[!UICONTROL pausar]**, **[!UICONTROL reanudar]** o **[!UICONTROL cancelar]** la descarga.
La aplicación Aspera Connect proporciona una ventana de actividad en el sistema donde el usuario puede ver y administrar todas las sesiones de transferencia. Para obtener más información, consulte [la documentación del cliente de Aspera Connect](https://downloads.asperasoft.com/en/documentation/8).

![](assets/aspera-activity-window.png)

Cuando se completa correctamente la descarga, un cuadro de diálogo muestra la ubicación en la que se descargan los recursos al sistema del usuario. Si se produce un error, muestra el error.

>[!NOTE]
>
>Existe una limitación conocida en la aplicación cliente de Aspera Connect que no muestra ningún mensaje para seleccionar la ubicación de descarga si **[!UICONTROL se pregunta siempre dónde guardar los archivos]** descargados en la ficha [!UICONTROL Transferencias] dentro [!UICONTROL de Preferencias]. Antes de que comience cualquier descarga, proporcione la ubicación en el cuadro de texto **[!UICONTROL Guardar archivos descargados.]**

## Uso del acelerador de archivos en el navegador Microsoft Edge {#using-file-accelerator-on-microsoft-edge-browser}

Microsoft Edge se ejecuta en modo protegido mejorado (EPM), que impide la comunicación con el servidor de Aspera Connect, en la misma red privada o con un sitio de confianza. Por lo tanto, aparece una ventana emergente cada vez que se establece una conexión con el servidor.

![](assets/switchapps-msedge.png)

Para utilizar la funcionalidad de descarga acelerada en Microsoft Edge, elimine el sitio de Brand Portal de la lista de sitios de confianza.

1. Abra el Panel de control (pulse la tecla **[!UICONTROL Ventana + X]** y, a continuación, seleccione **[!UICONTROL Panel de control]**).
2. Vaya **[!UICONTROL a Red e Internet &gt; Opciones de Internet]**. Haga clic en la ficha **[!UICONTROL Seguridad]** .
3. Haga clic en la zona Sitios **[!UICONTROL de confianza]** y, a continuación, haga clic **[!UICONTROL en Sitios]**.
4. Elimine el sitio de Brand Portal de la lista.

## Preferencias del cliente de Aspera Connect {#aspera-connect-client-preferences}

Hay algunas preferencias útiles que se pueden configurar en la preferencia del cliente de IBM Aspera Connect haciendo clic con el botón derecho en el icono y seleccionando **[!UICONTROL Preferencias]**.

![](assets/download_assets_frombrandportalimg19.png)

Puede establecer la ubicación de descarga predeterminada.

![](assets/aspera-preferences.png)

Además, el cliente de Aspera Connect se puede marcar para iniciar automáticamente el inicio del sistema de modo que el cliente de Connect se esté ejecutando y esté disponible para que la descarga comience más rápido.

![](assets/aspera-automaticallylaunch.png)

## Solución de problemas con la aceleración de descargas {#troubleshoot-issues-with-download-acceleration}

Si la aceleración de descarga no funciona para usted, siga estos pasos para solucionar los problemas:

1. Compruebe que los puertos no están bloqueados al visitar [https://test-connect.asperasoft.com](https://test-connect.asperasoft.com/) desde su ordenador.

   Si los puertos no son correctos, póngase en contacto con su equipo de red y asegúrese de que los Puertos 33001 (ambos TCP y UDP) no están bloqueados en el servidor de seguridad.

2. Si los puertos están correctamente, compruebe si la red no es lenta, midiendo el ancho de banda disponible con [https://www.speedtest.net/](https://www.speedtest.net/).

   Si el ancho de banda es pequeño (1-10 Mbps) o Kbps, utilice las preferencias de Aspera e intente limitar el ancho de banda igual al ancho de banda disponible.

3. Para confirmar si las descargas del servidor de Aspera están funcionando, utilice [https://demo.asperasoft.com/aspera/user](https://demo.asperasoft.com/aspera/user).\
   (inicio de sesión: asperaweb, password: demoaspera)

4. Si no funciona ninguno de los pasos anteriores para solucionar problemas, desactive la opción Activar aceleración de descarga y utilice la descarga normal.
