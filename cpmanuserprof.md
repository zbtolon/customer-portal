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


# Managing a user profile
{: #customerportal_accuserprof}

In the customer portal, a user profile contains a variety of data about the user, including contact information and the API key. It is also the location in which passwords are stored. If you have administrative access, you can change permissions and device access from the profile.
{:shortdesc}

Within the user profile, you can manage contact information and passwords, view API keys, and update permissions and device access based on your permissions.

## Editing a user profile
{: #cp_edituserprofile}

After a user profile has been created in the customer portal, you can edit it at any time. Details associated with the user profile include personal information, login settings, API access details, user notification subscriptions, and security questions. Use the following steps to edit a user profile.

1. Access the customer portal by using your unique credentials.
2. Select **Account > Users** from the navigation bar.
3. Click the user name to access the associated user profile for that user.
4. Edit the **User Profile** details as necessary. For users in accounts that use IBMid for authentication, update your email and password in your IBMid profile. See Table 1 for more information.
5. If you want to reset your password after you log in, click **Reset Password** to generate an email allowing you to change your password.
6. Click **Edit User** to submit the changes.

| Field | Definition |
|-----|----------|
| First name, Last name | First and last name of the user associated with the user profile.|
| Email Address | Preferred email address to receive notifications from {{site.data.keyword.BluSoftlayer_notm}} infrastructure regarding the account. Changing the email address changes the record in {{site.data.keyword.BluSoftlayer_notm}} infrastructure. This change does not affect the linkage to the IBMid authentication credentials. You must change the email address for the IBMid from the IBMid profile.|
| Time zone | Preferred time zone to use when displaying time-stamped data.|
| Phone, Alt phone| Preferred contact phone numbers to be used by {{site.data.keyword.BluSoftlayer_notm}} infrastructure.|
| Street address, City, Country, State/Province, ZIP/Postal code | Full address for contact to be used by {{site.data.keyword.BluSoftlayer_notm}} infrastructure.|
{: caption="Table 1. Personal information configuration settings for editing a user profile" caption-side="top"}

|Field|Definition|
|-----|----------|
| Restrict Access to IP | IP address to restrict access to when attempting to use the customer portal under the associated user profile. |
| Expire password in (only for users in accounts that do NOT use IBMid for authentication) | Amount of time in which a password should be associated with the user profile before a new password must be selected. |
| Parent user | User account that is considered the parent user of the user profile. The parent user default is the primary account ID. |
| Require security questions? | Select this check box when security questions should be required during login. If this box is selected, security questions are required for the user profile. |
| VPN Password | Password to be used for VPN access. Click the **Use Portal Password for VPN** check box to use the customer portal password to access {{site.data.keyword.BluSoftlayer_notm}} infrastructure network through VPN. |
{: caption="Table 2. Log in settings configuration settings for editing a user profile" caption-side="top"}

|Section|Field|Definition|
|-------|-----|----------|
| API Access Information | Allowed IPs | IP addresses permitted to authenticate to the API with the unique API key associated with the user profile |
| User Notification Subscriptions | Billing | Select the **Billing** check box to receive an email invoice after it has been created. |
| Security questions | Security question | When editing your profile, this is the question that you must answer to log in when security questions have been activated for your profile.
| Security answers | Answer | Case sensitive answer to the applicable security question. |
{: caption="Table 3. Other configuration settings for editing a user profile" caption-side="top"}
After you submit edits to a user profile, the changes are applied immediately. You can change the user profile again at any time by repeating the previous steps.

See [Switching to IBMid](/docs/account/softlayerlink.html#switching-to-ibmid) for more information about setting up an IBMid account.

## Editing a user's customer portal permissions
{: #cp_editusercpperm}

User permissions in the customer portal are set by the account administrator when the user is added and can be edited at any time by an authorized user. You can edit your own user profile and, if you are an administrative user, some fields of the user profiles for users that you added. Permissions are divided into five tabs: support, devices, network, services, and account. You can update the permissions for one user at a time and you must save your changes for them to become active.

Use the following steps to edit a user's customer portal permissions.

1. Access the customer portal by using your unique credentials.
2. Select **Account > Users** from the navigation bar.
3. Click the user name of the user to access the user profile.
4. Click the **Permissions** icon to access the Permissions window.

  You might get a message indicating that changes haven't been saved to the user profile. If no changes have been made to the profile, click through to discard changes and access the Permissions window.
  {: tip}

5. Select the permissions:
  * To set quick permissions, select the permission set from the **Quick Permissions** list. After you select a permission set, each permission associated with the set is displayed in orange text with an orange arrow pointing to the check box. Then click **Set Permissions** for each tab.
  * To set individual permissions, select or deselect each check box on the tabs to update the user's permissions. Click **Select All Permissions** or **Deselect All Permissions** on any tab to select or deselect all permissions at once.
6. Click **Edit Portal Permissions** to submit changes and update the user's permissions.
7. To reset the user's permissions to the original settings instead of saving them, click **Reset Permissions**. Click **Cancel** to cancel the changes and return to the Users window.

User permissions are updated immediately after you submit the changes. If permissions have been granted, the user can view or interact with the selected features. If permissions have been removed, the user can no longer view or interact with the selected features. Permissions can be updated again at any time by repeating the previous steps.

## Adding external authentication for a user
{: #cp_addextauthuser}

From the customer portal, you can activate external two-factor authentication (2FA) to add protection when you log in to the portal. This extra layer of security protects the account from unverified access, ensuring devices, data, and account information are protected. See [Setting up two-factor authentication](/docs/customer-portal/cpenable2fa.html#customerportal_2fa) for more information.


## Changing a user's status
{: #cp_changeuserstat}

Your status in the customer portal determines your accessibility to the customer portal. Status categories that you can update on the account include Active, Disabled, and VPN Only. Your status might be changed for a variety of reasons and the status can be updated at any time. Customer status categories include those that users can update and those that are updated automatically. They include:
<dl>
<dt>Active</dt>
<dd>The user has full access to the customer portal and VPN based on permissions that are set by the account administrator. This status might be manually selected or changed at any time.</dd>
<dt>Disabled</dt>
<dd>The user does not have access to any permissions or subscriptions on the account, including customer portal and VPN. If the status category is set to disabled by another user on the account, this status can be manually selected or changed at any time.</dd>
<dt>VPN Only</dt>
<dd>The user has full access to VPN connectivity, based on his or her permission set, but cannot access the customer portal. This status can be manually selected or changed at any time.</dd>
<dt>Inactive</dt>
<dd>The user has not accessed the customer portal or VPN in the last 60 days. This is a system-generated status.</dd>
<dt>cancel_pending</dt>
<dd>An administrator on the account has canceled this user and the cancellation is currently being processed. This is a system-generated status.</dd>
</dl>

Use the following steps to change a user's status in the customer portal.

1. Access the customer portal by using your unique credentials.
2. Select **Account** > **Users** from the navigation bar.
3. Select **Change User Status** from the **Actions** list.
4. From **Status** list, select the appropriate status according to the definitions in the previous list.
5. Click **Save**.

After you update a user's status, changes to customer portal accessibility align with the new status.


## Editing a user's VPN access
{: #cp_edituservpnaccess}

When a [new user is added](/docs/customer-portal/cpmanacctadduser.html#customerportal_addusertocpacct) to a customer portal account, VPN access is selected from a variety of connection methods, including SSL, PPTP, or a combination of the two. With VPN access, the private network can be accessed in its entirety or network access can be limited to one or more specific subnets. You can manage and update VPN access at any time from the Users window. Use the following steps to edit a user's VPN access.

1. Access the customer portal by using your unique credentials.
2. Select **Account** > **VPN Access** from the navigation bar.
3. From the **VPN Access** column for the user, click the current VPN access type link to display the VPN Access window.
4. From the **VPN Type** list, select a VPN method (SSL, PPTP, SSL and PPTP, or none) to assign the user.
5. Indicate how you want to manage the **Subnet Access**:
  * Select **Auto** to automatically manage subnet access
  * Select **Manual** to manually manage subnet access and then select the **Grant Access** check box for each subnet you want the user to access. Be sure to clear any check boxes for subnets that you do not want the user to access.
6. Click **Save**.

After you update a user's VPN access, their permissions are updated and the VPN Access column displays the updated VPN access method, if applicable.

### Activating or deactivating VPN access
{: #cp_pptpvpn}

You can activate PPTP VPN to form a secure tunnel to the {{site.data.keyword.BluSoftlayer_full}} infrastructure private network that uses specialized client software that runs on your desktop or dedicated device. You can use PPTP if you need to connect your entire office or if you cannot use the SSL VPN solution.

You are allotted one PPTP connection with extra connections available. You can request support to enable unlimited PPTP access, which is available at no extra charge. Use the following steps to activate or deactivate PPTP VPN access:

1. Access the customer portal by using your unique credentials.
2. Select **Account** > **VPN Access** from the menu bar.
3. From the **VPN Access** column for the user, click the current VPN access type link to display the VPN Access window.
4. From the **VPN Type** list, select a VPN method (SSL, PPTP, SSL and PPTP, or none) to assign the user.


## Selecting email notifications
{: #cp_select-email-notifications}

You can select which email notifications you want to receive from {{site.data.keyword.BluSoftlayer_notm}} infrastructure, and which you don't. By default, you receive all email notifications but you can change them at any time. To change your email notification settings, use the following steps:
1. Access the customer portal by using your unique credentials for the account that is associated with the email address that receives notifications.
2. Click **Account** > **Users** > **E-mail Preferences** from the menu bar.
3. From the list of notification types, clear any notifications that you no longer want to receive.

Your changes are saved automatically. These settings affect the emails that are sent to you, however, they do not affect the email notifications of any other users on your account.


## Setting the EU Supported option
{: #cp_seteusupported}

You can indicate that you want support exclusively from a support team that is physically located in the European Union (EU). You can select this option when you set up your account or when you update your existing account. To set the **EU Supported** option, use the following steps:
1. Access the customer portal by using your unique credentials.
2. Click **Account** > **Manage** > **Company Profile** from the menu bar.
3. Select the **EU Supported** check box.
4. Click **Request Profile Update**.

If the **EU Supported** option is not available, you might have users in your account with PPTP VPN access enabled. Disable the PPTP VPN access for all of the users in your account first to enable the **EU Supported** option. For more information, see [Activating or deactivating PPTP VPN access](/docs/customer-portal/cpmanuserprof.html#cp_pptpvpn).

For more information about implementing the **EU Supported** option when you open a support ticket, see [Requesting support for resources in the European Union](/docs/get-support/howtogetsupport.html#eusupported).
