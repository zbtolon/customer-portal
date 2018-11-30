---

copyright:

  years: 1994, 2018

lastupdated: "2018-11-28"

---

{:shortdesc: .shortdesc}
{:codeblock: .codeblock}
{:tip: .tip}
{:screen: .screen}
{:new_window: target="_blank"}
{:faq: data-hd-content-type='faq'}


# FAQs
{: #bicpfaq}

## How do I retrieve my credentials for the customer portal?
{: #bicp_retcreds}
{: faq}

If you use IBMid for authentication, when you place your first order or when you're added as a user to an account, you receive an email that has a link to get you started with your IBMid. If you lose or forget your user name or password, go to your [IBMid profile ![External link icon](../icons/launch-glyph.svg)](https://www.ibm.com/account/profile){:new_window} and reset or recover the password. You're prompted to enter specific information, which might include creating answers to your security questions.

If you don't use IBMid for authentication, when you place your first order or you're added as a user to a [customer portal ![External link icon](../icons/launch-glyph.svg)](https://control.softlayer.com/){:new_window} account, you receive an email that has your user name and initial password to get started in the customer portal. Be sure to change your password after you log in for the first time by editing your user profile.

If you forget your password after you log in, use the **Forgot Password** feature that is available on the login screen of the customer portal. You're prompted to enter specific information, including a set of security questions you specified when you set up your user profile.

If you forget your user name, contact your account administrator or master user, who can retrieve your user name. If you're the administrator or master user on the account, contact Support for more assistance.

## What is the IBMid?
{: #bicp_whatisibmid}
{: faq}

New accounts require IBMid for authentication. Existing accounts continue to use the SoftLayer user name and password for authentication until you run the migration tool to switch to an IBMid. Your SoftLayer account has a master user who then has authority to add more users within that same account. 

## How do I link an existing SoftLayer account?
{: #bicp_linkbmxacct}
{: faq}

If you're the master user on your SoftLayer account, log in to the customer portal and click **Link an account** in the header. See [Linking IBMid user accounts](/docs/account/softlayerlink.html) for more information.

## Do I must be an existing {{site.data.keyword.Bluemix_notm}} user to link accounts?
{: #bicp_bmxusertolink}
{: faq}

No. You can create a new {{site.data.keyword.Bluemix_notm}} account or link an existing {{site.data.keyword.Bluemix_notm}} Lite or Pay-As-You-Go account.

## How does two-factor authentication work?
{: #bicp_2fa}
{: faq}

There's no impact to two-factor authentication (2FA) configuration at the account level. 2FA isn't per IBMid; it's still per account. When an IBMid is associated with many accounts, and you switch between accounts, you must confirm your identity every time you switch to a different account that requires 2FA. This is true even if the prior account and the new account are both configured with the same 2FA mechanism.

For more information about IBMid with 2FA, see [Multifactor authentication usage in linked accounts](/docs/account/softlayerlink.html#2fa).

## Who can link accounts?
{: #bicp_wholinkaccts}
{: faq}

Only {{site.data.keyword.BluSoftlayer_notm}} infrastructure master users can link SoftLayer and {{site.data.keyword.Bluemix_notm}} accounts. A master user's email must also be associated to the primary owner of the {{site.data.keyword.Bluemix_notm}} account being linked.

## What will I use to log in to each console?
{: #bicp_logineachport}
{: faq}

Your account billing is linked and you can easily move between your SoftLayer and {{site.data.keyword.Bluemix_notm}} accounts, but your account identities remain separate.

* If your account doesn't use IBMid for authentication, continue to use your SoftLayer ID for SoftLayer products and services, and use your IBMid for {{site.data.keyword.Bluemix_notm}} products and services.

* If your account uses IBMid for authentication, you use your IBMid to access both your SoftLayer and your {{site.data.keyword.Bluemix_notm}} accounts.

## Why do I get an error when I try to log in with my SoftLayer user name?
{: #bicp_SLloginerror}
{: faq}

After you switch to an IBMid, if you log in to the customer portal with your {{site.data.keyword.BluSoftlayer_notm}} infrastructure user name, the "Invalid login credentials provided" error is displayed. After you switch to an IBMid, you can no longer log in to the customer portal with your {{site.data.keyword.BluSoftlayer_notm}} infrastructure user name. You must click **Login with IBMid** in the Account Login dialog.

## Why do I get an error when I try to log in with my IBMid?
{: #bicp_IBMidloginerror}
{: faq}

When you log in with your IBMid, the "We didn't recognize this IBMid or email" error is displayed. Make sure that you enter a fully qualified email address. Also, make sure that you aren't using your {{site.data.keyword.BluSoftlayer_notm}} infrastructure user name.

## Can {{site.data.keyword.BluSoftlayer_notm}} infrastructure team members access my linked account?
{: #bicp_linkgiveteamaccess}
{: faq}

You must invite them to {{site.data.keyword.Bluemix_notm}}. In the {{site.data.keyword.Bluemix_notm}} console, click **Manage** > **Account** > **Users**. After you select a resource group, you can add {{site.data.keyword.BluSoftlayer_notm}} infrastructure team members. You might have to log in to the customer portal before you can send invitations. {{site.data.keyword.Bluemix_notm}} gets the list of {{site.data.keyword.BluSoftlayer_notm}} infrastructure users, and then you can select which users to invite to the {{site.data.keyword.Bluemix_notm}} account.

## Where's my email to complete the switch to IBMid?
{: #bicp_ibmidswitchemail}
{: faq}

If you followed the wizard to switch to IBMid and haven't received the email, it can take from minutes to hours for the email with your registration code to be sent to you. You can go back to the **Edit User Profile** page in the customer portal, and click **Resend Email** to try again.

## Will I have full root access to my account?
{: #bicp_fullrootaccaccess}
{: faq}

Master users, and those with administrator permissions, have full root access to accounts on the customer portal and API. Users without administrator permissions have accessibility that is controlled by those with admin roles. These permissions can be updated by administrators from the customer portal by [editing a user profile](/docs/customer-portal/cpmanuserprof.html#cp_edituserprofile). Without administrator permissions, you can edit your user profile in the customer portal by clicking your user name on the top panel.

## Can I link an {{site.data.keyword.Bluemix_notm}} Subscription account?
{: #bicp_linkbmxsubacct}
{: faq}

All linked accounts in {{site.data.keyword.Bluemix_notm}} must be Lite or Pay-As-You-Go accounts. 

## How do I unlink my account?
{: #bicp_unlinkacct}
{: faq}

After accounts are linked, they can't be unlinked.


## What is my company profile and where can I find it?
{: #bicp_whatfindcompprof}
{: faq}

The company profile is the information that is submitted at the time the account is created and includes a primary contact for your company, along with the company name, address, and phone number. This information is used for various reasons and should be kept current always. To view the company profile for your account or to request changes, see [Updating your company profile](/docs/customer-portal/cpmanacctcompprofcont.html#cp_updcompprof).

## Where do I find my device and software passwords?
{: #bicp_devswpw}
{: faq}

Device and software passwords are stored in two locations within the customer portal. To retrieve device credentials, including the root or admin user name and password for both {{site.data.keyword.baremetal_short}} and {{site.data.keyword.virtualmachinesshort}}, see [Interact with a Device in the Snapshot View](/docs/vsi/vsi_interact_device_snapshot_view.html). To quickly view and retrieve software credentials that are manually tracked by using the customer portal, see [Managing device access](/docs/vsi/vsi_device_access.html).

## How do I keep my web data in sync?
{: #bicp_webdatasync}
{: faq}

Though you're responsible for maintaining data consistency between real servers, {{site.data.keyword.BluSoftlayer_full}} provides a private network that you can use to synchronize without incurring usage charges.

## What is the Event Management System?
{: #bicp_whatisems}
{: faq}

The Event Management System is a toolset that optimizes the way {{site.data.keyword.BluSoftlayer_full}} shares information with users about unplanned infrastructure issues and upcoming planned maintenance events. It uses targeted, subscription-based email alerts for these incidents to share the type of event that occurred. It provides subscribed users with details about the overall impact of the event and a current status of the unplanned incident in progress (UIP).

## Can I cancel a device?
{: #bicp_candev}
{: faq}

You can cancel a device at any time through the customer portal. See [Cancel a Device](/docs/vsi/vsi_managing.html) for more information about completing a cancellation request.
