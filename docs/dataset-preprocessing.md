# Datasets en voorbewerking
Tijdens onze eerste teamgesprekken besloten we om op zoek te gaan naar datasets die niet alleen rijk aan informatie waren, maar ook ruimte boden voor meerdere perspectieven. Uiteindelijk kozen we voor twee goed bij elkaar passende bronnen: het World Happiness Report 2015 en de Mental Health Disorders Dataset (1990–2019). Het geluksonderzoek laat zien hoe mensen hun leven ervaren op basis van factoren zoals sociale steun en vrijheid. Tegelijk geeft de mentale gezondheidsdataset inzicht in het percentage mensen dat worstelt met depressie of angst. Door beide datasets samen te brengen konden we landen vergelijken op zowel geluksniveau als mentale gezondheid.

## Opschoning
De twee gebruikte datasets hadden als bestandstype .csv. De Mental Health Disorders Dataset (1990–2019) bevatte 8 kolommen en 6420 rijen, terwijl het World Happiness Report 2015 bestond uit 10 kolommen en 158 rijen.
Op basis van de continue variabele Happiness score is een nieuwe categorische kolom Score Category aangemaakt. Deze groepeert landen in vier klassen op basis van hun geluksscore: Zeer laag (0–4), Laag (4–6), Gemiddeld (6–7.5) en Hoog (7.5–10).

Voor het analyseren van correlaties tussen geluk en mentale gezondheid zijn beide datasets gefilterd op het jaar 2019 en vervolgens samengevoegd op landniveau. Zo ontstond één gecombineerde dataset die gebruikt kon worden voor verdere visualisatie.

Tot slot zijn uitsluitend de relevante kolommen behouden, zodat de uiteindelijke dataset overzichtelijk bleef en de visualisaties helder en interpreteerbaar konden worden weergegeven.

## Beschrijving van variabelen
In termen van variabelentype en meetschaal kunnen de gebruikte variabelen in deze dataset als volgt worden geclassificeerd:

Continue / Ratio-variabelen:

 `Happiness score` (ook aangeduid als `geluksindex` of `geluksniveau`), `Depressie` (%), `Angst` (%), `Social support`

Discrete / Nominale variabelen:

 `Land`

Discrete / Intervalvariabelen:

 `Jaar`

Momenteel gebruikte variabelen zijn:

 `Happiness score`, `Depressie` (%), `Angst` (%), `Social support`, `Land`, `Jaar`


## Aggregaties
Om de relatie tussen geluk en mentale gezondheid inzichtelijk te maken, hebben we de gegevens per land samengevoegd en geaggregeerd op het jaar 2015. In dit jaar zijn zowel geluksdata als percentages van depressie en angststoornissen beschikbaar voor een groot aantal landen.

Voor verschillende visualisaties is er bovendien een selectie gemaakt van de top 15 of top 5 landen met de hoogste geluksindex. Dit helpt bij het identificeren van patronen, bijvoorbeeld in maatschappelijke steun of het gelijktijdig voorkomen van depressie en angststoornissen.