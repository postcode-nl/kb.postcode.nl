---
title: Why Google Maps is not always suitable for address validation in Shopify
---

Shopify uses services such as Google Autocomplete by default to help customers enter their addresses. While this makes address entry easier, an address suggestion does not automatically mean that the address actually exists or is still valid.

## The problem with outdated addresses in Google Maps

Google Maps may contain addresses that have changed or no longer exist. For example, a building may have been demolished, new homes may have been built, or a street name or house number may have changed.

When these outdated addresses still appear as suggestions, customers may select an address that is no longer valid. This can result in incorrectly addressed parcels, failed deliveries, returns, and unnecessary additional costs.

Two real-world examples demonstrate why up-to-date address data matters.

# Real-world examples

## Netherlands: Example 1 — demolished building

### Welgelegen 6, Almelo

The address Welgelegen 6 in Almelo ceased to exist on 6 January 2025. The original building was demolished, and new homes with addresses on Ter Kleef were built at this location.

However, in September 2026, the old address could still be found in Google Maps. This meant that users could still select an address that had not existed for quite some time.

[Old address in Google Maps](https://www.google.com/maps/place/Welgelegen+6,+7608+JZ+Almelo/)

[Current registration in the BAG](https://bagviewer.kadaster.nl/?searchQuery=almelo+ter+kleef&objectId=0141300000001069)

## Netherlands: Example 2 — changed house number

### Bredeweg 182, Cortelande

On 5 January 2026, the address Bredeweg 182 was removed from the Dutch Key Register of Addresses and Buildings (BAG) and changed to Bredeweg 1.

In September 2026, Google Maps displayed both the new and the old address. As a result, users could still select the outdated house number.

[Old address in Google Maps](https://www.google.com/maps/place/Bredeweg+182,+2761+KC+Cortelande/)

[Current registration in the BAG](https://bagviewer.kadaster.nl/?searchQuery=bredeweg&objectId=1892010000679428)

These examples are based on discrepancies identified in September 2026. The information in Google Maps may have been updated since then.

## Germany: Example 1 — existing address missing

### Gustel-Eger-Weg 1, 14513 Teltow

Added in September 2026. This address is not known in Google Maps, where the entire area shares the address "Lichterfelder Allee 45, 14513 Teltow".

[Google Maps of the area](https://www.google.com/maps/place/Teltow,+Germany/@52.4024382,13.2759742,16.67z/data=!4m6!3m5!1s0x47a85b9cc55bbcf1:0x51197605115bce47!8m2!3d52.3975008!4d13.2752586!16zL20vMGRtbDI2?entry=ttu&g_ep=EgoyMDI2MDkyMS4wIKXMDSoASAFQAw%3D%3D)

[OpenstreetMap area shows new streets](https://www.openstreetmap.org/search?query=Gustel-Eger-Weg%091%0914513%09Teltow&zoom=19&minlon=7.544479966163636&minlat=50.94182460899971&maxlon=7.548149228096009&maxlat=50.942715274960186#map=16/52.40279/13.28060)

[Deutsche Post PLZ search API answer](https://www.postdirekt.de/plzsuche-service/streetcodes?postal_code=&city=Teltow&district=&street=Gustel-Eger-Weg)

## Germany: Example 2 — address shouldn't exist

### Schulstr. 1, 66917 Wallhalben

This address building was renovated somewhat recently, and now has the number 3 as of September 2026. However Google Maps still returns it as existing and as number 1.

[Google Maps of the area](https://www.google.com/maps/@49.3161986,7.5220783,3a,75y,153.9h,72.98t/data=!3m7!1e1!3m5!1sjqsniezZPI2dhN485pzZXQ!2e0!6shttps:%2F%2Fstreetviewpixels-pa.googleapis.com%2Fv1%2Fthumbnail%3Fcb_client%3Dmaps_sv.tactile%26w%3D900%26h%3D600%26pitch%3D17.024377364286607%26panoid%3DjqsniezZPI2dhN485pzZXQ%26yaw%3D153.90228507390293!7i16384!8i8192?entry=ttu&g_ep=EgoyMDI2MDkyMi4wIKXMDSoASAFQAw%3D%3D)

[OpenstreetMap shows the new number](https://www.openstreetmap.org/query?lat=49.316097&lon=7.522167)

## How does Postcode.eu prevent these problems?

Postcode.eu uses government registers and other official address sources, such as national land registries and postal organisations. For Dutch addresses, we use the BAG, among other sources.

By keeping our address data up to date and frequently incorporating the latest changes from official sources, we can provide a high level of accuracy. This helps prevent outdated or incorrect addresses from entering your webshop or administrative systems.

For Dutch addresses, we offer our trusted Dutch Postcode API. This allows customers to easily complete their address by entering just their postcode and house number.

With our Address Autocomplete API, customers can select up-to-date addresses as they type. Our Address Validate API can also check existing or manually entered addresses and correct them where possible.

## Up-to-date address data for international addresses

Do you sell internationally? Then it is equally important to ensure that customers provide an existing and up-to-date delivery address.

Postcode.eu provides reliable address data for 14 European countries: the Netherlands, Belgium, Germany, France, Spain, Italy, Austria, Luxembourg, Denmark, Finland, Norway, Sweden, Switzerland, and the United Kingdom.

For these countries, we exclusively use official address sources, such as national government registers and postal organisations. With a single API and one subscription, you can autocomplete and validate addresses across all supported countries.

This helps prevent failed deliveries and unnecessary returns, including for international orders.

[Explore all supported countries and our International Address API](https://www.postcode.eu/products/address-api/international)

## Up-to-date address validation for your Shopify store

The [InStijl Postcode Check app](https://apps.shopify.com/postcode-check) is available for Shopify. This integration works with our Address API and automatically validates addresses associated with orders. Incorrect addresses can be corrected where possible using our up-to-date address data.

The app also supports international address validation and offers a checkout integration for Shopify Plus. To use the integration, you need a subscription to our API and a separate subscription to the app. App support is provided by InStijl.

[Explore all available integrations](https://www.postcode.eu/products/address-api/implementation)

Please note: Address autocomplete and address validation are not the same thing. Its standard address autocomplete functionality, including suggestions provided by Google, does not in itself guarantee that a suggested address still exists.
