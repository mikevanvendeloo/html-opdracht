
## Opdracht 1
In het eerste verhaal maken we een opsomming van wapens. Die opsomming doen we met een bullet list, dus bijvoorbeeld zo:
* bijl
* zwaard
* Pijl en boog

In HTML doe je dat als volgt:
```html
<p>Hieronder de lijst van wapens die het meest gebruikt worden:</p>
<ul>
    <li>Bijl</li>
    <li>Zwaard</li>
</ul>
```
UL staat voor unordered list. Kijk maar eens wanneer je dit in je eerste verhaal onder de titel zet, wat er dan wordt getoond.

Stel we willen niet een bolletje als opsommingsteken, maar een vierkantje, dan doe je dat als volgt:
```css
ul {  list-style-type: square; }
```


Stel we willen hier een genummerd lijstje van maken, dan hoeven we alleen maar de **&lt;ul&gt;** te veranderen in **&lt;ol&gt;**. Doe het maar eens en zie hoe de lijst veranderd.

Stel je wil romeinse cijfers gebruiken als nummering, dan kan je dat doen door deze stijling toe te passen:
```css
ol {list-style-type: upper-roman;}
```

Voor beide lijsten geld dat je ook ervoor kan zorgen dat er geen teken staat, maar dat het wel een opsomming onder elkaar is. Gebruik daarvoor:
```css
ol {list-style-type: none;}
```

Voeg nu in het tweede verhaal zelf een lijst toe met daarin een opsomming van de gevaarlijkste wezens in Minecraft.

## Opdracht 2
Soms wil je een tabel toevoegen, bijvoorbeeld als je een score lijstje wil maken met het aantal kills.
In HTML kan je ook makkelijk een tabel maken, waarbij je ook een speciale code hebt voor de kop regel van een tabel en voor een afsluitende regel.
Voorbeeld:
```html
<table>
    <thead>
        <tr>
            <th>Kolom 1</th>
            <th>Kolom 2</th>
        </tr>
    </thead>
    <tbody>
        <tr>
            <td>Waarde kolom 1</td>
            <td>Waarde kolom 2</td>
        </tr>
        <tr>
            <td>Tweede waarde kolom 1</td>
            <td>Tweede waarde kolom 2</td>
        </tr>
    </tbody>
    <tfoot>
        <tr>
            <td>Totaal kolom 1</td>
            <td>Totaal kolom 2</td>
        </tr>
    </tfoot>
</table>
```

Door de apart *thead*, *tfoot* en *tbody* elementen kan er ook makkelijk stijling worden toegepast op dat deel van de tabel. Zo kan je bijvoorbeeld bij de footer een streep aan de bovenkant tonen door de volgende css toe te passen:
```css 
tfoot { border-top: 1px solid #000000}
```

Als je kijkt naar bovenstaande voorbeeld, dan zie je voor een rij altijd de tag *tr*, voor een kolom gebruik je *td*. 

Voeg nu zelf een tabel toe in verhaal 3. Je mag zelf weten wat je erin zet en over of je 2 of zelfs meer kolommen wil gebruiken.

Klaar? Voeg dan nog wat extra stijling toe zodat de regels om en om een kleutje krijgen:
```css
tr:nth-child(even) {background: #f2f2f2}
```

Kies nu zelf een kleur uit die je mooi vind passen.
Probeer ook de kop (thead) eens een achtergrond kleur te geven.


## Opdracht 3
Soms wil je een uitspraak toevoegen van iemand. Dit kan je doen door:
```html
<blockquote>I would wish you good luck, but luck won't carry you through the Nether.</blockquote>
```

Om een quote wat specialer te maken en er uit te laten springen kan je met stijling het wat attractiever maken:
```css
blockquote{
  font-size: 1.4em;
  width:60%;
  margin:50px auto;
  font-style:italic;
  color: #555555;
  padding:1.2em 30px 1.2em 75px;
  border-left:8px solid #78C0A8 ;
  line-height:1.6;
  position: relative;
  background:#EDEDED;
}

```
Met deze stijling zetten we met *border-left* een groene verticale streep ervoor, met *background* maken we de achtegrond grijs. Met de *font-style* zorgen we ervoor dat de tekst scheef komt te staan en met de *line-height* zorgen we voor wat meer ruimte tussen de regels.

Door de *margin* te zetten, zorgen we ervoor dat de kantlijn verspringt ten opzicht van de rest van het verhaal. Met *padding* wordt de tekst niet direct neergezet, maar wordt er wat ruimte omheen genomen.

Nog een mooie toevoeging is om een quote teken te gebruiken. Dit kan met speciale stijling:
```css
blockquote::before{
  font-family:Arial;
  content: "\201C";
  color:#78C0A8;
  font-size:4em;
  position: absolute;
  left: 10px;
  top:-10px;
}
```
Speciaal is hier het *content* stuk, waarmee we dus een " plaatsen.