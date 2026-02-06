---
title: Waarom kan ik geen postcode en huisnummer in het buitenland gebruiken?
---
In Nederland hebben wij een vrij uniek postcodesysteem. Daarmee is het mogelijk om met alleen de postcode en het huisnummer een volledig adres aan te vullen. Bijna iedereen in Nederland kent ook zijn eigen postcode en huisnummer, daardoor is het voor webshops eenvoudig om met correcte adressen te werken.

In andere landen werkt het anders, daar is een postcode veel minder specifiek. Zo zijn postcodes in België samengesteld op basis van de sorteersector, postkantoren en uitgiftekantoren. Hierdoor bevat de postcode in België 4 cijfers. Er is grofweg één postcode per plaats, terwijl een postcode in Duitsland regiogebonden is en  bestaat uit 5 cijfers.

Onze International Autocomplete API houdt hier uiteraard rekening mee; een gebruiker kan een adres in vrijwel elk formaat opgeven (bijv 'amsterdam kalverstraat 4', 'kalverstraat 4', '2011DA 1', etc) in een enkel invoerveld. Tijdens het typen worden suggesties getoond waarmee de gebruiker direct een uniek adres selecteert, of in meer detail kan verder zoeken. Deze suggesties worden gedaan via de 'autocomplete' methode. Wanneer een suggestie gekozen wordt met de precisie van een adres, kan de 'getDetails' methode aangeroepen worden om alle gevalideerde adresdetails te verkrijgen.

Zie ook onze [technische demo](https://developer.postcode.eu/documentation/international/overview).
