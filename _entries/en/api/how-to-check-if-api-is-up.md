---
title: How can I check if the API is up?
---

Uptime monitoring for the API is available at [status.postcode.eu](https://status.postcode.eu/).

We strongly advise against performing automated uptime checks from your own systems. Firstly, this causes unnecessary load on our servers. Secondly, you incur unnecessary costs. Furthermore, performing these types of checks is not very useful: our own systems management is already automatically notified of any issues.

What we do recommend is implementing good logging. If something goes wrong during the usual API calls, your own systems management can take quick action, for example by resolving an internal problem directly, or by contacting us if necessary.
