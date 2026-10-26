# Svenska vägmärken för GIS och ArcGIS Pro

Detta repository innehåller svenska vägmärken i olika filformat, framtagna från EPS- och SVG-filer publicerade av Transportstyrelsen.

Syftet är att göra symbolerna enklare att använda i GIS, kartproduktion och framför allt Esri ArcGIS Pro.

## Innehåll

Repositoryt innehåller vägmärken i följande format:

- **SVG** – vektorgrafik
- **EPS** – originalformat från Transportstyrelsen
- **PDF** – konverterade vektorfiler
- **PNG** – rasterbilder
- **STYLX** – ArcGIS Pro Style-fil med vägmärkessymboler

Exempel på katalogstruktur:

```text
eps/
svg/
pdf/
png/
stylx/
```

## ArcGIS Pro

`.stylx`-filen är skapad för användning i Esri ArcGIS Pro.

Symbolerna kan användas för att symbolisera GIS-data med svenska vägmärken. Symbolnamnen baseras på vägmärkenas beteckningar.

Observera att symbolnamnen i STYLX-filen är skrivna med gemener. Om ett attributfält i exempelvis ett GIS-lager innehåller koder med versaler kan dessa därför behöva normaliseras vid matchning, exempelvis med ett Arcade-uttryck:

```arcade
Lower($feature.skyltkod)
```

Exempel:

```text
GIS-data: C31
Symbol:   c31
```

## Källa

Grundmaterialet (EPS och SVG) kommer från Transportstyrelsen och föreställer de officiella svenska vägmärkena.

[Transportstyrelsens webbplats](https://www.transportstyrelsen.se/)

De PDF-, PNG- och STYLX-filer som finns i detta repository har skapats genom bearbetning och konvertering av detta material.

## Användning och rättigheter

Kontrollera Transportstyrelsens aktuella villkor för användning av vägmärkesbilderna innan materialet återanvänds eller distribueras.

Detta repository gör inte anspråk på upphovsrätt till Transportstyrelsens ursprungliga vägmärken eller originalfiler.

De konverterade filerna har skapats för att göra materialet mer lättillgängligt för användning i GIS och andra tekniska system.

## Observera

Repositoryt är inte en officiell publikation från Transportstyrelsen.

Filerna tillhandahålls som ett praktiskt hjälpmedel för GIS, kartografi och visualisering. För juridiskt eller normerande bruk bör information alltid verifieras mot Transportstyrelsens aktuella officiella material.

## Bidrag

Felrapporter, förbättringar och kompletteringar är välkomna via GitHub Issues eller Pull Requests.
