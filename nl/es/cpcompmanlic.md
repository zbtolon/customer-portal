---

copyright:

  years: 1994, 2018

lastupdated: "2017-12-06"

---

{:shortdesc: .shortdesc}
{:codeblock: .codeblock}
{:tip: .tip}
{:screen: .screen}
{:new_window: target="_blank"}

# Gestión de dispositivos
{: #cp_compacclisc}

Puede gestionar las licencias para el software del panel de control activo, como cPanel y Parallels, desde el portal del cliente en la ventana Licencias del panel de control. Puede ver licencias y sus IP asociados, descargar archivos de licencia y cancelar licencias individuales. También puede gestionar las contraseñas para el software en cada dispositivo desde el Portal del cliente.
{:shortdesc}


## Descarga de una licencia para un dispositivo
{: #cp_compdllisc}

Un archivo de licencia se utiliza para verificar que la licencia es válida para el software en un dispositivo, y cualquier característica de software que esté habilitada. Puede descargar archivos de licencia desde el portal del cliente, pero sólo en el dispositivo que ejecuta el software de panel de control correspondiente. Utilice los pasos siguientes para descargar un archivo de licencia.

1. Inicie sesión en el portal del cliente con sus credenciales exclusivas.
2. Seleccione **Dispositivos** > **Gestionar** > **Licencias del panel de control** desde el menú para acceder a la ventana Licencias de panel de control.
3. Seleccione **Acciones > Descargar archivo de licencia** para la licencia.
4. Guarde o descargue el archivo en el software del panel de control en el dispositivo utilizando las solicitudes proporcionadas por el sistema operativo del dispositivo.

Después de descargar el archivo de licencia en el dispositivo, se actualizarán los detalles del software del panel de control sobre la licencia. Si se producen problemas o si la descarga no ha sido satisfactoria, intente el proceso de descarga de nuevo repitiendo los pasos anteriores.

## Cancelación de una licencia de panel de control
{: #cp_compcanlisc}

Las licencias de panel de control se facturarán mensualmente, basándose en los términos acordados en el momento de adquirir la licencia. Puede cancelar licencias en cualquier momento y se cancelarán en la fecha del próximo aniversario de facturación. Para asegurarse de que una cancelación se haya aplicado de forma apropiada al ciclo de facturación actual, las cancelaciones deben realizarse no menos de 24 horas antes de la fecha de aniversario de facturación. La información específica sobre el aniversario de facturación de la cuenta se mostrará durante el proceso de cancelación. Utilice los pasos siguientes para cancelar una licencia de panel de control.

1. Realice una copia de seguridad o transfiera los datos asociados con la licencia del panel de control.
2. Inicie sesión en el portal del cliente con sus credenciales exclusivas.
3. Seleccione **Dispositivos** > **Gestionar** > **Licencias del panel de control** desde el menú para acceder a la ventana Licencias de panel de control.
4. Seleccione **Acciones** > **Cancelar** para la licencia del panel de control que desee cancelar.
5. Escriba las notas relativas a la cancelación en el recuadro de texto **Notas**.
6. Pulse **Continuar** para avanzar a la pantalla de confirmación.
7. Marque el recuadro de selección **Reconocimiento de pérdida de datos**.

  Si no ha realizado copia de seguridad de los datos importantes, vuelva al primer paso y copie todos los datos antes de cancelar la licencia.
  {: tip}

8. Pulse **Cancelar licencia**.

Después de iniciar el proceso de cancelación, la licencia del panel de control está planificada para la cancelación para la siguiente fecha de aniversario de facturación. Si la cancelación se realizó en error, puede anular la cancelación en la pantalla Cancelaciones en el portal del cliente.

## Gestión de las contraseñas de software en dispositivos
{: #cp_bpmanacctresp}

Se asigna una contraseña a cada parte de software que se suministra en un dispositivo, la cual se genera automáticamente mediante los sistemas de infraestructura de {{site.data.keyword.BluSoftlayer_notm}}. Las contraseñas de software para cada dispositivo se almacenan en el separador **Contraseñas** de la pantalla Detalles de dispositivo en el portal del cliente.  Después de acceder al software por primera vez, cambie las contraseñas. Opcionalmente, puede almacenar credenciales de software en el separador **Contraseñas** para cada dispositivo. Sin embargo, cuando almacena contraseñas en el portal del cliente, cualquier persona con acceso a la cuenta y con permisos apropiados podrá ver estas contraseñas.
