---

copyright:

  years: 1994, 2018

lastupdated: "2018-05-30"

---

{:shortdesc: .shortdesc}
{:codeblock: .codeblock}
{:tip: .tip}
{:screen: .screen}
{:new_window: target="_blank"}


# Efectuar un pago
{: #customerportal_makepayment}

Todos los detalles de facturación de la infraestructura de {{site.data.keyword.Bluemix}}, desde facturas a información de pago, están almacenados de forma segura en el portal de clientes. Si cambia su método de pago, o si se cancela o caduca su tarjeta de crédito, actualice la información de pago para evitar cargos por retraso.
{:shortdesc}

## Visualización de la factura
{: #cp_viewinvoice}

En la ventana Facturas, cada factura individual viene resumida con su número de factura, fecha, tipo de factura así como con otros saldos monetarios. Las facturas pueden ser de cualquiera de los tipos siguientes:

<dl>
<dt>Nuevo</dt>
<dd>La primera factura de una serie de facturas recurrentes.</dd>
<dt>Recurrente</dt>
<dd>Una factura de cargos recurrentes que han estado activos en la cuenta durante más de un mes.</dd>
<dt>Cargo único</dt>
<dd>Un cargo único para distintos gastos, que podrían incluir los sobrecostes.</dd>
<dt>Crédito</dt>
<dd>Un crédito de la infraestructura de {{site.data.keyword.BluSoftlayer_notm}} en el saldo de su cuenta.</dd>
<dt>Reembolso</dt>
<dd>Una inversión de cargos, para un cargo puntual o recurrente.</dd>
</dl>

También puede ver un resumen de facturación de la cuenta, incluida la información siguiente:
  * Saldo actual y saldo próximo estimado
  * Método de pago
  * Fechas de las últimas y de las próximas facturas recurrentes

1. Pulse **Cuenta** > **Facturación** > **Facturas** en el menú.
2. Puede ver la factura en el portal de clientes o descargarla.

Si está viendo la factura en el portal de clientes, se mostrará una lista detallada de elementos de facturación para la factura seleccionada. Pulse en cualquier lugar de la línea para un elemento de facturación para ver más detalles sobre el cargo. Si ha descargado la factura, podrá verla en función de los valores del navegador. Las facturas descargadas proporcionan una factura de resumen desglosada y una factura detallada desglosada para cada elemento de facturación.

## Adición de un método de pago
{: #cp_cpmanacctbillpay}

Es obligatorio que cada cuenta de SoftLayer tenga una tarjeta de crédito registrada a la que se le cargue automáticamente la cantidad de la factura cada mes. Esta información debe estar siempre actualizada para evitar pagos atrasados; puede actualizarla en cualquier momento para garantizar que la información de pago sea siempre precisa. Si la información de la tarjeta de crédito registrada es correcta pero se debe aplicar una forma de pago alternativa al saldo actual, consulte [Realizar un pago único](/docs/customer-portal/cpmanacctbillpay.html#cp_makeonetimepayment). Utilice los pasos siguientes para añadir un método de pago para una cuenta en el portal de clientes.

1. Pulse **Cuenta** > **Facturación** > **Método de pago** en el menú.
2. Especifique los detalles de facturación necesarios para la tarjeta en cada campo de la sección **Dirección de facturación**.
> **Nota:** Pulse el recuadro de selección **Utilizar la información de la empresa** para completar automáticamente los campos con la información de la empresa que la infraestructura de {{site.data.keyword.BluSoftlayer_notm}} tiene registrada para la cuenta.
3. Especifique la información de la tarjeta de crédito en cada campo de la sección **Información de pago**.
4. Pulse **Añadir tarjeta de crédito** para añadir la tarjeta de crédito como método de pago mensual.
5. Opcionalmente, seleccione **Soporte en la UE** para asegurarse de que el equipo de soporte de Europa gestione los problemas de mantenimiento y de soporte.  Para obtener más información sobre esta opción, consulte [Establecimiento de la opción de equipo de soporte europeo exclusivo](/docs/customer-portal/pay-invoice.html#cp_seteusupported).

Después de añadir el método de pago, la solicitud será procesada por los representantes de la cuenta de SoftLayer para garantizar la validez de la tarjeta. Las tarjetas validadas estarán disponibles para su uso en la cuenta dentro de 24 horas. El cambio de estado para el método de pago será enviado por correo electrónico al contacto proporcionado al añadir el método de pago.

## Realizar un pago único
{: #cp_makeonetimepayment}

Puede realizar pagos únicos utilizando una cuenta de PayPal o una tarjeta de crédito principal y puede realizar pagos para un saldo completo o parcial. Los detalles de los pagos puntuales no se registran para su uso futuro y no modifican los métodos de pago mensuales actuales para la cuenta.

1. Vaya a la página Realizar un pago único en el portal de clientes.
 * Desde el menú: Vaya a **Cuenta** > **Realizar un pago**.
 * Desde la página Facturas: Pulse **Pagar saldo**.
2. Especifique el importe de pago en el campo **Importe de pago**.
3. Si está realizando el pago con PayPal, pulse **PayPal** y siga las indicaciones de PayPal para completar el pago. No es necesaria ninguna otra acción. Si está realizando el pago con una tarjeta de crédito, especifique el **Número, fecha de caducidad y código de seguridad de la tarjeta** en los campos apropiados.
4. Especifique la información de facturación en los campos apropiados en la sección **Dirección de facturación de la tarjeta de crédito**.
5. Opcionalmente, seleccione **Soporte en la UE** para asegurarse de que el equipo de soporte de Europa gestione los problemas de mantenimiento y de soporte.  Para obtener más información sobre esta opción, consulte [Establecimiento de la opción de equipo de soporte europeo exclusivo](/docs/customer-portal/pay-invoice.html#cp_seteusupported).
6. Pulse **Pagar con tarjeta de crédito** para iniciar el pago.

Después de iniciar el pago, este se procesará. Si surgen problemas con el pago, siga las indicaciones de la infraestructura de {{site.data.keyword.BluSoftlayer_notm}} o de PayPal hasta que se resuelva el problema. El pago se procesará. Se aplicará el importe y se actualizará el saldo actual.
