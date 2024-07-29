# Dragning

**Dragning** är en grundläggande mekanisk belastning som uppstår när en kraft verkar längs en kropps längdaxel och drar den isär. Denna typ av belastning är vanlig i många strukturella applikationer, såsom kablar, stänger och andra komponenter som måste motstå dragkrafter.

## Definition av Dragning

Dragning inträffar när en yttre kraft appliceras på ett material så att materialet sträcks ut. Denna kraft kallas **dragkraft** och resulterar i en **spänning** inom materialet. Spänning mäter den inre kraften per ytenhet som uppstår på grund av den applicerade belastningen.

Enheten för kraft är Newton (N). En Newton definieras som den kraft som krävs för att accelerera ett föremål med en massa på ett kilogram med en hastighet av en meter per sekundkvadrat.

Formeln för spänning `σ` är:

```latexmath
\sigma = \frac{F}{A}
```

där:
- \(`σ`\)$ är spänningen i N/mm²
- \(`F`$\) är den applicerade kraften i Newton (N)
- \(`A`$\) är tvärsnittsarean av materialet i kvadratmillimeter (mm²)

## Spänningslagen om Dragning

Spänningslagen om dragning beskriver förhållandet mellan dragkraften och den resulterande spänningen i ett material. Enligt **Hookes lag** är spänningen proportionell mot den resulterande **töjningen** inom materialets elastiska gränser:

```latexmath
\sigma = E \cdot \epsilon
```

där:
- \(`σ`$\) är spänningen i N/mm²
- \(`E`$\) är elasticitetsmodulen eller Youngs modulus i N/mm²
- \(`ε`$\) är töjningen, enhetslös

## Exempel på Beräkning av Dragspänning

Anta att vi har en stång med en tvärsnittsarea på 10 mm² och en dragkraft på 1000 N applicerad längs stångens längdaxel. Vi kan beräkna dragspänningen enligt följande:

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

Enligt Hookes lag är töjningen `ε` proportionell mot den applicerade spänningen `σ` så länge materialet inte överskrider sin elastiska gräns. **Elasticitetsmodulen** `E` för materialet beskriver materialets styvhet.

För stål är elasticitetsmodulen typiskt omkring 210 000 N/mm². Om vi använder detta värde, kan vi beräkna töjningen `ε` som orsakas av den tidigare beräknade dragspänningen.

```latexmath
\epsilon = \frac{\sigma}{E}
```

Med `\sigma = 100 \, \text{N/mm}^2`$ och `E = 210 000 \, \text{N/mm}^2`$:

```latexmath
\epsilon = \frac{100 \, \text{N/mm}^2}{210 000 \, \text{N/mm}^2} \approx 0.000476
```

Detta betyder att för varje meter av stången, sker en förlängning på cirka 0.000476 meter (eller 0.476 millimeter).

## Sammanfattning

Dragning är en kritisk typ av belastning som är avgörande att förstå för att designa säkra och effektiva strukturer. Genom att använda grundläggande principer som spänningsformeln och Hookes lag, kan ingenjörer beräkna hur material beter sig under dragkrafter och säkerställa att de inte överskrider sina elastiska gränser.

## Nyckelord

- **Dragning**: En kraft som verkar längs en kropps längdaxel och sträcker den isär.
- **Spänning**: Den inre kraften per ytenhet som uppstår på grund av en applicerad belastning.
- **Dragkraft**: Den yttre kraft som appliceras på ett material och sträcker det.
- **Elasticitetsmodul**: En konstant som beskriver materialets styvhet och förhållandet mellan spänning och töjning.
- **Töjning**: Förändringen i längd delat med ursprungslängden av ett material under belastning.
- **Hookes lag**: En lag som beskriver att spänningen är proportionell mot töjningen inom ett materials elastiska gränser.

## Övningsuppgifter

För att säkerställa att du förstår koncepten som presenterats i detta kapitel, vänligen arbeta igenom följande övningsuppgifter. Lösningarna bör inkludera alla steg och formler som används.

### Övning 1: Beräkning av Dragspänning

En aluminiumstång med en tvärsnittsarea på 20 mm² utsätts för en dragkraft på 500 N. Beräkna dragspänningen i stången.

**Lösning:**

```latexmath
\sigma = \frac{F}{A}
```

där:
- `F = 500 \text{N}`$
- `A = 20 \, \text{mm}^2`$

```latexmath
\sigma = \frac{500 \, \text{N}}{20 \, \text{mm}^2} = 25 \, \text{N/mm}^2
```

Dragspänningen i aluminiumstången är 25 N/mm².

### Övning 2: Töjning och Förlängning

En koppartråd med en ursprunglig längd på 2 meter och en tvärsnittsarea på 1 mm² utsätts för en dragkraft på 200 N. Elasticitetsmodulen för koppar är 110 000 N/mm². Beräkna töjningen och den totala förlängningen av tråden.

**Lösning:**

Först beräknar vi spänningen:

```latexmath
\sigma = \frac{F}{A}
```

där:
- `F = 200 \text{N}`$
- `A = 1 \, \text{mm}^2`$

```latexmath
\sigma = \frac{200 \, \text{N}}{1 \, \text{mm}^2} = 200 \, \text{N/mm}^2
```

Nu beräknar vi töjningen `ε`:

```latexmath
\epsilon = \frac{\sigma}{E}
```

där:
- `\sigma = 200 \, \text{N/mm}^2`$
- `E = 110 000 \, \text{N/mm}^2`$

```latexmath
\epsilon = \frac{200 \, \text{N/mm}^2}{110 000 \, \text{N/mm}^2} \approx 0.001818
```

Förlängningen `ΔL` är:

```latexmath
\Delta L = \epsilon \cdot L
```

där `L = 2 \, \text{m}`$ (ursprunglig längd):

```latexmath
\Delta L = 0.001818 \cdot 2 \, \text{m} = 0.003636 \, \text{m} = 3.636 \, \text{mm}
```

Den totala förlängningen av koppartråden är 3.636 mm.

### Övning 3: Materialval

Två material, stål och aluminium, används för att tillverka stänger med samma dimensioner (tvärsnittsarea och längd). Elasticitetsmodulen för stål är 210 000 N/mm² och för aluminium är den 70 000 N/mm². Om båda stängerna utsätts för samma dragkraft, vilken stång kommer att ha den största töjningen? Beräkna töjningen för båda materialen.

**Lösning:**

Låt oss anta att dragkraften `F` och tvärsnittsarean `A` är samma för båda materialen.

För stål:

```latexmath
\sigma = \frac{F}{A}
```

Töjningen `ε_stål` är:

```latexmath
\epsilon_{stål} = \frac{\sigma}{E_{stål}}
```

För aluminium:

```latexmath
\sigma = \frac{F}{A}
```

Töjningen `ε_aluminium` är:

```latexmath
\epsilon_{aluminium} = \frac{\sigma}{E_{aluminium}}
```

Eftersom `E_{stål} = 210 000 \, \text{N/mm}^2`$ och `E_{aluminium} = 70 000 \, \text{N/mm}^2`$:

```latexmath
\epsilon_{stål} = \frac{\sigma}{210 000 \, \text{N/mm}^2}
```

```latexmath
\epsilon_{aluminium} = \frac{\sigma}{70 000 \, \text{N/mm}^2}
```

Eftersom elasticitetsmodulen för aluminium är mindre än för stål, kommer aluminiumstången att ha den största töjningen.

### Övning 4: Säkerhetsfaktor

En plaststång med en tvärsnittsarea på 5 mm² och en längd på 1 meter utsätts för en dragkraft på 50 N. Plastens elasticitetsmodul är 3 000 N/mm². Om det maximalt tillåtna töjningsvärdet för plasten är 0.01, beräkna säkerhetsfaktorn för denna belastning.

**Lösning:**

Först beräknar vi spänningen `σ`:

```latexmath
\sigma = \frac{F}{A}
```

där:
- `F = 50 \text{N}`$
- `A = 5 \, \text{mm}^2`$

```latexmath
\sigma = \frac{50 \, \text{N}}{5 \, \text{mm}^2} = 10 \, \text{N/mm}^2
```

Nu beräknar vi töjningen `ε`:

```latexmath
\epsilon = \frac{\sigma}{E}
```

där:
- `σ = 10 \, \text{N/mm}^2`$
- `E = 3 000 \, \text{N/mm}^2`$

```latexmath
\epsilon = \frac{10 \, \text{N/mm}^2}{3 000 \, \text{N/mm}^2} \approx 0.003333
```

Säkerhetsfaktorn `SF` är:

```latexmath
SF = \frac{\epsilon_{max}}{\epsilon}
```

där `ε_{max} = 0.01`$ (maximalt tillåtet töjningsvärde):

```latexmath
SF = \frac{0.01}{0.003333} \approx 3
```

Säkerhetsfaktorn för denna belastning är cirka 3.

### Övning 5: Spänning i en Kompositstång

En kompositstång består av två olika material: material A med en tvärsnittsarea på 8 mm² och material B med en tvärsnittsarea på 12 mm². En total dragkraft på 1 000 N appliceras på kompositstången. Elasticitetsmodulen för material A är 150 000 N/mm² och för material B är 100 000 N/mm². Beräkna den totala dragspänningen i kompositstången och fördelningen av spänningen mellan de två materialen.

**Lösning:**

Först beräknar vi spänningen för varje material:

För material A:

```latexmath
\sigma_A = \frac{F_A}{A_A}
```

där:
- `F_A = 400 \text{N}`$ (dragkraft för material A)
- `A_A = 8 \, \text{mm}^2`$

```latexmath
\sigma_A = \frac{400 \, \text{N}}{8 \, \text{mm}^2} = 50 \, \text{N/mm}^2
```

För material B:

```latexmath
\sigma_B = \frac{F_B}{A_B}
```

där:
- `F_B = 600 \text{N}`$ (dragkraft för material B)
- `A_B = 12 \, \text{mm}^2`$

```latexmath
\sigma_B = \frac{600 \, \text{N}}{12 \, \text{mm}^2} = 50 \, \text{N/mm}^2
```

Den totala dragspänningen i kompositstången är summan av spänningarna i de två materialen, vilket är 50 N/mm².
