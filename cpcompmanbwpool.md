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


# Optimizing your bandwidth usage
{: #cp_manbdwpool}

Public data network traffic transferred Outbound from IBM Cloud data centers around the globe are assessed Outbound Bandwidth charges. The charges depend on where the resource transferring the data resides, the amount of data that is egressed and any bandwidth allotments that your purchased IBM cloud products are eligible for. 
{:shortdesc} 

Customers can optimize bandwidth usage by "pooling" all of the bandwidth together for servers into a bandwidth pool. Bandwidth overages for servers in a bandwidth pool are summed up as a whole and overages are calculated only if the total bandwidth of all servers exceeds the total allocated bandwidth for all servers versus metering at the individual server level. 

The pool definitions are listed in the following table: 

| Pool      | Location(s)          |
| ------------- |:-------------:|
| USA    | DAL01<br/><br/>DAL02<br/><br/>DAL04<br/><br/>DAL07<br/><br/>DAL09<br/><br/>DAL10<br/><br/>DAL12<br/><br/>DAL13<br/><br/>HOU02<br/><br/>MON01<br/><br/>SEA01<br/><br/>SJC01<br/><br/>SJC03<br/><br/>SJC04<br/><br/>TOR01<br/><br/>WDC01<br/><br/>WDC04<br/><br/>WDC06<br/><br/>WDC07|
| Amsterdam & London | AMS01<br/><br/>AMS03<br/><br/>LON01<br/><br/>LON02<br/><br/>LON04<br/><br/>LON05<br/><br/>LON06<br/><br/>PAR01 |
| Australia | MEL01<br/><br/>SYD01<br/><br/>SYD04<br/><br/>SYD05 |
| Brazil | SAO01 |
| Frankfurt | FRA02<br/><br/>FRA04<br/><br/>FRA05 |
| India | CHE01 |
| Italy | MIL01 |
| South Korea | SEO01 | 
| Mexico | MEX01 | 
| Norway | OSL01 | 
| Singapore, Hong Kong & Tokyo | HKG02<br/><br/>SNG01<br/><br/>TOK02<br/><br/>TOK04<br/><br/>TOK05 |
{:caption="Table 1. Pooling definitions" caption-side="top"}


## Modifying a bandwidth pool
{: #cp_modbdwpool}

After a bandwidth pool is created, if you're an authorized user, you can access the pool at any time. You access the bandwidth pool to view devices associated with the pool, add devices to the pool, or remove devices from the pool. Use the following steps to access a pool:

1. Log in to the customer portal with your unique credentials.
2. Select **Network** > **Bandwidth** > **Pools** from the menu to access the Bandwidth Pools window.
3. Click the **Pool Name** to access the pool. Each device that is associated with the pool is displayed.
4. From the **Modify** tab, you can rename the pool, add a device, or remove a device from the pool:
  * To rename the pool, enter the new pool name in the field that has the current pool name.
  * To add a device to the pool, from the **Add Servers** list, select the device name, and then click **Select**.
  * To remove a device from a pool, from the **Remove Servers** list, select the device, and then click **Select**.
5. Click **Modify Rack**.
6. Click the **View All Bandwidth Pools** link to return to the Bandwidth Pools window.
