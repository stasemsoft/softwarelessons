<table style="border: solid thin"><tr><th>Datum</th>
<td>Week 11/12</td>
</tr>
<tr><th>Versie</th>
<td>2018 - Marcel V, Inge</td>
</tr>
<tr><th>Leerdoelen</th>
<td>Analyse, Ontwerp, Realisatie</td>
</tr>
<tr><th>Vereiste voorkennis</th>
<td>Analyse</td>
</tr>
<tr><th>Challenge Type</th>
<td>Integrale Toepassing</td>
</tr>
</table>



Aan: Software ontwikkelgroep &quot;De Goeroes&quot;
Betreft: specificatie hotelreserveringssysteem
Beste ontwikkelaars,
Hierbij de specificaties voor het te bouwen hotelsysteem zoals afgesproken:
### Omschrijving
Hotel Reeënrust werkt nu nog met een ingewikkeld systeem van Excel bestanden
om de reserveringen bij te houden. Graag zouden ze de reserveringen
in een applicatie willen bijhouden, zodat de werknemers van de receptie
de reserveringen gemakkelijk kunnen invoeren.
Later zou een website ook prettig zijn, zodat klanten zelf
hun reservering kunnen doen, maar voor nu ligt de focus op de applicatie
voor de receptie.
Het is belangrijk dat de applicatie gebruiksvriendelijk is en de gebruiker
de juiste meldingen krijgt.
### Scenario
Een klant belt naar de receptie om een kamer te reserveren.
De receptionist(e) voert de klantgegevens in en kijkt welke kamer
voor de opgegeven periode beschikbaar is.
Als de reservering voor meer dan 4 personen is,
zullen er meerdere kamers gereserveerd moeten worden.
Verder geeft de klant per gereserveerde kamer aan
of er gebruik gemaakt wordt van het ontbijt en/of diner.
De receptioniste kan op elk gewenst moment een overzicht opvragen
van alle reserveringen in het hotel. Tevens kan zij een lijst inzien
waarin per datum staat welke kamers deelnemen aan het ontbijt of diner.
De klantgegevens worden opgeslagen in een tekstbestand.
### Requirements
- De medewerker kan klantgegevens invoeren (NAW gegevens)
- De medewerker kan een reserveringen doen. Een reservering kan alleen in de toekomst plaatsvinden.
- De medewerker kan zien welke kamers voor een bepaalde periode beschikbaar zijn.
- De klantgegevens worden opgeslagen in een tekstbestand.
- De medewerker kan een overzicht raadplegen met alle reserveringen.
- De medewerker kan van een bepaalde datum een overzicht raadplegen waarin aangegeven staat welke kamers deelnemen aan het ontbijt of diner.

### Eigenschappen van het hotel
- Er zijn 120 kamers. Kamer 13 bestaat niet.
- Alle kamers zijn geschikt voor maximaal 4 personen (dit zou in de toekomst kunnen veranderen)

### Extra
- Het zou mooi zijn als ook de reserveringen opgeslagen kunnen worden in een tekstbestand. (Hint: Hiervoor dien je gebruik te maken van “Serialization”)


Hoogachtend verblijven wij,

Dhr. Drs. P. van Trommelen
Directeur Hotel Reeënrust
![](figures/logo_hotel.png "logo hotel")
