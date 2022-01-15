# Zelf een nieuwe pagina maken
## Oefening 1
Begin met de index.html en de styles.css zoals je die in de vorige opdracht hebt gemaakt en kopieer deze over de bestanden in deze directory heen. Nu gaan we verder met wat jij tot nu toe hebt gemaakt.
We beginnen allereerst met het toevoegen van een link op jouw pagina.

Zoek op internet een pagina op die waarnaar je zou willen linken. Kopieer het adres uit de adresbalk (dus bijvoorbeeld https://www.nu.nl). Ga nu naar een van de verhaal blokjes waar je deze link wilt toevoegen.
Zo'n verhaal ziet er ongeveer als volgt uit:
```html
<div class="verhaal">
    <div class="verhaal-image"><img src="images/axe.png" height="100" /></div>
    <div class="verhaal-content">
        <h2>Verhaal titel 4</h2>
        <p>Mijn verhaal tekst komt dan hier te staan.</p>
        <p>En voor een lang verhaal kunnen dat meerdere paragrafen of plaatjes zijn.</p>
    </div>
</div>
```
Onderaan na de laatste **&lt;/p&gt;** gaan we de link toevoegen. Dit doen we door onderstaande stukje code toe te voegen:
```html
<p><a href="plak hier jouw link">zet hier tekst die je klikbaar wil maken voor de link</a></p>
```
De tag voor een link heet dus **a** en het adres waarnaar de link wijst staat in het attribuut **href**. Vervolgens wil je natuurlijk dat de link niet zomaar in de tekst staat, maar je wilt daar een 'normale' telkst neerzetten waar je op kan klikken. Dat kan dus door tussen de **a** begin en eind tag een tekst te zetten. 

Als je nu kijkt naar je pagina heb je dus in jouw verhaal een link staan naar een pagina op internet. Als je erop klikt gaat de browser naar die pagina. Maar... Nu ben je van jouw pagina weg. Je kan weer terug natuurlijk, maar soms wil je dat een link niet over jouw pagina heen gaat, maar een nieuwe tab opent. Dat kan door het toevoegen van het attribuut **target** aan de link:
```html
<a href="plak hier jouw link" target="_blank">zet hier tekst die je klikbaar wil maken voor de link</a>
```
Nu opent de link een nieuwe tab. Probeer het maar eens.

Stel je wilt dat links waar je op klikt wel op een andere tab openen, maar dat het telkens dezelfde tab moet zijn. Dat kan ook. In plaats van de waarde **_blank** geeft je dan een naam aan die tab, bijvoorbeeld **uitleg**:
```html
<a href="https://en.wikipedia.org/wiki/Minecraft" target="uitleg">Uitleg</a> of <a href="https://www.speluitleg.com/minecraft/" target="uitleg">nog meer uitleg</a>
```
Plaats deze twee links maar eens in je pagina en je zal zien dat ze allebei op dezelfde tab openen en dat jouw pagina in zijn eigen tab open blijft.

## Oefening 2
Dit was een link naar een pagina ergens op internet, maar je kan ook linken naar een andere pagina die je zelf hebt gemaakt. Dat gaan we nu doen.

We beginnen door een nieuw verhaal toe te voegen aan onze pagina, je bepaald zelf waar je deze wilt plaatsen:
``html
<div class="verhaal">
    <div class="verhaal-image"><img src="images/axe.png" height="100" /></div>
    <div class="verhaal-content">
        <h2>Verhaal titel met een link</h2>
        <p>Mijn verhaal tekst komt dan hier te staan.</p>
        <p>En bij dit verhaal gaan we een link naar een nieuwe pagina van ons maken.</p>
    </div>
</div>
```

Nu plaatsen we een link naar onze nieuwe pagina die we gaan maken. Ze net als in de vorige oefening een link na de laatste paragraaf (**&lt;/p&gt;**). Verzin hiervoor zelf een naam van de pagina en van de tekst die je hiernaar wilt laten verwijzen:

```html
<p><a href="paginanaam.html">zet hier tekst die je klikbaar wil maken voor de link</a></p>
```
Klik nu maar eens op die link. Huh, nu krijg je een foutmelding dat de pagina niet wordt gevonden?! Dat noemen ze een 404. 
Logisch, want we hebben de pagina nog niet gemaakt natuurlijk. Dat gaan we dan nu maar doen in oefening 3!

## Oefening 3
Maak nu een bestand aan met dezelfde naaam als die je in de vorige oefening hebt gebruikt om de link aan te maken, dus in het voorbeeld zou dat zijn geweest **paginanaam.html**. Maakt dat bestand aan in dezelfde directory als index.html.

OK. Nu moeten we deze nieuwe pagina gaan vullen met HTML code natuurlijk. Hmmm, dat hebben we in opdracht 1 natuurlijk gehad. Probeer nu zelf uit (of kijk terug naar opdracht 1) om een pagina te maken. Zorg ervoor dat deze de volgende elementen bevat:
* head
* body
  * h1 met de pagina titel
  * een div met daarin een paragraaf.

Sla deze pagina op en ga nu terug naar je index.html in de browser en kijk nu wat er gebeurt als je op de link klikt naar jouw nieuwe pagina. Yes, nu zie je dus de nieuwe pagina!!!!
