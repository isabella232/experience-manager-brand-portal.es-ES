---
title: Guía para acelerar las descargas desde Brand Portal
seo-title: Guía para acelerar las descargas desde Brand Portal
description: Mejore el rendimiento de descarga de Brand Portal y de los vínculos compartidos.
seo-description: Mejore el rendimiento de descarga de Brand Portal y de los vínculos compartidos.
uuid: 2871137 e -6471-49 a 7-872 a -841 bd 92543 d 1
contentOwner: mgulati
topic-tags: descarga de descarga
content-type: referencia
products: SG_ EXPERIENCEMANAGER/Brand_ Portal
discoiquuid: 301 f 7 a 0 b -5527-4 aac-b 731-bfc 145 alimentado 0 c 0
translation-type: tm+mt
source-git-commit: 770c353b1143d879280df310012ce9d4d30b40c9

---


# Guía para acelerar las descargas desde Brand Portal {#guide-to-accelerate-downloads-from-brand-portal}

Brand Portal admite la descarga acelerada de archivos de recursos grandes mediante la integración con IBM Aspera Connect, que es una aplicación de instalación a petición. La aplicación utiliza tecnología patentada para eliminar sobrecargas TCP y ayuda a mejorar la velocidad de transferencia de los archivos, garantizando así una mejor experiencia de descarga. Los usuarios distribuidos en regiones geográficas, que tienen alta latencia, también pueden beneficiarse de esta capacidad.

>[!NOTE]
>
>IBM Aspera Connect permite la descarga rápida de archivos de recursos grandes de Brand Portal y de vínculos compartidos, pero la velocidad de descarga puede variar dependiendo de factores como ancho de banda de la red, latencia del servidor y ubicación geográfica de los clientes.

Para configurar inquilinos específicos para la descarga de archivos acelerados, los administradores **[!UICONTROL habilitan la aceleración de descarga]** (que está deshabilitada de forma predeterminada) desde **Configuración** general en el panel Herramientas administrativas.

Si se habilita, los usuarios de Brand Portal pueden reducir significativamente el tiempo empleado para descargar los archivos de recursos deseados desde Brand Portal o desde el vínculo compartido instalando el cliente de Aspera Connect.

![](assets/enable-fast-file-download.png)

## Requisitos previos para acelerar la descarga de archivos {#prerequisites-to-accelerate-file-download}

Para utilizar la funcionalidad más rápida de descarga de archivos, asegúrese de:

* Los puertos 33001 (TCP y UDP) se abren en el cortafuegos por administradores. Para obtener más información sobre los requisitos previos para utilizar IBM Aspera Connect, consulte [la documentación del cliente de Aspera Connect](https://downloads.asperasoft.com/en/documentation/8).

   A continuación se muestran los dominios de descarga para diferentes regiones geográficas:

   | Región | Dominio |
   |---|---|
   | NA OR 1 | downloads-na1.brand-portal.adobe.com |
   | NA VA 5 | downloads-na2.brand-portal.adobe.com |
   | EMEA LON 5 | downloads-emea1.brand-portal.adobe.com |
   | APAC SIN 2 | downloads-apac1.brand-portal.adobe.com |

* Los privilegios de administrador se utilizan para descargar el paquete de instalación de IBM Aspera Connect, ya que no se puede instalar Aspera Connect en la cuenta de invitado.

### Requisitos del sistema y del explorador {#system-and-browser-requirements}

Los requisitos del sistema y del explorador para Aspera Connect 3.8.0 son los siguientes:

| ﻿SO | Versión de SO | Explorador |  | Bibliotecas requeridas |
|----------------|----------------------------------------|-------------------|-------|--------------------------|
| Windows | Windows 7, 8, 10 | Chrome | 64-66 |  |
|  | Windows Server 2008, R 2, 2012 R 2, 2016 | Firefox | 57-60 |  |
|  |  | Firefox ESR | 52 |  |
|  |  | Internet Explorer | 11 |  |
|  |  | Microsoft Edge | 39-42 |  |
| Macos | 10.11 - 10.13 | Chrome | 64-66 |  |
|  |  | Firefox | 57-60 |  |
|  |  | Firefox ESR | 52 |  |
|  |  | Safari | 11 |  |
| Linux (64 bits) | RHEL 6 - 7 | Chrome | 64-66 | Openssl 1.0.2 g o superior |
|  | Centos 6 - 7 |  |  | Mesa EGL |
|  | Debian 7 - 9 |  |  | glib 2 2.28 o superior |
|  | SLE 11 - 12 |  |  |  |
|  | Fedora 26 - 27 |  |  |  |
|  | Opensuse 42.3 | Firefox | 57-60 |  |
|  | Ubuntu 14 - 17 | Firefox ESR | 52 |  |

Para obtener compatibilidad con plataformas de diferentes versiones de Aspera Transfer client, consulte [la matriz de compatibilidad con la plataforma Aspera Connect](https://www.asperasoft.com/company/support/transfer-clients/).

## Rendimiento de descarga esperado mediante el acelerador de archivos {#expected-download-performance-using-file-accelerator}

El rendimiento de descarga esperado para un archivo de 2 GB mediante el acelerador de descargas de archivos Aspera Connect en diferentes ubicaciones de cliente es el siguiente, teniendo en cuenta el servidor Brand Portal en Oregón en Estados Unidos:

| Ubicación del cliente | Latencia entre cliente y servidor | Velocidad con Aspera File Transfer Accelerator | Tiempo empleado para descargar un archivo de 2 GB con Aspera File Transfer Accelerator |
|---------------------------|-----------------------------------|---------------------------------------------|-------------------------------------------------------------------------|
| Estados Unidos Occidental (N. California) | 18 milisegundos | 36 MB/s | 57 segundos |
| Estados Unidos Occidental (Oregón) | 42 milisegundos | 36 MB/s | 57 segundos |
| Estados Unidos (N. Virginia) | 85 milisegundos | 35 MB/s | 58 segundos |
| APAC (Tokio) | 124 milisegundos | 36 MB/s | 57 segundos |
| Noida | 275 milisegundos | 13,36 MB/s | 153 segundos |
| Sídney | 175 milisegundos | 29 MB/s | 70 segundos |
| Londres | 179 milisegundos | 35 MB/s | 58 segundos |
| Singapur | 196 milisegundos | 34 MB/s | 60 segundos |

>[!NOTE]
>
>Los datos citados son según las pruebas realizadas en laboratorio y son sólo indicativo. Los resultados observados varían debido a factores como ancho de banda de la red, latencia del servidor y ubicación del cliente.

## Descarga del flujo de trabajo mediante el acelerador de archivos {#download-workflow-using-file-accelerator}

Para descargar recursos más rápidamente desde Brand Portal:

1. Inicie sesión en Brand Portal a través de un navegador preferido.
2. Busque y seleccione el archivo de recurso, la carpeta o la colección que desee descargar. Toque o haga clic en la opción de descarga.
Se abre el cuadro de diálogo Descargar con [la opción Activar aceleración] de descarga seleccionada.
   ![](assets/download-assetsbp.png)

   >[!NOTE]
   >
   >La funcionalidad para enviar notificaciones por correo electrónico con el vínculo para descargar recursos no se admite en este momento mientras se habilitan las descargas más rápidas.

   ![](assets/fast-download-emailchk.png)

3. Toque o haga clic **en Descargar**.
Para acelerar la experiencia de descarga en su cuenta de usuario de Brand Portal, debe tener instalada la aplicación cliente Aspera Connect en el sistema.

4. **Descargar el cliente
de Aspera Connect** Si el cliente de Aspera Connect no está instalado en el sistema o el cliente instalado de Aspera Connect existente está obsoleto, se muestra un mensaje en la página del navegador desde el que puede descargar el cliente de Aspera Connect específico para el sistema seleccionando **Descargar última versión**.

   ![](assets/aspera-not-launched.png)

   Para descargar la versión más reciente de Aspera Connect desde [https://downloads.asperasoft.com/connect2/](https://downloads.asperasoft.com/connect2/), seleccione **Descargar ahora** y siga las instrucciones.

5. **Instale el cliente
de Aspera Connect** para instalar la configuración del cliente IBM Aspera Connect, ejecute la configuración del archivo. msi de la aplicación cliente IBM Aspera Connect y siga el asistente de instalación.

6. Una vez que el cliente se haya instalado correctamente, actualice la página del explorador e inicie los pasos de descarga de nuevo o seleccione **Reiniciar** en el cuadro **de** diálogo Descargar recurso (paso 2).
Al utilizar Aspera Connect por primera vez, las indicaciones del explorador le permiten abrir el vínculo con **IBM Aspera Connect**. Para omitir este diálogo en el futuro, habilite **Recordar mi opción para vínculos FASCIP**.

   >[!NOTE]
   >
   >Este mensaje es diferente en los distintos exploradores.

7. Un cuadro de diálogo confirma si se realizará la transferencia o no. Seleccione **Permitir** para comenzar.
Para omitir este cuadro de diálogo en el futuro, habilite **Utilizar mi opción para todas las conexiones con este host**.
Comienza la descarga. Un cuadro de diálogo muestra el progreso de la descarga. Utilice el cuadro de diálogo para **pausar**, **reanudar** o **cancelar** la descarga.
La aplicación Aspera Connect proporciona una ventana de actividad en el sistema donde el usuario puede ver y administrar todas las sesiones de transferencia. Para obtener más información, consulte [la documentación del cliente de Aspera Connect](https://downloads.asperasoft.com/en/documentation/8).

![](assets/aspera-activity-window.png)

Cuando se completa correctamente la descarga, un cuadro de diálogo muestra la ubicación en la que se descargan los recursos al sistema del usuario. Si se produce un error, muestra el error.

>[!NOTE]
>
>Existe una limitación conocida en la aplicación cliente de Aspera Connect que no muestra ningún mensaje para seleccionar la ubicación de descarga si **se pregunta siempre dónde guardar los archivos** descargados en la ficha** Transferencias** dentro **de Preferencias**. Antes de que comience cualquier descarga, proporcione la ubicación en el cuadro de texto **Guardar archivos descargados.**

## Uso del acelerador de archivos en el navegador Microsoft Edge {#using-file-accelerator-on-microsoft-edge-browser}

Microsoft Edge se ejecuta en modo protegido mejorado (EPM), que impide la comunicación con el servidor de Aspera Connect, en la misma red privada o con un sitio de confianza. Por lo tanto, aparece una ventana emergente cada vez que se establece una conexión con el servidor.

![](assets/switchapps-msedge.png)

Para utilizar la funcionalidad de descarga acelerada en Microsoft Edge, elimine el sitio de Brand Portal de la lista de sitios de confianza.

1. Abra el Panel de control (pulse la tecla **Ventana + X** y, a continuación, seleccione **Panel de control**).
2. Vaya **a Red e Internet &gt; Opciones de Internet**. Click the **Security** tab.
3. Haga clic en la zona Sitios **de confianza** y, a continuación, haga clic **en Sitios**.
4. Elimine el sitio de Brand Portal de la lista.

## Preferencias del cliente de Aspera Connect {#aspera-connect-client-preferences}

Hay algunas preferencias útiles que se pueden configurar en la preferencia del cliente de IBM Aspera Connect haciendo clic con el botón derecho en el icono y seleccionando **Preferencias**.

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
