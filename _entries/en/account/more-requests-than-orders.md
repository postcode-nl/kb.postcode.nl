---
title: Why do I see more requests on my API account than I have orders?
---
The number of address requests in practice never exactly matches the number of orders in a webshop. There can be several reasons for this, which depend on the plugin used or your own implementation. The most common reasons are:

*   We often see the same addresses being requested repeatedly, for example because a user enters the same address multiple times or because the address is checked again at multiple points within the webshop software. This can cause 1 order to trigger many requests. By temporarily storing a validated address (e.g., up to 1 week), you prevent the same address from being unnecessarily retrieved via our service again and again.

*   Requests with invalid postcodes or house numbers: these requests will never yield an address. Before requesting, check if the postcode is complete and in a correct format, and if the house number starts with digits. Also, ensure that an address is only checked once a user has finished typing.
