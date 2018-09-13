<table style="border: solid thin"><tr><th>Datum</th>
<td>Week 14/15</td>
</tr>
<tr><th>Versie</th>
<td>2018 - FHICT</td>
</tr>
<tr><th>Leerdoelen</th>
<td>Realisatie</td>
</tr>
<tr><th>Vereiste voorkennis</th>
<td>Classes</td>
</tr>
<tr><th>Challenge Type</th>
<td>Integrale Realisatie</td>
</tr>
</table>


### Inleiding
Voor de Grote Slakkenrace 2019 moet vanaf een leeg project met Visual Studio
een applicatie gemaakt worden om een SlakkenRace mee te kunnen houden.
1.	Maak een nieuw Windows Form Project aan.
2.	Hernoem ‘Form1’naar ‘SnailRaceForm’.
Als je dit doet door in de *Solution Explorer* de *file* te *renamen*
stelt Visual Studio voor dat ie het *Code Element* (in dit geval dus het Form)
ook hernoemt: mooi!
3.	Maak een nieuwe class Snail aan.
`Ctrl+Shift+A` (of rechtermuisknop op project in *Solution Explorer*),
een *class name*/*file name* intypen en `OK`.
4.	Zet op het Form onder elkaar 5 PictureBoxes, recht onder elkaar, gebruik voor elk het plaatje ‘snail.jpg’.
Als je het slim doet sleep je er 1 op je *Form*,
voegt er een plaatje aan toe en kopieert de *PictureBox* nog een aantal maal
(gebruik `ctrl+C` en `ctrl+V`).
5.	Voeg een button met Text ‘Race’ toe.

6.	Maak in class Snail een constructor aan met (voor nu) 2 parameters:
- int minimumSpeed
- int maximumSpeed

7.	Voeg 2 private Fields toe (ook wel member variabelen of instance variabelen genoemd):
- minimumSpeed
- maximumSpeed

8.	Class Snail moet nu een `Field` ‘pictureBox’ van het type PictureBox krijgen
(voeg hiervoor aan het begin van de file toe: using System.Windows.Forms;).
Let op: een *professional software engineer* zou het zo niet doen: Als je al een betere manier weet doe het dan op die manier!
Je mag zelf kiezen of je dit Field public of private maakt.
9.	Voeg een `Field` toe aan het Form (dus niet in een methode gedeclareerd maar er buiten) van type List&lt;Snail&gt;:```
List<Snail> snails = new List<Snail>();
```

10.	Voeg in SnailRaceForm_Load (als je deze nog niet hebt, dubbelklik dan op het Form) de volgende code toe:```
snails.Add( new Snail(2,8) );
snails.Add( new Snail(1,8) );
snails.Add( new Snail(4,6) );
snails.Add( new Snail(3,8) );
snails.Add( new Snail(3,9) );
```

11.	Verzin (en realiseer) een manier om elke snail te laten weten welke PictureBox daar bij hoort.
 
12.	Voeg nog een smalle maar hoge PictureBox toe rechts op het scherm.
13.	Als op button Race wordt geklikt glijden alle slakken om de beurt een stukje naar rechts totdat de eerste(n) tegen de muur gelopen is/zijn.
- a.	Let op: alle slakken moeten allemaal evenveel beurten krijgen.
- b.	Voeg in class Snail een methode toe ‘GlijEenStukje()’die de X-waarde aanpast en een boolean waarde retourneert: true als die slak in die beurt tegen de muur botste, en anders false.
- c.	Een MessageBox meldt achteraf de winnaar(s).
- d.	Gebruik 1 Random-object in het hele programma.
- e.	Hou met de ‘stapgrootte’ van elke slak met zijn minimum- en maximumsnelheid. Bijvoorbeeld een slak die minimum 3 en maximum 6 heeft moet per beurt een random getal tussen 3 en 6 opschuiven (Of de waarden 3 en 6 ook mogen mag je zelf bepalen).

14.	Elke winnaar krijgt er een bedrag bij. Dit bedrag kan later veranderen maar op dit moment is dat 12,25 euro. Voeg labels toe met van elke racer het bedrag dat hij tot nu toe verdiend heeft. Gebruik hiervoor string formatting.
