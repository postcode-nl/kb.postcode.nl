---
title: Why can't I use a postcode and house number abroad?
---
In the Netherlands, we have a rather unique postcode system. This makes it possible to complete a full address with just the postcode and house number. Almost everyone in the Netherlands also knows their own postcode and house number, making it easy for webshops to work with correct addresses.

In other countries, it works differently; there, a postcode is much less specific. For example, postcodes in Belgium are composed based on the sorting sector, post offices, and distribution offices. As a result, the postcode in Belgium consists of 4 digits. There is roughly one postcode per town, while a postcode in Germany is region-specific and consists of 5 digits.

Our International Autocomplete API naturally takes this into account; a user can specify an address in almost any format (e.g., 'amsterdam kalverstraat 4', 'kalverstraat 4', '2011DA 1', etc.) in a single input field. Suggestions are shown while typing, with which the user immediately selects a unique address or can search further in more detail. These suggestions are made via the 'autocomplete' method. When a suggestion is chosen with the precision of an address, the 'getDetails' method can be called to obtain all validated address details.

See also our [technical demo](https://developer.postcode.eu/documentation/international/overview).
