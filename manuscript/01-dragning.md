# Dragning

Dragning är en av de mest grundläggande typerna av mekaniska belastningar och uppstår när en kraft verkar längs med en kropps längdaxel och drar den isär. Denna typ av belastning är vanlig i många strukturella applikationer, såsom i kablar, stänger och andra komponenter som måste motstå dragkrafter.

## Definition av Dragning

Dragning inträffar när en yttre kraft appliceras på ett material på ett sådant sätt att materialet sträcks ut. Denna kraft kallas dragkraft och resulterar i en spänning inom materialet. Spänning är en mätning av den inre kraften per ytenhet som uppstår som en följd av den applicerade belastningen.

Formeln för spänning (σ) är:

```latexmath
\sigma = \frac{F}{A}
```

där:
- \(σ\) är spänningen i N/mm² (Newton per kvadratmillimeter).
- \(F\) är den applicerade kraften i Newton (N).
- \(A\) är tvärsnittsarean av materialet i kvadratmillimeter (mm²).

## Spänningslagen om Dragning

Spänningslagen om dragning beskriver förhållandet mellan dragkraften och den resulterande spänningen i ett material. Enligt Hookes lag, inom elastiska gränser, är spänningen proportionell mot den resulterande töjningen:

```latexmath
\sigma = E \cdot \epsilon
```

där:
- \(σ\) är spänningen i N/mm².
- \(E\) är elasticitetsmodulen eller Youngs modulus i N/mm².
- \(ε\) är töjningen, enhetslös (förändringen i längd delat med ursprungslängden).


## Exempel på Beräkning av Dragspänning

Anta att vi har en stång med en tvärsnittsarea på 10 mm² och en dragkraft på 1000 N appliceras längs med stångens längdaxel. Vi kan beräkna dragspänningen enligt följande:

```latexmath
\sigma = \frac{F}{A}
```

där:
- `F = 1000 \text{N}`$
- `A = 10 \, \text{mm}^2`$

Således:

```latexmath
\sigma = \frac{1000 \, \text{N}}{10 \, \text{mm}^2} = 100 \, \text{N/mm}^2
```

Detta innebär att dragspänningen i stången är 100 N/mm².

## Hookes Lag och Elastiska Gränser

Enligt Hookes lag är töjningen (ε) proportionell mot den applicerade spänningen (σ) så länge materialet inte överskrider sin elastiska gräns. Elasticitetsmodulen (E) för materialet är en konstant som beskriver materialets styvhet.

För stål är elasticitetsmodulen typiskt omkring 210,000 N/mm². Om vi använder denna värde, kan vi beräkna töjningen (ε) som orsakas av den tidigare beräknade dragspänningen.

```latexmath
\epsilon = \frac{\sigma}{E}
```

Med \(`\sigma = 100 \, \text{N/mm}^2`$\) och \(`E = 210,000 \, \text{N/mm}^2`$\):

```latexmath
\epsilon = \frac{100 \, \text{N/mm}^2}{210,000 \, \text{N/mm}^2} ≈ 0.000476
```

Detta betyder att för varje enhet längd av stången, sker en förlängning på cirka 0.000476 enheter längd.

## Sammanfattning

Dragning är en kritisk typ av belastning som är avgörande att förstå för att designa säkra och effektiva strukturer. Genom att använda grundläggande principer som spänningsformeln och Hookes lag, kan ingenjörer beräkna hur material beter sig under dragkrafter och säkerställa att de inte överskrider sina elastiska gränser.

## Övningsuppgifter

För att säkerställa att du förstår koncepten som presenterats i detta kapitel, vänligen arbeta igenom följande övningsuppgifter. Lösningarna bör inkludera alla steg och formler som används.

### Övning 1: Beräkning av Dragspänning

En aluminiumstång med en tvärsnittsarea på 20 mm² utsätts för en dragkraft på 500 N. Beräkna dragspänningen i stången.

### Övning 2: Töjning och Förlängning

En koppartråd med en ursprunglig längd på 2 meter och en tvärsnittsarea på 1 mm² utsätts för en dragkraft på 200 N. Elasticitetsmodulen för koppar är 110,000 N/mm². Beräkna töjningen och den totala förlängningen av tråden.

### Övning 3: Materialval

Två material, stål och aluminium, används för att tillverka stänger med samma dimensioner (tvärsnittsarea och längd). Elasticitetsmodulen för stål är 210,000 N/mm² och för aluminium är den 70,000 N/mm². Om båda stängerna utsätts för samma dragkraft, vilken stång kommer att ha den största töjningen? Beräkna töjningen för båda materialen.

### Övning 4: Säkerhetsfaktor

En plaststång med en tvärsnittsarea på 5 mm² och en längd på 1 meter utsätts för en dragkraft på 50 N. Plasticitetens elasticitetsmodul är 3,000 N/mm². Om det maximalt tillåtna töjningsvärdet för plasten är 0.01, beräkna säkerhetsfaktorn för denna belastning.

### Övning 5: Spänning i en Kompositstång

En kompositstång består av två olika material: material A med en tvärsnittsarea på 8 mm² och material B med en tvärsnittsarea på 12 mm². En total dragkraft på 1000 N appliceras på kompositstången. Elasticitetsmodulen för material A är 150,000 N/mm² och för material B är 100,000 N/mm². Beräkna den totala dragspänningen i kompositstången och fördelningen av spänningen mellan de två materialen.

