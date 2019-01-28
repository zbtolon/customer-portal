---

copyright:

  years: 1994, 2019

lastupdated: "2019-01-25"

---

{:shortdesc: .shortdesc}
{:codeblock: .codeblock}
{:tip: .tip}
{:screen: .screen}
{:new_window: target="_blank"}


# Making a payment
{: #customerportal_makepayment}

All of your {{site.data.keyword.Bluemix}} infrastructure billing details, from invoices to payment information, are securely stored in the customer portal. If your payment method changes, or your credit card is cancelled or expires, update your payment information to avoid late charges.
{:shortdesc}

## Viewing your invoice
{: #cp_viewinvoice}

On the Invoices window, each individual invoice is summarized by invoice number, date, invoice type and various monetary balances. Invoices can be any of the following types:

<dl>
<dt>New</dt>
<dd>The first invoice in a series of recurring invoices.</dd>
<dt>Recurring</dt>
<dd>An invoice for recurring charges that have been active on the account for more than one month.</dd>
<dt>One-time-charge</dt>
<dd>A one-time charge for various expenses, which might include overages.</dd>
<dt>Credit</dt>
<dd>A credit from {{site.data.keyword.BluSoftlayer_notm}} infrastructure to the account balance.</dd>
<dt>Refund</dt>
<dd>A reversal of charges, for either a one-time or recurring charge.</dd>
</dl>

You can also view a billing summary for the account, including the following information:
  * Current and estimated next balance
  * Payment method
  * Last and next recurring invoice dates

1. Click **Account** > **Billing** > **Invoices** from the menu.
2. You can either view the invoice in the customer portal or download the invoice.

If you're viewing the invoice in the customer portal, an itemized list of billing items is shown for the selected invoice. Click anywhere on the line for a billing item to view more itemized details about the charge. If you downloaded the invoice, you can view it based on your browser settings. Downloaded invoices provide both an itemized summary and itemized detailed billing for each billing item.

**Note for those outside of the US:** If you are located outside the United States, you will be using a separate tool called Invoices which is located at http://www.ibm.com/support/customer/invoices. The specific steps you will need for each country are listed at [https://www.ibm.com/support/customer/zz/en/selectcountrylang_invoices.html](https://www.ibm.com/support/customer/zz/en/selectcountrylang_invoices.html){: new_window} ![External link icon](../icons/launch-glyph.svg "External link icon"). If you have any issues, contact us at 1-866-325-0045 and ask for access to your invoice.

{: note}

## Adding a payment method
{: #cp_cpmanacctbillpay}

Each SoftLayer account is required to have a credit card on file that is automatically charged the invoice amount each month. This information must always be current to avoid late payments; you can update it at any time to ensure that the payment information is always accurate. If the credit card information on file is correct but you want to apply an alternative form of payment to the current balance, see [Managing your billing items](/docs/customer-portal/cpmanacctbillpay.html#cp_makeonetimepayment). Use the following steps to add a payment method for an account in the customer portal.

1. Click **Account** > **Billing** > **Payment Method** from the menu.
2. Enter the required billing details for the card in each field in the **Billing Address** section.
> **Note:** Click the **Use Company Information** check box to automatically complete the fields with the company information that {{site.data.keyword.BluSoftlayer_notm}} infrastructure has on file for the account.
3. Enter the credit card information in each field in the **Payment Information** section.
4. Click **Add Credit Card** to add the credit card as a monthly payment method.
5. Optionally, select **EU Supported** to ensure that the support team in Europe handles your maintenance and support issues.  For more information about this option, see [Setting the European supported option](/docs/customer-portal/cpmanuserprof.html#cp_seteusupported).

After you add the payment method, the request is processed by SoftLayer account representatives to ensure the validity of the card. Validated cards are available for use on the account within 24 hours. The status change for the payment method is emailed to the contact that was provided when the payment method was added.

## Making a one-time payment
{: #cp_makeonetimepayment}

You can make one-time payments by using either a PayPal account or a major credit card and you can make payments for either a full or partial balance. One-time payment details aren't recorded for future use and don't modify current monthly payment methods for the account.

1. Go to the Make A One Time Payment page in the customer portal.
 * From the menu: Go to **Account** > **Make a Payment**.
 * From the Invoices page: Click **Pay Balance**.
2. Enter the payment amount in the **Payment Amount** field.
3. If you're making your payment with PayPal, click **PayPal** and follow the prompts from PayPal to complete payment. No further action is required. If you're making your payment with a credit card, enter the **Card Number, Expiration and Security Code** in the appropriate fields.
4. Enter the billing information in the appropriate fields in the **Credit Card Billing Address** section.
5. Optionally, select **EU Supported** to ensure that the support team in Europe handles your maintenance and support issues.  For more information about this option, see [Setting the European supported option](/docs/customer-portal/cpmanuserprof.html#cp_seteusupported).
6. Click **Pay with Credit Card** to initiate the payment.

After you initiate the payment, the payment is processed. If issues arise with the payment, follow the prompts from either {{site.data.keyword.BluSoftlayer_notm}} infrastructure or PayPal until the issue is resolved. The payment is processed. The amount is applied, and the current balance is updated.
