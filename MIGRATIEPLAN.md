# Migratie Garage Peter – werkdocument

## Status
- Eerste ontwerp in GitHub. **Niet live zetten op garagepeter.be.**
- Nieuwe pagina heeft bewust `noindex,nofollow` zolang het een ontwerp is.
- Bestaande WordPress-site, boekingsfuncties en URL's blijven onaangeroerd.

## Geïnventariseerde bestaande onderdelen
- Homepage: https://garagepeter.be/
- Diensten: https://garagepeter.be/services/
- Over ons: https://garagepeter.be/over-ons/
- Contact: https://garagepeter.be/contact/
- Autoverhuur: https://garagepeter.be/autoverhuur-bredene/
- Nieuwsarchief: https://garagepeter.be/laatste-nieuws/
- Roetfilterpagina: https://garagepeter.be/roetfilter-reinigen-motor-ontkalken-bredene/
- Andere service- en nieuwspagina's nog te inventariseren.

## Nog te doen vóór omschakeling
1. Complete URL-lijst en media-inventaris maken, inclusief WordPress-exports.
2. Bestaande teksten, berichten en foto's overzetten met behoud van broninformatie en datums.
3. Huidige links naar externe tweedehandswagenwebsite, onderhoudsafspraken en Oscar boeking vaststellen.
4. Fotomateriaal, team, contactgegevens, openingsuren en mobiele weergave nakijken.
5. SEO: bestaande slugs behouden of 301-redirects voorzien, canonicals, sitemap, structured data.
6. Veiligheid en eventuele contactformulieren testen; geen klantgegevens in GitHub.
7. Nieuwe site op aparte testomgeving controleren; pas na akkoord WordPress vervangen.
8. Bij livegang noindex verwijderen, SSL en redirects testen en back-ups bewaren.

## Techniek
Statische HTML/CSS/JS via GitHub en YRServer; servercode alleen wanneer nodig. GitHub is versiebeheer, geen vervanging voor back-ups of serverbeveiliging.
