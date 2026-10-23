# Garage Peter — WordPress URL-inventaris en 301-plan (WERKDOCUMENT)

**23 oktober 2026. Niet uitvoeren op de live WordPress-site.** Deze inventaris is voorlopig: de volledige WordPress-sitemap/API en Search Console export zijn nog niet beschikbaar. 'Gevonden' betekent publiek vastgesteld; 'controle' is slechts een vermoedelijke slug.

| Oude WordPress URL | Nieuwe bestemming | Actie | Status/opmerking |
|---|---|---|---|
| `https://garagepeter.be/` | `/` | behouden | zeker |
| `https://garagepeter.be/home/` | `/` | 301 | gevonden |
| `https://garagepeter.be/contact/` | `/contact.html` | 301 | gevonden |
| `https://garagepeter.be/over-ons/` | `/index.html#over-ons` | nog beslissen | gevonden; liever aparte over-ons pagina |
| `https://garagepeter.be/services/` | `/index.html#diensten` | nog beslissen | gevonden; liever aparte diensten-overzichtspagina |
| `https://garagepeter.be/auto-onderhoud-bredene/` | `/auto-onderhoud-herstellingen-bredene.html` | 301 | gevonden |
| `https://garagepeter.be/auto-herstellingen-bredene/` | `/auto-herstellingen-bredene.html` | 301 | gevonden |
| `https://garagepeter.be/keuring-van-wagens-bredene/` | `/autokeuring-voorbereiding-bredene.html` | 301 | gevonden |
| `https://garagepeter.be/banden-bredene/` | `/banden-kopen-monteren-bredene.html` | 301 | gevonden |
| `https://garagepeter.be/depannage-wagens-bredene/` | `/depannage-autopech-bredene-campings.html` | 301 | gevonden |
| `https://garagepeter.be/services/depannage/` | `/depannage-autopech-bredene-campings.html` | 301 | gevonden |
| `https://garagepeter.be/autoverhuur-bredene/` | `/autoverhuur-bredene-oscar.html` | 301 | gevonden |
| `https://garagepeter.be/laatste-nieuws/` | `/nieuws.html` | 301 | gevonden |
| `https://garagepeter.be/roetfilter-reinigen-motor-ontkalken-bredene/` | Nog te bepalen | review | SEO-overlap met aparte specialistensite |
| `https://garagepeter.be/afgekeurd-deeltjestest-roetfilter-reinigen/` | Nog te bepalen | review | bestaand nieuwsartikel behouden |
| `https://garagepeter.be/bmw-x1-roetfilter-motor-ontkalken-bredene/` | Nog te bepalen | review | uniek praktijkvoorbeeld; eigen artikel nodig |
| `https://garagepeter.be/garage-peter-bereikt-100-google-reviews/` | Nog te bepalen | review | nieuwsartikel |
| `https://garagepeter.be/garage-peter-steunt-blauwe-kruis-van-de-kust/` | Nog te bepalen | review | nieuwsartikel |
| `https://garagepeter.be/motor-ontkalken-en-roetfilter-reinigen-bij-garage-peter/` | Nog te bepalen | review | nieuwsartikel |
| `https://garagepeter.be/services/aankoop-wagens/` | Nog te bepalen | controle | mogelijke dienstenpagina; slug te verifiëren |
| `https://garagepeter.be/services/verkoop-wagens/` | Nog te bepalen | controle | mogelijke dienstenpagina; slug te verifiëren |
| `https://garagepeter.be/services/keuring-van-wagens/` | Nog te bepalen | controle | mogelijke dienstenpagina; slug te verifiëren |
| `https://garagepeter.be/services/kleine-reparaties/` | Nog te bepalen | controle | mogelijke dienstenpagina; slug te verifiëren |

## Nieuwsartikelen nog individueel inventariseren
- Roetfilter ontkalken en geforceerd regenereren (22/09/2026)
- Wanneer moet mijn wagen naar de keuring? Keuringscalculator (17/09/2026)
- Diesel afgekeurd voor te hoge uitstoot (13/08/2026)
- Noodloop zonder foutcode? (29/06/2026)
- Ontkalking roetfilter Ford C-Max (24/06/2026)
- Groot verlof zomer 2026 (10/06/2026)
- Peugeot Partner 1.2 PureTech olieverbruik (06/05/2026)
- Peugeot 5008 1.2 PureTech geen oliedruk (18/03/2026)
- Autoverhuur nieuwe Opel Corsa en Citroën C3 (04/03/2026)

De titels zijn zichtbaar in het huidige nieuwsarchief, maar individuele slugs moeten nog uit de WordPress-export/sitemap worden bevestigd.

## Regels voor lancering
1. Alle URL's uit Search Console, WordPress-sitemap en WordPress-export toevoegen; oude 404's uit GSC beoordelen.
2. Belangrijke nieuwsartikelen elk een eigen pagina en 301 geven; niet blind alle berichten naar /nieuws.html redirecten.
3. Een 301 stuurt naar een echte pagina, niet naar een fragment (#over-ons of #diensten). Voor die twee eerst eigen overzichtspagina's bouwen of passende 200-pagina kiezen.
4. Na akkoord serverregels voor YRServer configureren en testen op HTTP-status 301, HTTPS, www/non-www, querystrings en geen redirectketens.
5. Tot lancering noindex op de GitHub-testsite behouden; pas bij productie canonical, robots en sitemap afronden.
6. Oude WordPress-site en databank back-uppen; geen wijzigingen aan productie vóór toestemming.
