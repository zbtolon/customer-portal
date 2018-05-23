---

copyright:

  years: 2018

lastupdated: "2018-05-22"

---

{:shortdesc: .shortdesc}
{:codeblock: .codeblock}
{:tip: .tip}
{:screen: .screen}
{:new_window: target="_blank"}


# Setting up two-factor authentication
{: #customerportal_2fa}

Within the customer portal, external two-factor authentication (2FA) can be activated to add extra protection when you log in to the portal. This extra layer of security protects the account from unverified access, ensuring that devices, data, and account information are protected.
{:shortdesc}

If you enable 2FA in the customer portal for your existing SoftLayer account, you are required to enter your security code when you log in to the {{site.data.keyword.Bluemix_notm}} console. However, the 2FA applies only to the infrastructure resources in your {{site.data.keyword.Bluemix_notm}} account. Therefore, you might be able to do various actions to the resources in your {{site.data.keyword.Bluemix_notm}} account without completing 2FA.

2FA for your SoftLayer account is not per IBMid. It is still per account. When an IBMid is associated with multiple accounts, and you switch between accounts, you must confirm your identity every time you switch to a different account. You must confirm your identity when you switch between accounts even if the prior account and the new account are both configured with the same 2FA mechanism.

## Enabling 2FA

2FA authentication is available in two forms. Both methods of external authentication can be added per user for a small monthly fee:

* Symantec Identify Protection is the most commonly used external authentication tool, providing a dynamic security code that is used in addition to the user name and password when you access the Customer Portal.
* PhoneFactor authentication provides out-of-band authentication with a phone call, SMS, or mobile app.

 If you have a linked account, you can take advantage of the multi-factor authentication (MFA) setting by [enabling multi-factor authentication](/docs/iam/mfa.html) for your entire {{site.data.keyword.Bluemix_notm}} account.
 {: tip}

To set up 2FA, complete the following steps:

1. Access the **Users** screen in the customer portal.
2. Select **Add External Authentication** from the **Actions** menu for the user.
3. Based on the type of external authentication being ordered, complete the following steps:
    * If you choose Symantec Identity Protection, select **Symantec Identity Protection**, and then enter the user's credential ID.
    * If you choose PhoneFactor, select **PhoneFactor**.
4. Click **Continue**.
5. Complete the prompts on the screen for the **Promo Code** and **MSA Acknowledgement**.
6. Click **Order External Authentication** to complete the order. Click **Cancel** to cancel the action.

## Next steps
{: #2fanextsteps}

After you add the external authentication for a user, the next steps depend on the authentication type.
* If Symantec Identity Protection is enabled, you must add the security code that is associated with the user's Credential ID. This security code is the code that was entered in the system at the time the Symantec Identity Protection was added to the account.
* If PhoneFactor is enabled, the user must activate PhoneFactor to use this type of two-factor authentication with the account.

### Activating PhoneFactor authentication
{: #cp_actphonefacauth}

After you add PhoneFactor, you must manually activate external authentication with PhoneFactor through the customer portal. Because PhoneFactor uses manual contact, it is important to ensure that all phone numbers that are associated with the account are up-to-date always. Failure to keep contact information updated might result in being unable to access the customer portal and VPN when PhoneFactor is active. When PhoneFactor is successfully added, you receive an email to confirm that PhoneFactor has been added. After you receive the email, use the following steps to activate PhoneFactor authentication.

1. Access the customer portal by using your unique credentials.
2. Select **Account > Users** from the navigation bar.
3. Click the user name to access the associated user profile for that user.
4. Scroll to the **PhoneFactor Settings** section.

  If the PhoneFactor Settings section is not available, first verify that you received the PhoneFactor provisioning email which indicates that PhoneFactor is provisioned. If PhoneFactor is provisioned and the section is not available, create a support ticket. If PhoneFactor is not yet provisioned, wait for the email and try again.
  {: tip}

5. Select **Active** from the **Status** list.
6. Edit the **Primary Phone Number** for authentication.
  1. Click the **Edit** link.
  2. Enter the **Country Code**, **Phone Number** and **Extension**, if applicable, in the associated fields.
  3. Click **Authenticate and Save Number** to complete authentication.

    When you add a phone number for authentication, you must be by the phone. After you click **Authenticate**, the number is called and you are prompted to complete a step to authenticate the number. Phone numbers cannot be authenticated without completion of these steps.
    {: tip}

  4. To add a **Secondary Phone Number**, repeat these steps.
7. Select the **Contact Method** from the **Method** list.
8. Select a **PIN type** from the **PIN Type** list.
9. If you select **One Time** > **PIN Value**, enter the PIN in the **PIN Value** field.
10. Click **Update** to update the changes and activate PhoneFactor authentication.

After you activate PhoneFactor, authentication through PhoneFactor is required by the customer portal or VPN. After you authenticate with the user credentials, a message tells you that PhoneFactor authentication is being attempted. You, or the user you are adding, must be near the phone that is listed with PhoneFactor to complete authentication. PhoneFactor attempts to authenticate five times. After five unsuccessful authentication attempts, you are locked out for approximately one hour. You, or a user with administrative access to the account, can change the PhoneFactor authentication settings at any time.  You, or an administrator of the account, can deactivate PhoneFactor at any time.

 If you choose to set up PhoneFactor for the customer portal and your VPN login, the result is two separate 2FA login processes, one for the customer portal, and another for VPN.
 {: tip}

#### PhoneFactor authentication methods
{: #cp_phonefacauthmeths}

If you set up PhoneFactor as the authentication type, you can choose one of the following options as an authentication method:

<dl>
<dt>Phone call and standard (no pin)</dt>
<dd>With this option enabled, when you log in to the portal, you receive a phone call to the primary number enabled. When you answer the call, you are told to press the # key to complete authentication.</dd>
<dt>Phone call with pin</dt>
<dd>With this option selected, you enter a pin value in the customer portal. The pin must be 4 - 8 numbers. When you try to log in to the portal, you receive a call to the primary number listed in the portal. When you answer, you are told to enter your pin number followed by the # to complete the authentication.</dd>
<dt>SMS text and one-time pin</dt>
<dd>With this option selected, you receive a text message with a pin that you use to reply to the message. When you enter the pin that is provided, the authentication process completes and logs you in to the portal.</dd>
<dt>SMS text with one-time &amp; pin value</dt>
<dd>With this option selected, you create a pin value of 4 - 8 numbers. You then receive a text message, and you reply with the provided code and your pin number without spaces.</dd>
<dt>PhoneFactor app and standard (no pin)</dt>
<dd>Open the PhoneFactor application (Microsoft Authenticator) on your device and click <strong>Authenticate</strong>. It shows that you successfully authenticated by using PhoneFactor and logs you in to the portal.</dd>
<dt>PhoneFactor app with pin</dt>
<dd>With this option, you set a pin, 4 - 8 numbers, in the portal. You then open the PhoneFactor application (Microsoft Authenticator) on your device. Next, enter your pin that was created in the portal and click <strong>Authenticate</strong> to log in to the portal.</dd>
</dl>
