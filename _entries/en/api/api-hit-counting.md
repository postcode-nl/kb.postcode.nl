---
title: How are API hits counted for the subscription?
---
We have deliberately designed our pricing for the autocomplete International Address API so that only full lookups are invoiced. This means that all hits you perform after a keystroke, including the final getDetails call (when the result is found), are counted as 1 lookup.

For the simpler Dutch Postcode API, hits are counted per request.
