---
title: Current API status
---


## [status.postcode.eu](https://status.postcode.eu/)

*   Check the current status of our API's using the link above.
*   This page will contain additional up-to-date information in case of an active issue impacting users of our API. 

## PHP vulnerability - 21-10-2026

We are aware of the [PHP vulnerabilities](https://www.php.net/archive/2026.php#2026-10-20-1) that have come to light. In order to address this issue we have taken steps to mitigate potential impact on our applications.

Additionally, we have shut down our client facing web interface at account.postcode.eu. This precaution has no impact on the availability of our real-time API products.

We are monitoring the situation and will be applying security updates to our servers as soon as they come out.

#### 21-10-2026 16:20 CET

We have updated our servers to the latest PHP releases that address the vulnerabilities. Our servers are no longer vulnerable.

#### Rotating API keys

If believe your own software may have been affected by the PHP vulnerabilities, we recommend you rotate your Postcode.eu API keys in order to prevent abuse. Your keys provide access to the following:
- Account name, limit, and current usage amount
- Admin and contact email addresses
- Address API functionality

Follow these steps to rotate your keys:
- [Log in](https://account.postcode.eu) with your *administrator* user
- In the top menu, navigate to 'Manage > Credentials' ('Beheer > Credentials')
- Create new credentials using the 'Create credentials' ('Nieuwe credentials') button. Your new API key and secret will be provided via e-mail.
- Configure the new credentials in your application and confirm that your API integration works.
- You should now disable your old credentials by editing them and providing an expiration date.


## Common issues

Are you experiencing API errors even though the API is up? Below are some common issues that you might encounter.

*   Check your account status by logging in to [account.postcode.eu](https://account.postcode.eu/). Make sure there are no overdue invoices. Invoices that are left unpaid will eventually lead to a temporarily blocked account.
*   Do you have a test account? You may have run out of test requests. Log in to [account.postcode.eu](https://account.postcode.eu/) to check your account status and request a subscription.
*   If you are using a third party plugin to access our API, make sure it's licence is still valid. Contact your plugin provider to check this.


## Server locations

We use machines in the following locations:

*   Falkenstein, Germany
*   Haarlem, Netherlands
*   Schiphol-Rijk, Netherlands


## Recent incidents

* 21-10-2026: PHP vulnerabilities. Our servers have been updated to solve this issue at 16:20 CET.
* March 14th - March 18th: intermittent downtime incorrectly registered on status.postcode.eu. *There were no actual API issues during this period*. This was a monitoring error caused by a [Cloudflare issue](https://www.cloudflarestatus.com/incidents/kxvggpg7kwx5).
