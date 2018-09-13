<a id="cha:knowOis11dictaat"></a>

### Werken met variabelen in C#
Dit hoofdstuk is geschreven als een *naslagwerk*,
het is niet geschikt om uit te leren hoe je met variabelen programmeert.
#### Typen variabelen

Een variabele is een stukje geheugen waarin tijdelijk
een waarde kan worden  opgeslagen. De veelgebruikte typen variabelen zijn:

<table style="border: solid thin"><tr><th>Inhoud</th>
<th>Naam</th>
<th>Voorbeelden</th>
</tr>
<tr><td style="text-align: left">Stukje tekst</td>
<td style="text-align: left">String</td>
<td style="text-align: left">&quot;abcde&quot;</td>
</tr>
<tr><td style="text-align: left"></td>
<td style="text-align: left"></td>
<td style="text-align: left">&quot;dit is een tekst&quot;</td>
</tr>
<tr><td style="text-align: left"></td>
<td style="text-align: left"></td>
<td style="text-align: left">&quot;&quot;</td>
</tr>
<tr><td style="text-align: left"></td>
<td style="text-align: left"></td>
<td style="text-align: left">etc.</td>
</tr>
<tr><td style="text-align: left">Geheel getal</td>
<td style="text-align: left">Int</td>
<td style="text-align: left">12</td>
</tr>
<tr><td style="text-align: left"></td>
<td style="text-align: left"></td>
<td style="text-align: left">-1337</td>
</tr>
<tr><td style="text-align: left"></td>
<td style="text-align: left"></td>
<td style="text-align: left">0</td>
</tr>
<tr><td style="text-align: left"></td>
<td style="text-align: left"></td>
<td style="text-align: left">etc.</td>
</tr>
<tr><td style="text-align: left">Komma getal</td>
<td style="text-align: left">Double</td>
<td style="text-align: left">10.2</td>
</tr>
<tr><td style="text-align: left"></td>
<td style="text-align: left"></td>
<td style="text-align: left">-12.3</td>
</tr>
<tr><td style="text-align: left"></td>
<td style="text-align: left"></td>
<td style="text-align: left">5.0</td>
</tr>
<tr><td style="text-align: left"></td>
<td style="text-align: left"></td>
<td style="text-align: left">etc.</td>
</tr>
<tr><td style="text-align: left">Waar of niet waar</td>
<td style="text-align: left">Bool</td>
<td style="text-align: left">true, false</td>
</tr>
</table>


#### Variabele aanmaken (declareren)
Variabelen kunnen op verschillende manieren worden aangemaakt,
enkele voorbeelden staan hier-onder. Merk op dat:
- Je de variabele naam zelf kunt kiezen
- De regel moet worden beeindigd met een &quot;;&quot;-teken

Op verschillende manieren kunnen variabelen worden aangemaakt. Programmeer op een lege regel het type van de variabele (zie hierboven), de naam die je de variabele wil geven (deze kies je zelf) en een &quot;;&quot; teken om het programmeercommando af te sluiten.
<table style="border: solid thin"><tr><th>Voorbeeld</th>
<th>Effect</th>
</tr>
<tr><td style="text-align: left">String s;</td>
<td style="text-align: left">Variabele met de naam s wordt aangemaakt.</td>
</tr>
<tr><td style="text-align: left"></td>
<td style="text-align: left">De default waarde is &quot;&quot;.</td>
</tr>
<tr><td style="text-align: left">`int i;`</td>
<td style="text-align: left">Variabele met de naam `i` wordt aangemaakt.</td>
</tr>
<tr><td style="text-align: left"></td>
<td style="text-align: left">De default waarde is 0.</td>
</tr>
<tr><td style="text-align: left">`double d;`</td>
<td style="text-align: left">Variabele met de naam &quot;d&quot; wordt aangemaakt.</td>
</tr>
<tr><td style="text-align: left"></td>
<td style="text-align: left">De default waarde is 0.0</td>
</tr>
<tr><td style="text-align: left">Bool b;</td>
<td style="text-align: left">Variabele met de naam &quot;b&quot; wordt aangemaakt.</td>
</tr>
<tr><td style="text-align: left"></td>
<td style="text-align: left">De default waarde is false</td>
</tr>
<tr><td style="text-align: left">String mijnString;</td>
<td style="text-align: left">Variabele met de naam &quot;mijnString&quot; wordt aangemaakt.</td>
</tr>
<tr><td style="text-align: left"></td>
<td style="text-align: left">De default waarde is &quot;&quot;</td>
</tr>
<tr><td style="text-align: left">int getal;</td>
<td style="text-align: left">Variabele met de naam &quot;getal&quot; wordt aangemaakt.</td>
</tr>
<tr><td style="text-align: left"></td>
<td style="text-align: left">De default waarde is 0</td>
</tr>
<tr><td style="text-align: left">double straal;</td>
<td style="text-align: left">Variabele met de naam &quot;straal&quot; wordt aangemaakt.</td>
</tr>
<tr><td style="text-align: left"></td>
<td style="text-align: left">De default waarde is 0.0</td>
</tr>
</table>

Direct na het aanmaken heeft een `variabele` een `waarde` die we
de `default waarde` noemen. Dit kan per programmeertaal enigszins
verschillen. Daarom is het een goede gewoonte variabelen waarvan je
wil dat ze een specifieke waarde hebben deze waarde expliciet
toe te kennen.
#### Waarde aan variabele geven (toekenning of assignment)
Als een variabele eenmaal is aangemaakt kan hier een waarde aan worden toegekend.
Merk op:
- Alleen geldige waarden kunnen worden toegekend (string waarden aan strings, getallen aan int, etc.), het programmeren van een niet geldige toekenning levert een fout op waardoor het programma niet kan worden uitgevoerd.
- De variabele waaraan een waarde moet worden toegekend staat aan de linkerkant van het &quot;=&quot; teken, en de waarde welke in de variabele moet worden gestopt staat rechts van het &quot;=&quot; teken.
- De regel code wordt weer beeindigd met het &quot;;&quot;-teken.

Hier volgen enkele voorbeelden. In commentaar staat erbij uitgelegd
wat het betekent.```
String s;     // maak een variabele aan met naam "s".
s = "test";	  // Variabele met de naam "s" krijgt de waarde "test".
```

```
int i;
i = 10;	// maak variabele met naam "i" aan en geef die waarde 10
```

```
double d;
d = 1.52; //	Nieuwe variabele genaamd "d" krijgt de waarde 1,52
```

```
bool b;
b = true;	// Nieuwe variabele "b" krijgt de waarde true
```

```
String string1;
string 1 = "abc";
String string2;
string2 = string1;	// Variabele met de naam "string2" krijgt
                    // de waarde van "string1", namelijk "abc"
```

```
int getalA;
getalA = 5;
int getalB;
getalB  = getalA;	// Variabele met de naam "getalB" krijgt
                  // de waarde van "getalA", namelijk 5
```

```
double kommaGetalA;
kommaGetalA = 1.32;
double kommaGetalB;
kommaGetalB  = kommaGetalA;	// Variabele met de naam "kommaGetalB" krijgt
                            // de waarde van "kommaGetalA",
                            // namelijk 1.32
```

```
String s;
s = textBox1.Text;
    // Variabele met de naam "s" krijgt
    // als waarde de tekst die in de
    // TextBox genaamd "textBox1" staat.
```
Dit werkt omdat de `Text property` van de *TextBox* ook
van het `type` `string` is.

#### Variabele aanmaken en direct een waarde geven (declare en initialize)

Variabele met de naam *s* aanmaken en waarde &quot;test&quot; toekennen:```
String s = "test";
```

Variabele met de naam *i* aanmaken en waarde `10` toekennen:```
int i =10;
```

Variabele met de naam *d*  aanmaken en waarde `1,52` toekennen:```
double d = 1.52;
```

Variabele met de naam *b* aanmaken en waarde `true` toekennen:```
bool b = true;
```

#### Waarden omzetten naar andere typen (convert)
<p class="note">Merk op: het omzetten van een `int` of `double` naar een `String` lukt altijd, andersom lukt niet altijd en kan een foutmelding opleveren tijdens het uitvoeren van het programma (`crash` of `Unhandled Exception`).</p>
<p class="note">Een `bool` variabele kan niet worden geconverteerd.</p>
Zet de waarde van *i* om
naar een tekst met dezelfde waarde. Het
resultaat van de laatste regel is dat variabele *s* de waarde `81` krijgt.```
int i = 81;
String s;
s = Convert.ToString(i);
```

Zet de waarde van *d* om naar een tekst met dezelfde waarde.
Het resultaat van de laatste regel is dat variabele *s*
de waarde `"12.33"` krijgt:```
double d =12.33;
String s;
s = Convert.ToString(d);
```

Zet de waarde van *s* om naar een geheel getal (`integer`)
met dezelfde waarde als dat lukt (anders krijg je een foutmelding).
Het resultaat van de laatste regel is dat variabele *i* de
waarde `7` krijgt:```
int i;
String s = "7";
i  = Convert.ToInt32(s);
```

Zet de waarde van *s* om naar een *kommagetal* met
dezelfde waarde als dat lukt (anders krijg je een foutmelding).
Het resultaat van de laatste regel is dat variabele *d* de
waarde `12.129` krijgt:```
double d;
String s = "12.129";
d  = Convert.ToDouble(s);
```

#### String bewerkingen (String functies)
Hieronder worden enkele veelgebruikte String functies gedemonstreerd en kort toegelicht.
##### String’s samenvoegen
Met het `plus` teken kunnen strings aan elkaar worden geplakt.```
string tekst = "een tekst.";
string woorden = "Hier staat";
string s = woorden+tekst;
```

De `s` `variabele` krijgt hier de waarde `"Hier staateen tekst."` Merk op dat niet automatisch spaties worden toegevoegd.
```
  string tekst = "tekst.";
  string woorden = "Hier staat";
  string s = woorden + " een " + tekst;
```

	 Met het &quot;+&quot;-teken kunnen strings aan elkaar worden geplakt.
De &quot;s&quot; variabele krijgt hier de waarde &quot;Hier staat een tekst.&quot;
##### IndexOf

De plaats van een String binnen een andere String bepalen:
De *Positie* variabele krijgt de waarde `1`.
Merk op dat de positie van de eerste gevonden &quot;e&quot; in de String
wordt gevonden (waarbij vanaf `0` wordt geteld):```
string tekst = "regel tekst";
int positie = tekst.IndexOf("e");
```

Er kan ook naar meerdere letters achter elkaar gezocht worden:```
string tekst = "regel tekst";
int positie = tekst.IndexOf("tek");
```
De &quot;Positie&quot; variabele krijgt de waarde 6.
**Niet gevonden** geeft `-1`:```
string tekst = "regel tekst";
int positie = tekst.IndexOf("a");
```
De &quot;Positie&quot; variabele krijgt de waarde -1. De waarde -1 betekent dus: de String komt niet voor binnen de andere String.
##### Substring
Een stukje uit een string kopiëren:```
string tekst = "regel tekst";
string deelTekst = tekst.Substring(0, 1);
```
wat heeft als resultaat dat in deelTekst de waarde &quot;r&quot; komt te staan omdat van de oorspronkelijke tekst vanaf positie 0 precies 1 letter gekopieerd wordt.
```
string tekst = "regel tekst";
string deelTekst = tekst.Substring(6, 5);
```
Deze code heeft als resultaat dat in deelTekst de waarde &quot;tekst&quot; komt te staan omdat van de oorspronkelijke tekst vanaf positie 6 precies 5 letters gekopieerd worden.
##### Length

Aantal tekens van de String bepalen. Achter `Length` hoeven
geen haakjes openen en sluiten geplaatst te worden omdat het
een `property` (eigenschap) van de string is en niet een `method`
die je uitvoert.
```
string tekst = "regel tekst";
int lengte = tekst.Length;
```

Deze code heeft als resultaat dat in lengte de waarde `11` komt te staan omdat de tekst precies elf lang is. Merk op: dit is inclusief spaties in de tekst.
De `double quotes` om begin en einde van de String waarde aan te geven worden niet meegeteld.
```
string tekst = "";
int lengte = tekst.Length;
```

Deze code heeft als resultaat dat in *lengte* de waarde `0` komt te staan
omdat geen tekens in de string staan.
#### int en double bewerkingen (operatoren)

Onderstaande bewerkingen zijn zowel op `int` `typen` als
op `double` typen van toepassing:
```
int k;
k = 5 + 10;
```
Aan variabele *k* wordt in de laatste regel code de waarde `15` toegekend
omdat het `+`teken de waarden `5` en `10` bij elkaar optelt.
```
int i = 2;
int k;
k = i + 1;
```
Aan variabele *k* wordt in de laatste regel code de waarde 3 toegekend
omdat het `+`teken de waarden `2` en `1` bij elkaar optelt.
```
int i = -8;
int k;
k = 1 + i;
```
Aan variabele *k* wordt in de laatste regel code de waarde `-7` toegekend
omdat het `+`teken de waarden `1` en `-8` bij elkaar optelt.
```
int i = 5;
int j = 3;
int k;
k = i + j;
```
Aan variabele *k* wordt in de laatste regel code de waarde `8` toegekend
omdat het `+`teken de waarden uit *i* en *j* bij elkaar op telt.
Bij bovenstaande voorbeelden kan de operator (het `+`teken)
worden vervangen door één van de volgende mogelijkheden:<table style="border: solid thin"><tr><th>Symbool</th>
<th>Uitwerking</th>
</tr>
<tr><td style="text-align: left">+</td>
<td style="text-align: left">Optellen</td>
</tr>
<tr><td style="text-align: left">-</td>
<td style="text-align: left">Aftrekken</td>
</tr>
<tr><td style="text-align: left">*</td>
<td style="text-align: left">Vermenigvuldigen</td>
</tr>
<tr><td style="text-align: left">/</td>
<td style="text-align: left">Delen</td>
</tr>
<tr><td style="text-align: left">%</td>
<td style="text-align: left">Geeft de rest na deling. Bijvoorbeeld:</td>
</tr>
<tr><td style="text-align: left"></td>
<td style="text-align: left">7 % 5 = 2</td>
</tr>
<tr><td style="text-align: left"></td>
<td style="text-align: left">11 % 2 = 1</td>
</tr>
<tr><td style="text-align: left"></td>
<td style="text-align: left">6 % 2 = 0</td>
</tr>
</table>
 ### Werken met keuzestructuren in C#
Dit hoofdstuk is geschreven als een *naslagwerk*,
het is niet geschikt om uit te leren hoe je met variabelen programmeert.

Als een stukje code soms wel en soms niet moet worden uitgevoerd,
dan heb je een `if` of `if … else` `statement` nodig.
Moet een stukje code soms één keer en soms vaker worden herhaald,
dan heb je een `for` of `while` `statement` nodig.
#### if-statement
Deze structuur wordt gebruikt om een stukje code uit te voeren
afhankelijk van een bepaalde situatie (de `conditie` genoemd).
Algemene vorm:
```
if ([conditie])
{
  [Uit te voeren code als conditie waar is]
}
```
waarbij `conditie` is een stelling die de waarde
`true` (*waar*) of `false` (*niet waar*) heeft.
Voorbeelden van condities:<table style="border: solid thin"><tr><th>Conditie</th>
<th>Betekenis</th>
</tr>
<tr><td style="text-align: left">true</td>
<td style="text-align: left">Waar</td>
</tr>
<tr><td style="text-align: left">false</td>
<td style="text-align: left">Niet waar</td>
</tr>
<tr><td style="text-align: left">i &gt; 5</td>
<td style="text-align: left">Is i groter dan 5?</td>
</tr>
<tr><td style="text-align: left">i &lt; 7</td>
<td style="text-align: left">Is i kleiner dan 7?</td>
</tr>
<tr><td style="text-align: left">i &gt;= 1</td>
<td style="text-align: left">Is i groter of gelijk aan 1?</td>
</tr>
<tr><td style="text-align: left">i &lt;= 2</td>
<td style="text-align: left">Is i kleiner of gelijk aan 2?</td>
</tr>
<tr><td style="text-align: left">i  == 3</td>
<td style="text-align: left">Is i precies gelijk aan 3?</td>
</tr>
<tr><td style="text-align: left">i  != 3</td>
<td style="text-align: left">Is i ongelijk aan 3?</td>
</tr>
<tr><td style="text-align: left">stukjeText == &quot;abcde&quot;</td>
<td style="text-align: left">Is *stukjeText* precies gelijk aan &quot;abcde&quot;?</td>
</tr>
<tr><td style="text-align: left">stukjeText &lt; &quot;abcde&quot;</td>
<td style="text-align: left">Komt *stukjeText* eerder in het alphabet dan &quot;abcde&quot;?</td>
</tr>
<tr><td style="text-align: left">etc.</td>
<td style="text-align: left"></td>
</tr>
</table>

Verder staat *[Uit te voeren code als conditie waar is]* voor
een stukje code (dit kunnen meerdere regels code zijn)
dat moet worden uitgevoerd als de conditie `true` (*waar*) is.
Als precies één regel code moet worden uitgevoerd zou je ervoor
kunnen kiezen de accolades openen en sluiten weg te laten,
maar dit maakt de kans op bugs een stuk groter,
dus dat raden we af.
 #### if … else … statement

Een if statement kan uitgebreid worden met een &quot;else&quot; blok. Als de conditie niet &quot;waar&quot; oplevert dan wordt de code in het else blok uitgevoerd.
Algemene vorm:
```
if ([conditie])
{
[Uit te voeren code als conditie waar is]
}
else
{
 [Uit te voeren code als conditie niet waar is]
}
```

Merk op: of de conditie nu wel of niet waar is, altijd wordt één van de twee stukjes code uit-ge-voerd.
#### Voorbeelden "if …" statement en "if … else …" statement

```
if (true)
{
	TextBox1.Text = "test";
}
```

Het stukje code tussen { en } wordt altijd uitgevoerd,
dus de `Text` van de *TextBox* wordt altijd &quot;test&quot; gemaakt.
```
if (false)
{
	TextBox1.Text = "test";
}
```

Het stukje code tussen { en } wordt nooit uitgevoerd.
```
bool b = true;
if (b)
{
	TextBox1.Text = "test";
}
```

Als `b` de waarde `true` (= *waar*)
heeft wordt de `Text` in de *TextBox* &quot;test&quot;  gemaakt.
Dit is hier nu altijd het geval omdat in dit stukje code
aan variabele `b` alleen de waarde &quot;true&quot; wordt toegekend.
```
int i = 10;
if (i < 5)
{
  i  = i + 1;
}
```

Als getal `i` kleiner dan 5 is,
dan wordt bij de waarde van `i` één opgeteld,
anders gebeurt er niets.
```
TextBox1.Text = "test2";
if (TextBox1.Text !=  "test")
{
  TextBox1.Text = "test3";
}
```

Als de tekst in de textbox niet gelijk is aan &quot;test&quot; (dat is hier het geval) dan wordt de tekst van de textbox veranderd in &quot;test3&quot;.
```
if (true)
{
	TextBox1.Text = "test";
}
else
{
	TextBox1.Text = "test2";
}
```

Het stukje code tussen de eerste { en } wordt altijd uitgevoerd,
dus de `Text` van de `TextBox` wordt altijd &quot;test&quot; gemaakt.
Het stukje code tussen de tweede { en } wordt nooit uitgevoerd.
```
int i = 5;
if (i >= 10)
{
  i  = i + 1;
}
else
{
  i = i + 5;
}
```

Als getal *i* groter of gelijk aan `10` is
dan wordt bij getal *i* `1` opgeteld.
Dit is hier niet het geval, dus wordt bij *i* `5` opgeteld.
Resultaat: *i* krijgt de waarde `10`.
```
int i = 5;
if (i >= 10)
{
  i  = i + 1;
}
else
{
  i = i + 5;
  if (i >= 10)
  {
    i = 20;
  }
}
```

Als getal *i* groter of gelijk aan `10` is
dan wordt bij getal *i* `1` opgeteld.
Dit is hier niet het geval, dus wordt bij *i* `5` opgeteld.
Resultaat: *i* krijgt de waarde `10`,
vervolgens wordt gecontroleerd of `i >= 10`,
dat is nu het geval dus krijgt *i* uiteindelijk de waarde `20` toegekend.
#### while statement
Deze structuur wordt gebruikt om een stukje code uit te voe-ren
zolang aan bepaalde voorwaarden is voldaan.
Dit varieert van `0` keer de code uitvoeren tot het
in de oneindigheid aantal keer uitvoeren van de code).
Algemene vorm:```
  while ([conditie])
  {
  [Uit te voeren code zolang de conditie waar is]
  }
```

<p class="note">Na de eerste regel staat geen &quot;;&quot; teken.</p>
<p class="note">Eerst wordt gecontroleerd of aan een voorwaarde is voldaan, dan pas wordt eventueel code uitgevoerd.</p>
#### do while statement

Deze structuur wordt gebruikt om een stukje code uit te voeren. Elke keer nadat het stukje code is uitgevoerd wordt gecontroleerd of nog aan bepaalde voorwaarden is voldaan, zo ja, dan wordt de code opnieuw uitgevoerd. Het aantal keer uitvoeren van de code varieert van 1 keer de code uitvoeren tot het in de oneindigheid aantal keer uitvoeren van de code.
Algemene vorm:```
do
{
  [Uit te voeren code zolang de conditie waar is]
} while ([conditie]);
```

<p class="note">Na de laatste regel staat een &quot;;&quot; teken.</p>
<p class="note">Eerst wordt de code één keer uitgevoerd, dan pas wordt gecontroleerd of de code eventueel vaker moet worden uitgevoerd.</p> #### Voorbeelden while en do while statement

```
int i = 0;
while(i < 10)
{
	MessageBox.Show("Test");
  i = i + 1;
}
```

Variabele *i* krijgt in het begin de waarde `0`
en er wordt net zo lang doorgegaan met *MessageBoxes* weergeven
totdat *i* kleiner dan `10` is.
De code wordt dus doorlopen met achtereenvolgens
de waarden `0` , `1`, `2`, `3`, `4`, `5`, `6`, `7`, `8` en `9`.
Er worden daarom `10` *Messageboxes* getoond met de tekst `"Test"`.
```
int i = 5;
while(i > 0)
{
	MessageBox.Show("Test");
  i = i – 1;
}
```

Variabele *i* krijgt in het begin de waarde `5` en er wordt
direct gestopt als *i* de waarde `0` krijgt toegekend.
De code wordt dus doorlopen met
de waarden `5`, `4`, `3`, `2`, `1`.
Er worden daarom `5` *Messageboxes* getoond met de tekst `"Test"`.
```
int i = 10;
do
{
	MessageBox.Show("Test");
  i = i + 1;
}
while (i < 5);
```

Variabele *i* krijgt in het begin de waarde `10`,
de code wordt uitgevoerd, en vervolgens
wordt net zo lang doorgegaan met *Messageboxes* weergeven
totdat *i* kleiner dan `5` is.
De code wordt dus doorlopen met de waarde `10`.
Er wordt daarom `1` *Messagebox* getoond met de tekst `"Test"`.
#### for statement

Deze structuur wordt gebruikt om een stukje code een
vooraf bekend aantal keer uit te laten voeren.
Algemene vorm:```
for([teller variabele aanmaken]; [herhalingsconditie]; [teller variabele aanpassen])
{
  [herhaaldelijk uit te voeren code]
}
```

waarbij *[teller variabele aanmaken]*	een `variabele` met
zelf te kiezen variabelenaam wordt aangemaakt en van een waarde voorzien.
Veel gebruikte variabele namen voor een for statement zijn &quot;i&quot;, &quot;j&quot;, &quot;k&quot;
omdat deze een hele korte naam hebben, dat leest in veel gevallen prettig.
Ook &quot;index&quot;, &quot;count&quot; of &quot;teller&quot; worden vaak gebruikt.
Het type variabele is meestal int.
De waarde waarmee de teller wordt gevuld is afhankelijk van wat je
aan het programmeren bent. In veel gevallen heeft deze de waarde `0`.
Voorbeelden:```
int i = 0
```

```
int j = 100
```

Dan *[herhalingsconditie]*: deze uit te voeren code wordt
net zo lang herhaald als uit de voorwaarde de waarde `true` komt.
Hierin verwijs je naar de *teller* variabele.
Voorbeelden:```
i < 10
j > 0
```

[teller variabele aanpassen]
	Het verhogen of verlagen van de teller. Vaak wordt deze met 1 verhoogd of verlaagd, soms in grotere stappen (bijv. `10`).
Voorbeelden:
```
i = i + 1
j = j – 10
```

[herhaaldelijk uit te voeren code]
	Het stukje code (dit kunnen meerdere regels code zijn) dat moeten worden uitgevoerd zolang de herhalingsconditie &quot;true&quot; (waar) is.
Ieder `for`statement is om te zetten naar een `while` statement
dat hetzelfde doet, en andersom.
 #### Voorbeelden for statement

```
for(int i =0 ; i < 10 ; i = i + 1)
{
	MessageBox.Show("Test");
}
```

Variabele `i` krijgt in het begin de waarde 0 en er wordt direct gestopt als i de waarde 10 krijgt toegekend. De code wordt dus doorlopen met de waarden 0,1,2,3,4,5,6,7,8 en 9. Er worden daarom 10 messagebox-en getoond met de tekst &quot;Test&quot;.
```
for(int i =5;i > 0; i = i - 1)
{
	MessageBox.Show("Test");
}
```

Variabele `i` krijgt in het begin de waarde 5 en er wordt direct gestopt als i de waarde 0 krijgt toegekend. De code wordt dus doorlopen met de waarden 5,4,3,2,1. Er worden daarom 5 messagebox-en getoond met de tekst &quot;Test&quot;.
```
for(int i =0;i < 10;i++)
{
	MessageBox.Show("Test");
}
```

Hetzelfde resultaat als het eerste voorbeeld,
maar dan in een verkorte schrijfwijze:```
i = i + 1;
```
is hetzelfde als```
i++;
```

Hetzelfde resultaat als het tweede voorbeeld,
maar dan in een verkorte schrijf-wijze:```
for(int i =5;i > 0; i--)
{
	MessageBox.Show("Test");
}
```

```
i=i-1;
```
is hetzelfde als```
i--;
```


De code```
for(int i =0;i < 10; i++)
{
	MessageBox.Show("Test "+i);
}
```
heeft als resultaat dat *MessageBoxes*
verschijnen met achtereenvolgens:```
"Test 0"
"Test 1"
"Test 2"
"Test 3"
"Test 4"
"Test 5"
"Test 6"
"Test 7"
"Test 8"
"Test 9"
```

De code```
for(int i =5;i > 0; i = i - 2)
{
	MessageBox.Show("Test "+i);
}
```
laat messagebox-en verschijnen met achtereenvolgens:```
"Test 5"
"Test 3"
"Test 1"
```
en tot slot geeft```
for(int y =0;y < 2; y++)
{
  for(int x =0;x < 3; x++)
  {
    MessageBox.Show("("+x+","+y+")");
  }
}
```
als resultaat *MessageBoxes* verschijnen met:```
"(0,0)"
"(1,0)"
"(2,0)"
"(0,1)"
"(1,1)"
"(2,1)"
```





### Werken met methoden in C#
Dit hoofdstuk is geschreven als een *naslagwerk*,
het is niet geschikt om uit te leren hoe je met variabelen programmeert.

#### Algemene structuur methoden

Een methode is een stukje code dat vanuit een ander stukje code
is aan te roepen. Als een methode een waarde terug geeft
welke gebruikt gaat worden in het stukje code waar vanuit
deze is aangeroepen spreek je over een methode welke &quot;een waarde teruggeeft&quot;.
Ook kunnen aan een methode één of meer waarden worden meegegeven.
Dit worden argumenten genoemd.
#### Belangrijkste voordelen van het gebruik van methoden:
1. Overzichtelijkheid: Als alle code in één enkele event handler (bijv. *ButtonX_Click*) wordt geplaatst wordt je code al snel erg overzichtelijk.
2. Werk verdelen: Als je voordat je gaat programmeren het programmeerwerk wilt verdelen kun je de te maken code opdelen in methoden en deze met verschillende programmeurs tegelijkertijd programmeren.
3. Onderhoudbaarheid &amp; herbruikbaarheid: Als je op verschillende plaatsen in je programma hetzelfde stuk code vaker uit wilt voeren kun je vanaf de verschillende plaatsen een methode aanroepen die je maar één keer hoeft te programmeren.  Dat scheelt code en is gemakkelijker te onderhouden dan dat je code verschillende keren in je programma kopiert en plakt.

Een methode heeft de volgende structuur:
```
private [returnType] [methodeNaam]([parameters])
{
  …
  [return returnWaarde]
}
```

<dl><dt>`private`</dt>
<dd>geeft aan dat de `methode` alleen binnen het huidige bestand (lees: `Form1`) kan worden aangeroepen. Wat dit precies inhoudt is voor dit vak niet interessant, hier wordt later op teruggekomen.</dd>
<dt>[returnType]</dt>
<dd>Het type van de waarde die de methode terug geeft. Als de methode geen waarde terug geeft, is dit `void` (*niets*). Voorbeelden: `int`, `double`, `bool`, `string`, `void`.</dd>
<dt>[methodeNaam]</dt>
<dd>Zelf gekozen naam voor de methode, te vergelijken met een zelf gekozen naam voor een variabele.	Voorbeelden: *TelOp*, *ToonMelding*, *Methode1*, *Abc*.</dd>
<dt>[parameters]</dt>
<dd>Optioneel onderdeel. Hiermee wordt opgegeven welk(e) type(n) waarde(n) moet worden meegegeven aan de methode en onder welke naam deze waarde binnen de method kunnen worden gebruikt. Meerdere parameters worden gescheiden met een &quot;,&quot;-teken.	Voorbeelden: `int deler`, `int getalA`, `int getalB`, `bool isIngelogd`, `double eenKommaGetal`.</dd>
<dt>[return returnWaarde]</dt>
<dd>Met `return`&quot; gevolgd door een waarde die aan het *[returnType]* voldoet wordt een waarde teruggegeven vanuit de methode aan het stukje code dat de methode heeft aangeroepen. Als *[returnType]* `void` is hoeft er geen return worden gebruikt. Voorbeelden: `return uitkomst;`, `return 10;`, `return mijnTekst;`, `return "Hallo"+" daar!";`, `return getal > 10;`</dd>
</dl>


#### Voorbeelden Methoden

Een aantal voorbeeldmethoden:
```
    private int AddTwoNumbers(int number1, int number2)
    {
        int som;
        som = number1 + number2
        return som;
    }

    private int SquareANumber(int number)
    {
        return number * number;
    }
```

Bovenstaande methoden zijn als volgt aan te roepen:
```
	int sum = AddTwoNumbers(8765, 287);
```
of:```
	int kwadraat = SquareANumber(63);
```
of, beiden:```
	int total = SquareANumber(AddTwoNumbers(1, 2));
```

##### Tekst en uitleg (engelstalig) over methoden en parameters
Zie bijvoorbeeld
[C-sharpcorner over methods](http://www.c-sharpcorner.com/UploadFile/myoussef/CSharpMethodsP_111152005003025AM/CSharpMethodsP_1.aspx)
voor meer uitleg.
### Handige sneltoetsen en opties in Visual Studio

<p class="note">Als in een sneltoets combinatie een komma staat, dan moet eerst het deel voor de komma worden ingedrukt, dan laat je de toetsen los en druk je daarna de letter in die na de komma staat.</p>
<table style="border: solid thin"><tr><th>Sneltoets</th>
<th>Menu</th>
<th>Toelichting</th>
</tr>
<tr><td style="text-align: left">CTRL-W, X</td>
<td style="text-align: left">View → Toolbox</td>
<td style="text-align: left">Maakt het Toolbox scherm met alle</td>
</tr>
<tr><td style="text-align: left"></td>
<td style="text-align: left"></td>
<td style="text-align: left">visuele objecten zichtbaar.</td>
</tr>
<tr><td style="text-align: left">CTRL-W, P</td>
<td style="text-align: left">View → Properties</td>
<td style="text-align: left">Window	Scherm met de</td>
</tr>
<tr><td style="text-align: left"></td>
<td style="text-align: left"></td>
<td style="text-align: left">eigenschappen van visuele objecten</td>
</tr>
<tr><td style="text-align: left"></td>
<td style="text-align: left"></td>
<td style="text-align: left">tonen. Hier vind je ook de events</td>
</tr>
<tr><td style="text-align: left"></td>
<td style="text-align: left"></td>
<td style="text-align: left">van de visuele objecten.</td>
</tr>
<tr><td style="text-align: left">CTRL-W, E</td>
<td style="text-align: left">View → Error List</td>
<td style="text-align: left">Toont het scherm met de eventuele</td>
</tr>
<tr><td style="text-align: left"></td>
<td style="text-align: left"></td>
<td style="text-align: left">fouten die in je code gevonden zijn</td>
</tr>
<tr><td style="text-align: left"></td>
<td style="text-align: left"></td>
<td style="text-align: left">(ververs het scherm door je project</td>
</tr>
<tr><td style="text-align: left"></td>
<td style="text-align: left"></td>
<td style="text-align: left">opnieuw te build-en met de F6 knop,</td>
</tr>
<tr><td style="text-align: left"></td>
<td style="text-align: left"></td>
<td style="text-align: left">zie hieronder).</td>
</tr>
<tr><td style="text-align: left"></td>
<td style="text-align: left"></td>
<td style="text-align: left">Dubbelklikken op een error navigeert</td>
</tr>
<tr><td style="text-align: left"></td>
<td style="text-align: left"></td>
<td style="text-align: left">naar de plaats in je code waar de</td>
</tr>
<tr><td style="text-align: left"></td>
<td style="text-align: left"></td>
<td style="text-align: left">fout is gevonden.</td>
</tr>
<tr><td style="text-align: left"></td>
<td style="text-align: left"></td>
<td style="text-align: left">Tip: bekijk eerst de eerste fout,</td>
</tr>
<tr><td style="text-align: left"></td>
<td style="text-align: left"></td>
<td style="text-align: left">andere fouten kunnen hier een gevolg</td>
</tr>
<tr><td style="text-align: left"></td>
<td style="text-align: left"></td>
<td style="text-align: left">van zijn.</td>
</tr>
<tr><td style="text-align: left">F6</td>
<td style="text-align: left">Build → Build Solution</td>
<td style="text-align: left">Controleert je code op fouten en bouwt</td>
</tr>
<tr><td style="text-align: left"></td>
<td style="text-align: left"></td>
<td style="text-align: left">vervolgens een uitvoerbaar bestand.</td>
</tr>
<tr><td style="text-align: left">F5</td>
<td style="text-align: left">Debug → Start Debugging</td>
<td style="text-align: left">Build je project (zie F6 hierboven) als</td>
</tr>
<tr><td style="text-align: left"></td>
<td style="text-align: left"></td>
<td style="text-align: left">dat nog niet gebeurd is, en voert het</td>
</tr>
<tr><td style="text-align: left"></td>
<td style="text-align: left"></td>
<td style="text-align: left">uitvoerbaar bestand vervolgens uit.</td>
</tr>
<tr><td style="text-align: left"></td>
<td style="text-align: left"></td>
<td style="text-align: left">Dit doet hetzelfde als een klik op de knop</td>
</tr>
<tr><td style="text-align: left"></td>
<td style="text-align: left"></td>
<td style="text-align: left">met het groene pijltje (`play`knop).</td>
</tr>
<tr><td style="text-align: left">Shift-F5</td>
<td style="text-align: left"></td>
<td style="text-align: left">Stop de uitvoer van je programma. Handig</td>
</tr>
<tr><td style="text-align: left"></td>
<td style="text-align: left"></td>
<td style="text-align: left">als je programma vast loopt.</td>
</tr>
</table>


### Online C-sharp tutorials

#### MSDN tutorial
[MSDN How do I Learn C# tutorials (Engelstalig)](http://msdn.microsoft.com/en-us/vcsharp/aa336766.aspx)
Bruikbaarheid:	*
Toelichting: 	Enkele gedetailleerde walkthroughs. Aanrader als je al bekend bent met programmeren in een andere programmeertaal.
#### techzine tutorial
[Les 1: Beginnen met C# (Nederlandstalig)](http://www.techzine.nl/tutorials/358/3/c-les-1-beginnen-met-c-de-eerste-stapjes.html)
Bruikbaarheid:	****
Toelichting: 	Uitleg over het maken van een programma aan de hand van een voorbeeldprogramma dat telkens een stukje wordt uitgebreid. Het gebruik van variabelen, FOR en WHILE lus worden uitgelegd. Let op: in deze tutorial wordt een Console applicatie gemaakt, dit is iets anders dan een Form applicatie.
#### Webbrowser tutorial
[Zelf een webbrowser maken (Nederlandstalig)](http://www.sitemasters.be/tutorials/17/1/564/CSharp.NET/CSharp_Zelf_een_WebBrowser_maken)
Bruikbaarheid:	*
Toelichting: 	Tutorial waarin een webbrowser gebouwd wordt. Weinig toelichting op wat er gebeurt maar wel een leuk eindresultaat. Deze tutorial is vanaf lesweek 3 redelijk goed te maken.
#### Blackwasp tutorial
[BlackWasp](http://www.blackwasp.co.uk/)
Bruikbaarheid:	***
Toelichting: 	Verzameling tutorials en artikelen (Engelstalig).

### Online C-sharp boeken

[C# Station Tutorial (Engelstalig)](http://csharp-station.com/)
Bruikbaarheid:	***
Toelichting: 	Uitleg over de basis onderdelen van C# zoals expressies, typen, variabelen en controlestructuren. De &quot;lessons&quot; 1 t/m 5 zijn interessant voor OIS.

[C# Yellow Book (Engelstalig)](http://www.robmiles.com/c-yellow-book/Rob%20Miles%20CSharp%20Yellow%20Book%202010.pdf)
Bruikbaarheid:	**Toelichting: 	Compleet boek over programmer constructies en onderwerpen. Wellicht handig als naslagwerk, niet geschikt als leerboek voor OIS. Let op: in deze tutorial wordt uitgegaan van een Console applicatie als beginpunt, dit is iets anders dan een Form applicatie.

 ### Bruikbare technieken proftaak
#### 3d objecten
In de eerste opdracht over XNA heb je met plaatjes gewerkt en niet met 3D-modellen.
3D is mooier, echter en interessanter. Maar ook lastiger te implementeren.
Op Internet zijn aardige voorbeelden te vinden.
Probeer eerst deze uit:
[MSDN over XNA en 3D](http://msdn.microsoft.com/en-us/library/bb203897(v=xnagamestudio.31).aspx)
#### WIIMote
In de opdracht &quot;1e XNA&quot;  heb je kunnen zien dat het XNA framework
was toegevoegd aan Visual Studio 2010.
Dit is te vinden in de solution Explorer onder Reference.
![](figures/xnaframework.png "eerste XNA")

In het programma gebruikte je het keyword `using` om gebruik te maken van de mogelijkheden van het Framework.
Om een component te gebruiken in Visual Studio ga je altijd op deze manier te werk. Het XNA framework heb je geïnstalleerd en daarbij werden de referentie aan VS toegevoegd.
Net zoals het XNA framework aan Visual Studio 2010 is toegevoegd kun je een softwarecomponent toevoegen om de Wiimote te gebruiken. Deze component is te vinden op het Internet  genaamd WiiMoteLib.dll
Hiervoor is er geen installatie nodig, maar je kunt met een rechtermuisklik op reference in het menuutje kiezen voor add reference. Hierna browse je naar de juiste file.
De *Wiimote* gaat communiceren met je applicatie via *Bluetooth*. Het instellen van Bluetooth kun je ook overal op het Internet vinden. Google: Wiimote Bluetooth
Ook zijn er verschillende testprogramma’s te vinden.
#### XBOX 360
Bij de ISSD kun je ook een XBOX lenen om daar je XNA-applicatie op te draaien.
In de C#/XNA programma is een kleine aanpassing nodig om de applicatie geschikt te maken voor de XBOX.
Voer de volgende stappen uit om een game van je laptop naar de Xbox te porten:
•	Rechtermuisknop klikken op je windowsproject
•	Selecteer &quot;Create a Copy of Project for Xbox 360&quot;
Zie uitgebreider http://msdn.microsoft.com/en-us/library/bb976061.aspx
Even uitproberen. Je moet namelijk in een lan zitten, ook lid zijn van creatorclub enzo.
 ### XNA en/of gaming bronnen
Let op: XNA wordt niet meer gebruikt voor OIS. Wij gebruiken MonoGame.
Tutorials voor veelgebruikte gaming aspecten (let op: deze zijn gemaakt voor XNA 3.0 dus werken soms net iets anders)
[http://www.xnadevelopment.com/tutorials.shtml](http://www.xnadevelopment.com/tutorials.shtml)
[http://creators.xna.com](http://creators.xna.com)
[http://creators.xna.com/en-us/Academia](http://creators.xna.com/en-us/Academia)
[http://www.xbox.com/en-US/kinect](http://www.xbox.com/en-US/kinect)
[http://depts.washington.edu/cmmr/Research/XNA_Games/XNACS1WorkBook.html](http://depts.washington.edu/cmmr/Research/XNA_Games/XNACS1WorkBook.html)
[http://dxframework.org/](http://dxframework.org/)
[Game Studio Express](http://msdn2.microsoft.com/en-us/library/bb200104.aspx)
[Video Game programming](http://www.academicresourcecenter.net/curriculum/pfv.aspx?ID=6878)
[http://www.garagegames.com/products/torque/x/](http://www.garagegames.com/products/torque/x/)
[https://www.academicresourcecenter.net/curriculum/FacetMain.aspx?FT=Tag&amp;TagList=3&amp;ResultsTitle=Gaming%20and%20Graphics&amp;ShowResults=1](https://www.academicresourcecenter.net/curriculum/FacetMain.aspx?FT=Tag&TagList=3&ResultsTitle=Gaming%20and%20Graphics&ShowResults=1)
[http://www.youtube.com/watch?v=6AKgH4On65A](http://www.youtube.com/watch?v=6AKgH4On65A)
[http://www.youtube.com/watch?v=c_LrVqI6StY](http://www.youtube.com/watch?v=c_LrVqI6StY)
[http://graphics.cs.columbia.edu/projects/goblin/](http://graphics.cs.columbia.edu/projects/goblin/)
 ### XNA problemen oplossen
#### No suitable graphics card found
Het kan gebeuren dat XNA de volgende foutmelding geeft:
Dit probleem is op te lossen door de instelling &quot;de volledige  HiDef API gebruiken&quot; die standaard aan staat te veranderen in &quot;Use Reach to access a limited API set ….&quot;.  Deze instelling is te vinden bij &quot;Project Properties&quot; op het tabblad &quot;XNA Game Studio&quot;.
#### XNA programma kan niet worden uitgevoerd
Het gebruik hiervan op zogenaamde ‘N’ versies van windows 7 kan tot problemen leiden bij het gebruik van XNA. Voor meer info over ‘N’ versies van windows 7, zie: http://en.wikipedia.org/wiki/Windows_7_editions#Sub-editions
N versies van windows 7 missen Windows Media Player en de daarbij horende codecs, door EU restricties. Gevolg hiervan is dat XNA programma’s die (bijvoorbeeld) WAV bestanden bevatten niet kunnen compileren.
In plaats van een melding dat je WMP/codecs mist, krijg je bij het compileren een cryptische melding over een missende DLL die je, eenmaal gevonden, niet kunt toevoegen aan je project
Oplossing voor dit probleem: Windows Media Player downloaden en installeren, zie:
http://windows.microsoft.com/en-US/windows/downloads/windows-media-player
(Deze linkt door naar deze link: http://www.microsoft.com/downloads/en/details.aspx?FamilyID=31017ed3-166a-4c75-b90c-a6cef9b414c4)
