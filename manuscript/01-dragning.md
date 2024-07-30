# Dragning

**Dragning** är en grundläggande mekanisk belastning som uppstår när en kraft verkar längs en kropps längdaxel och drar den isär. Denna typ av belastning är vanlig i många strukturella applikationer, såsom kablar, stänger och andra komponenter som måste motstå dragkrafter.

## Definition av Dragning

Dragning inträffar när en yttre kraft appliceras på ett material så att materialet sträcks ut. Denna kraft kallas **dragkraft** och resulterar i en **spänning** inom materialet. Spänning mäter den inre kraften per ytenhet som uppstår på grund av den applicerade belastningen.

Enheten för kraft är Newton (N). En Newton definieras som den kraft som krävs för att accelerera ett föremål med en massa på ett kilogram med en hastighet av en meter per sekundkvadrat.

Formeln för spänning `σ` (sigma) är:

{title: "Spänningsformeln"}
```latexmath
\sigma = \frac{F}{A}
```

där:
- \(`σ`\) är spänningen i N/mm² (grekiska bokstaven sigma). Kan även uttryckas MPa.
- \(`F`\) är den applicerade kraften i Newton (N)
- \(`A`\) är tvärsnittsarean av materialet i kvadratmillimeter (mm²)

## Exempel på Beräkning av Dragspänning

Anta att vi har en stång med en tvärsnittsarea på 10 mm² och en dragkraft på 1000 N applicerad längs stångens längdaxel. Vi kan beräkna dragspänningen enligt följande med Hookes lag:

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

Om man vill göra beräkningen i Python så följer här exempel på det.

 {caption: "Beräkna dragspänning i Python"}
```python
def berakna_dragspanning(kraft, area_mm2):
    """
    Beräknar dragspänning.

    Parameters:
    kraft (float): Kraft i Newton.
    area_mm2 (float): Tvärsnittsarea i kvadratmillimeter.

    Returns:
    float: Dragspänning i N/mm².
    """
    return kraft / area_mm2


kraft = 1000  # Newton
area_mm2 = 10  # kvadratmillimeter

dragspanning = berakna_dragspanning(kraft, area_mm2)
print(f"Dragspänningen är {dragspanning} N/mm²")
```

När vi kör denna kod så får vi följande resultat.
```bash
Dragspänningen är 100.0 N/mm²
```

## Hookes Lag och Elastiska Gränser

Enligt Hookes lag är **töjningen** `ε` proportionell mot den applicerade spänningen `σ` så länge materialet inte överskrider sin elastiska gräns. **Elasticitetsmodulen** `E` för materialet beskriver materialets styvhet.

{title: "Hookes lag"}
```latexmath
\sigma = E \cdot \epsilon
```

där:
- \(`σ`\) är spänningen i N/mm²
- \(`E`\) är elasticitetsmodulen eller Youngs modulus i N/mm²
- \(`ε`\) är töjningen, enhetslös

För stål är elasticitetsmodulen typiskt omkring 210 000 N/mm². Om vi använder detta värde, kan vi beräkna töjningen `ε` som orsakas av den tidigare beräknade dragspänningen.

```latexmath
\epsilon = \frac{\sigma}{E}
```

Med `\sigma = 100 \, \text{N/mm}^2`$ och `E = 210 000 \, \text{N/mm}^2`$:

```latexmath
\epsilon = \frac{100 \, \text{N/mm}^2}{210 000 \, \text{N/mm}^2} \approx 0.000476
```

Detta betyder att för varje meter av stången, sker en förlängning på cirka 0.000476 meter (eller 0.476 millimeter).

Här kombinerar vi beräkning av dragspänning och töjning i ett Python program.

 {caption: "Beräkna töjning i Python"}
```python
def berakna_dragspanning(kraft, area_mm2):
    """
    Beräknar dragspänning.

    Parameters:
    kraft (float): Kraft i Newton.
    area_mm2 (float): Tvärsnittsarea i kvadratmillimeter.

    Returns:
    float: Dragspänning i N/mm².
    """
    return kraft / area_mm2

def berakna_tojning_mm_per_meter(dragspanning, elasticitetsmodul=210000):
    """
    Beräknar töjning i millimeter per meter.

    Parameters:
    dragspanning (float): Dragspänning i N/mm².
    elasticitetsmodul (float): Elasticitetsmodulen för materialet i N/mm² (standardvärde för stål är 210000 N/mm²).

    Returns:
    float: Töjning i mm/meter.
    """
    # Beräkna töjning som är enhetslös
    tojning = dragspanning / elasticitetsmodul
    # Konvertera enhetslös töjning till mm/meter för tydligare förståelse
    tojning_mm_per_meter = tojning * 1000  # 1 meter = 1000 millimeter
    return tojning_mm_per_meter

# Exempel på användning
kraft = 1000  # Newton
area_mm2 = 10  # kvadratmillimeter

dragspanning = berakna_dragspanning(kraft, area_mm2)
tojning_mm_per_meter = berakna_tojning_mm_per_meter(dragspanning)

print(f"Dragspänningen är {dragspanning:} N/mm²")
print(f"Töjningen är {tojning_mm_per_meter:.3f} mm/meter")
```

När vi kör denna kod så får vi följande resultat.
```
Dragspänningen är 100.0 N/mm²
Töjningen är 0.476 mm/meter
```

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


### Övning 2: Töjning och Förlängning

En koppartråd med en ursprunglig längd på 2 meter och en tvärsnittsarea på 1 mm² utsätts för en dragkraft på 200 N. Elasticitetsmodulen för koppar är 110 000 N/mm². Beräkna töjningen och den totala förlängningen av tråden.

### Övning 3: Materialval

Två material, stål och aluminium, används för att tillverka stänger med samma dimensioner (tvärsnittsarea och längd). Elasticitetsmodulen för stål är 210 000 N/mm² och för aluminium är den 70 000 N/mm². Om båda stängerna utsätts för samma dragkraft, vilken stång kommer att ha den största töjningen? Beräkna töjningen för båda materialen.

### Övning 4: Säkerhetsfaktor

En plaststång med en tvärsnittsarea på 5 mm² och en längd på 1 meter utsätts för en dragkraft på 50 N. Plastens elasticitetsmodul är 3 000 N/mm². Om det maximalt tillåtna töjningsvärdet för plasten är 0.01, beräkna säkerhetsfaktorn för denna belastning.

### Övning 5: Spänning i en Kompositstång

En kompositstång består av två olika material: material A med en tvärsnittsarea på 8 mm² och material B med en tvärsnittsarea på 12 mm². En total dragkraft på 1 000 N appliceras på kompositstången. Elasticitetsmodulen för material A är 150 000 N/mm² och för material B är 100 000 N/mm². Beräkna den totala dragspänningen i kompositstången och fördelningen av spänningen mellan de två materialen.
