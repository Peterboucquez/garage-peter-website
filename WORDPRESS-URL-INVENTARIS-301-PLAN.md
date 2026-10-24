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


## 24 oktober 2026 — geverifieerde sitemap-audit (31 WordPress-pagina's)
Bron: door Garage Peter aangeleverde `page-sitemap.xml` (31 URL's). Daarnaast zijn 173 post-URL's en 15 portfolio-URL's ontvangen; samen **219**. Dit is de sitemap-inventaris, geen garantie dat alle historische/geïndexeerde URL's erin staan. **Nog niets op productie uitvoeren.**

| Oude URL (pad) | Bestemming/actie | Prioriteit |
|---|---|---|
| `/` | `/` behouden | kritiek |
| `/password-recovery/` | Accountfunctie onderzoeken; geen publieke 301 naar homepage | onderzoek |
| `/login/` | Accountfunctie onderzoeken; toegang beveiligen | onderzoek |
| `/testlogin/` | Testfunctie; nagaan of uitschakelen/410 passend is | onderzoek |
| `/test-formulier/` | Testformulier; nagaan of uitschakelen/410 passend is | onderzoek |
| `/services/kleine-reparaties/` | `/auto-herstellingen-bredene.html` | hoog |
| `/enkele-van-onze-klanten/` | Testimonials/reviews inventariseren; bestemming bepalen | middel |
| `/autoscout/` | Externe verkoopintegratie controleren; bestemming bepalen | middel |
| `/erp-subscription/` | Functie/abonnement controleren; niet blind redirecten | onderzoek |
| `/occasiewagens/` | `/tweedehandswagens-kopen-bredene.html` na controle | hoog |
| `/submissions/` | Formulierinzendingen controleren; geen publieke 301 | onderzoek |
| `/privacy/` | **Nieuwe privacypagina vereist** | kritiek |
| `/factuurvoorwaarden-herstelling-wagens/` | **Bestaande voorwaarden inhoudelijk overnemen** | kritiek |
| `/factuurvoorwaarden-tweedehandswagens/` | **Bestaande voorwaarden inhoudelijk overnemen** | kritiek |
| `/services/` | **Nieuwe dienstenoverzichtspagina vereist** | hoog |
| `/services/verkoop-wagens-bredene/` | `/tweedehandswagens-kopen-bredene.html` na inhoudscontrole | hoog |
| `/services/aankoop-wagens-bredene/` | Aankoopdienst verifiëren; bestemming bepalen | middel |
| `/distributieriem-vervangen-bredene/` | **Nieuwe distributieriem-dienstenpagina vereist** | hoog |
| `/services/keuring-van-wagens/` | `/autokeuring-voorbereiding-bredene.html` | hoog |
| `/depannage-wagens-bredene/` | `/depannage-autopech-bredene-campings.html` | hoog |
| `/services/depannage/` | `/depannage-autopech-bredene-campings.html` | hoog |
| `/over-ons/` | **Nieuwe over-ons-pagina vereist** | hoog |
| `/autoverhuur-bredene/` | `/autoverhuur-bredene-oscar.html` | hoog |
| `/factuur-voorwaarden/` | **Bestaande voorwaarden inhoudelijk overnemen** | kritiek |
| `/auto-herstellingen-bredene/` | `/auto-herstellingen-bredene.html` | hoog |
| `/tweedehandswagens-bredene/` | `/tweedehandswagens-kopen-bredene.html` | hoog |
| `/auto-onderhoud-bredene/` | `/auto-onderhoud-herstellingen-bredene.html` | hoog |
| `/banden-bredene/` | `/banden-kopen-monteren-bredene.html` | hoog |
| `/contact/` | `/contact.html` | hoog |
| `/keuring-van-wagens-bredene/` | `/autokeuring-voorbereiding-bredene.html` | hoog |
| `/roetfilter-reinigen-motor-ontkalken-bredene/` | Eigen Garage Peter-pagina of relevante 301, met SEO-afstemming op roetfilter-specialist.be | hoog |

**Belangrijk:** privacy- en factuurvoorwaarden niet zelf verzinnen of zonder bron kopiëren. Login-/ERP-/formulier-URL's eerst technisch en qua privacy beoordelen. Het redirectplan wordt pas uitgevoerd na controle van de nieuwe bestemmingspagina's en akkoord voor lancering.
