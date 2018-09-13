### Wat is casting?
Een voorbeeld van casting in C#```
Product product = (Product) ListBoxProducten.Items[2];
```
Uit de `Items` van een `ListBox` genaamd *ListBoxProducten*
wordt hier het item met *index* 2 uitgelezen.
De Items zijn van type *Object* maar de ontwikkelaar wéét dat alle
*items* in de *ListBox* van *type* `Product` zijn,
en wil dit item dus in een variabele van type `Product` stoppen:
dit kan door een `cast` te gebruiken: Het `(Product)` meteen rechts
van het **=**-teken is de `cast` en geeft aan dat wat er rechts van staat
behandeld moet worden als zijnde van het type `Product`.

### Waarom is casten onveilig en moet je het zo weinig mogelijk gebruiken?
Zogenaamde statisch getypeerde talen (*statically-typed languages*)
als C#, Java, C en C++ kennen allemaal `casting`.
*Statically typed* wil zoveel zeggen als:
Op het moment dat het programma wordt gecompileerd (`Compile time`)
wordt van elke waarde en variabele vastgesteld wat het type is.
Dat type kan *runtime* (tijdens het uitvoeren van het programma)
niet meer veranderen: de compiler kan hierdoor een hoop fouten opsporen
en de ontwikkelaars hierop wijzen. Ontwikkelaars gebruiken dit als een soort vangnet.
Door te gaan `casten` maak je eigen gaten in dat vangnet:
je zegt tegen de compiler: bemoei je er niet mee:
*Trust me, I know what I'm doing*.
### Meer info
https://docs.microsoft.com/en-us/dotnet/csharp/programming-guide/types/casting-and-type-conversions
