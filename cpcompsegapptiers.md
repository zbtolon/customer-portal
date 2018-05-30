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

# Securing and scaling your environment
{: #cp_compsegapptierssecscal}

When you host an application, two of the most critical aspects to consider for any system administrator are the security and scalability of the application.
{:shortdesc}

## Securing your systems with firewalls
{: #cp_bpsecuresystem}

Use the available hardware firewalls to ensure that your device is always secure. You can provision hardware firewalls on demand with no downtime, if rules are established properly, to protect your server from unwanted activity.

Firewalls are add-on services to any devices that you must manually configure and enable to ensure that they are effective. You can lock down superfluous ports and disable public ports for private network-based systems to further manage outside accessibility to your systems. Regular vulnerability scans in the customer portal identify any outstanding or unknown security risks so that you can mitigate risks quickly.

After you order your firewall, it must be enabled and rules must be set.

### Activating your firewall
{: #cp_bpnofirewalbypass}

Purchasing a firewall is a start to protecting your systems, but merely purchasing a firewall does not protect you. After it is provisioned, your firewall is in **Bypass Mode** and has no rules set. To get your firewall up and running, you must create rules and activate the firewall so that it can begin blocking unwanted activity.


## Securing your environment by segmenting your application tiers
{: #cp_copmsecenv}

By segmenting your logical application tiers into physical infrastructure tiers, you can provide greater security by using access control lists (ACLs). When you segment your application tiers, one of the most critical components to consider is what traffic you allow into each tier and from where. To determine this information, think about how your application fundamentally works and what services rely on each other to provide your users with the content that they requested.

For example, consider a two tiered application that relies on a web front and database back end. For this application, ensure that port 80 and 443 (if you're using SSL) are open to the internet on your web servers. You probably also want to lock down all ports to the internet and manage your server over VPN by using the {{site.data.keyword.BluSoftlayer_full}} infrastructure private network. You probably also want to unbind the public IP address on your database server and pass all traffic to it across port 1433 (for MSSQL) or port 3306 (for {{site.data.keyword.mysql}}) from your web server. You might manage your database server over the private network just like your web server. You might also set up a software firewall on the database server to lock down all traffic from the web server to the specific database ports.

By setting up your environment in this way, preventing accessing to SSH or RDP from the internet, and disabling all internet traffic to your database, you increase security. Creating ACLs between your web layer and database layer makes it more difficult to compromise your database if your web server gets compromised.

## Scaling your environment by segmenting your application tiers
{: #cp_copmscaleenv}

A multi-tiered environment also provides ease of scalability when compared to vertical or single host architectures. You can set up a multi-tiered environment to make scaling out your application easier by allowing scaling for the services that need more resources. For example, in the previous scenario, if your web server is being over taxed, you can deploy another web server. You can then replicate site or application data and balance the load or set up round robin DNS to enable your two web servers to split your web load. Round robin DNS or balancing the load provides high availability to your environment by enabling multiple web servers to respond to incoming requests. If a single server goes down, another node is available to handle your user requests.

You can also scale out your database. For example, with a {{site.data.keyword.mysql}} database, one option is to set up another physical server and use it as a subordinate in a {{site.data.keyword.mysql}} replication setup.  You can segment all of your database writes to the master and all reads to one or more subordinates to scale the database out to support more load. This type of setup also adds a level of high availability because you can change the status of a subordinate to master. You can then and route both read and write traffic to the subordinate if your {{site.data.keyword.mysql}} master node goes down.

These ideas are just a few of many ways to secure and scale your environment. If you have any questions or concerns that are related to the best way to design your environment from a security or scalability perspective, {{site.data.keyword.BluSoftlayer_notm}} infrastructure has a Sales Engineering team that can help.
