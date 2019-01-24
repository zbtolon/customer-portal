---

copyright:

  years: 1994, 2018

lastupdated: "2019-01-08"

---

{:shortdesc: .shortdesc}
{:codeblock: .codeblock}
{:tip: .tip}
{:screen: .screen}
{:new_window: target="_blank"}


# Optimización del uso del ancho de banda
{: #cp_manbdwpool}

El tráfico de red de datos públicos de salida de los centros de datos de IBM Cloud en todo el mundo tiene cargos evaluados de ancho de banda de salida. Los cargos dependen del lugar en el que reside el recurso que transfiere los datos, de la cantidad de datos de salida y de las asignaciones de ancho de banda a las que pueden optar los productos de IBM Cloud adquiridos. {:shortdesc} 

Los cliente puede optimizar el uso de ancho de banda "agrupando" todo el ancho de banda correspondiente a los servidores en una agrupación de ancho de banda. Los excedentes de ancho de banda para los servidores de una agrupación de ancho de banda se suman en su totalidad y los excedentes solo se calculan si el ancho de banda total de todos los servidores supera el ancho de banda asignado total para todos los servidores, en lugar de calcularse el nivel de cada servidor individual.
 

Las definiciones de agrupaciones se muestran en la tabla siguiente: 

| Agrupación | Ubicación o ubicaciones|
| ------------- |:-------------:|
| EE.UU.  | DAL01  <br/><br/>DAL02<br/><br/>DAL04<br/><br/> DAL07  <br/><br/> DAL09  <br/><br/> DAL10  <br/><br/>  DAL12  <br/><br/> DAL13  <br/><br/> HOU02  <br/><br/> MON01  <br/><br/>  SEA01  <br/><br/> SJC01  <br/><br/> SJC03  <br/><br/>SJC04<br/><br/>  TOR01  <br/><br/> WDC01  <br/><br/> WDC04  <br/><br/> WDC06  <br/><br/> WDC07  |
| Amsterdam y Londres | AMS01  <br/><br/> AMS03  <br/><br/>LON01<br/><br/>  LON02  <br/><br/>LON04<br/><br/>LON05<br/><br/>LON06<br/><br/> PAR01  |
|Australia| MEL01  <br/><br/> SYD01  <br/><br/>SYD04<br/><br/>SYD05 |
|Brasil| SAO01  |
| Frankfurt | FRA02  <br/><br/>FRA04<br/><br/>FRA05 |
|India| CHE01  |
|Italia| MIL01  |
|Corea del Sur| SEO01  | 
|México| MEX01  | 
|Noruega|  OSL01  | 
| Singapur, Hong Kong y Tokio | HKG02  <br/><br/> SNG01  <br/><br/> TOK02  <br/><br/>TOK04<br/><br/>TOK05 |
{:caption="Tabla 1. Definiciones de agrupaciones" caption-side="top"}


## Modificación de una agrupación de ancho de banda
{: #cp_modbdwpool}

Una vez que se cree una agrupación de ancho de banda, si es un usuario autorizado, puede acceder a la agrupación en cualquier momento. Acceda a la agrupación de ancho de banda para ver los dispositivos asociados con la agrupación, para añadir dispositivos a la agrupación, o para eliminar los dispositivos de la agrupación. Utilice los pasos siguientes para acceder a una agrupación:

1. Inicie sesión en el portal de clientes con sus credenciales exclusivas.
2. Seleccione **Red** > **Ancho de banda** > **Agrupaciones** desde el menú para acceder a la ventana Agrupaciones de ancho de banda.
3. Pulse el **Nombre de agrupación** para acceder a la agrupación. Se mostrará cada dispositivo que esté asociado con la agrupación.
4. Desde el separador **Modificar**, puede renombrar la agrupación, añadir un servicio, o eliminar un dispositivo de la agrupación:
  * Para cambiar el nombre de la agrupación, especifique el nuevo nombre de agrupación en el campo que contiene el nombre de la agrupación actual.
  * Para añadir un dispositivo a la agrupación, desde la lista **Añadir servidores**, seleccione el nombre de dispositivo y luego pulse **Seleccionar**.
  * Para eliminar un dispositivo de una agrupación, desde la lista **Eliminar servidores**, seleccione el dispositivo y luego pulse **Seleccionar**.
5. Pulse **Modificar bastidor**.
6. Pulse el enlace **Ver todas las agrupaciones de ancho de banda** para volver a la ventana Agrupaciones de ancho de banda.
