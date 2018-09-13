<a id="cha:Enum"></a>
### Definitie van Enum
- Enumeraties of kortweg enum’s stellen je in staat items op een gestructureerde, geordende manier voor te stellen.
- Een enumeratie zorgt ervoor dat de elementen aan te spreken zijn met een naam, maar worden intern genummerd (standaard vanaf 0).
- Met een enumeratie heb je onmiddellijk de Visual Studio Intellisense ter beschikking en behoed je jezelf voor tikfouten en logische fouten.

### Voorbeelden

```
enum Dag
{
   Zondag,
   Maandag,
   Dinsdag,
   Woensdag,
   Donderdag,
   Vrijdag,
   Zaterdag
}
```


Dan is mogelijk:```
Dag d;
d = Dag.Woensdag;
```
