---

copyright:

  years: 1994, 2018

lastupdated: "2018-05-22"

---

{:shortdesc: .shortdesc}
{:codeblock: .codeblock}
{:tip: .tip}
{:screen: .screen}
{:new_window: target="_blank"}


# Adding users to a SoftLayer account
{: #customerportal_addusertocpacct}

One or more users can interact with the products and services that are associated with an account. If you are the master user, you can add users at any time.
{:shortdesc}

If you are managing {{site.data.keyword.BluSoftlayer_full}} infrastructure users, which SoftLayer accounts that you can manage depends on the access that is assigned to your user account. The accounts that you can manage also depend on how your account is set up. If you are the master user, or have administrative access as an account owner, you can manage other customer portal users. If your account is not set up as a master user, you can manage your user profile.

Depending on your access, you can manage either your SoftLayer account or the accounts of other users from the Users window. The Users window in the [customer portal ![External link icon](../icons/launch-glyph.svg)](https://control.softlayer.com/){:new_window} displays users who are associated with an account. The interactions that are available on the Users window vary based on your unique account permission set.
  * If you are the master user of the account, you can see all users who are associated with the account.

  If you must share the master login credentials for your account, share the credentials carefully. Your master login controls every aspect of your account; protect it carefully. To enable other users to use the customer portal, you set up individual or permission-based users. Creating persmission-based users ensures that you to have the most control over who is able to interact with certain aspects of your account.
{:tip}

  * If you have administrative access, you can see all of the users that you added. If you gave those users permissions to administer other users, you can also see any users that they added. You can also manage any user who is associated with the account, including editing access to the customer portal, changing user status, and removing users.
  * If you are not the master user of the account and you do not have administrative access, only your profile is shown. You can interact with your own account, including viewing the API key, editing VPN access, and adding external authentication.

To manage users from the {{site.data.keyword.Bluemix_notm}} console, see the [Account setup](/docs/account/adminpublic.html#signing-up-for-ibm-cloud) section and [Managing identity and access](/docs/iam/quickstart.html#getstarted). For more information about the {{site.data.keyword.Bluemix_notm}} console, see [How the {{site.data.keyword.Bluemix_notm}} console works](/docs/overview/ui.html#ui).

Different people within an organization have different roles and responsibilities, and user permission sets are not one–size-fits-all. Therefore, you can add users to the customer portal with roles to provide access to exactly what they need for their specific role. If changes are made in error or are unauthorized, you can trace them back to the user or group. Therefore, you can provide proper training or update user permission to minimize risk. Your users can then focus on their specified role within the customer portal.

Use the following steps to add a user to an account.

1. Access the customer portal by using your unique credentials.
2. Select **Account > Users** from the navigation bar.
3. Click **Add User**.
4. Complete the required fields in the **Personal Information** section. Provide the status, a user name, and the email address for customer portal communication and notifications, including the initial notification to set up a password for the account.

  Optionally, instead of entering an address for the user, you can click the **Use Default Company Information** check box to populate the company address.
  {: tip}

5. Complete the required fields in the **Log In Settings** section. Specify whether the settings can be edited by the user, if the IP address is restricted, and whether the user is required to set up and use security questions. Also, for any users that aren't using IBMid, you can set the length of time before the password expires.
**Notes:**
* If you use IBMid for authentication, update passwords in your [IBMid profiles ![External link icon](../icons/launch-glyph.svg)](https://www.ibm.com/account/profile){:new_window} by following the instructions under **Sign In**.
* Click the **Use Portal Password for VPN** check box to sync the customer portal and VPN passwords.
6. Click **Add User**.

After you create an account for a user, the user receives an email notification to finish setting up their account. The user must set a password and, optionally, create security questions if you indicated that they are required.

How users without the administrative access of a master user log in to the customer portal depends on the master user who provided the user access in their SoftLayer accounts:
  * If the master user has an IBMid to authenticate, each user that the master user creates has an IBMid.
  * If the master user has an {{site.data.keyword.BluSoftlayer_notm}} Infrastructure ID to authenticate, each user that the master user creates has an {{site.data.keyword.BluSoftlayer_notm}} Infrastructure user name. The master user and each user that the master user creates must run the migration tool to switch to an IBMid.
  * If neither of these cases apply, for IBM Business Partners for example, contact Support to determine which user ID to use.

## Setting user permissions on the account
{: #cp_setuserpermsacct}

Use the following steps to set the permissions for the user you just added.

1. Click the **Permissions** icon, indicated by a user figure with a lock.
2. Update the **User Permissions** on all tabs for the new user.
> **Note:** Select an option from the **Quick Permissions** list to view permission sets for three types of users. Click **Set Permissions** to select the permissions set, or customize the user's accessibility by selecting individual options on each tab available.
3. Click **Add Portal Permissions** to add the permissions or click **Reset Permissions** to reset permissions for the user.
4. Click the **Device Access** icon, indicated by three servers.
5. Click the device check box for each device you want the user to be able to access.
6. Click **Update Device Access** after you select the devices.

You receive an email with links and information to guide you through setting up an IBMid for authentication into this account. The steps can include creating a new IBMid if the account is using IBMid for authentication. The invitation expires in 7 days, but you can contact your administrator to resend the invitation.

For all other authentication cases, after you add the new user, the user can then log in to the customer portal at any time. Users can then work with various products and services that are associated with the account. You can deactivate the user at any time.
