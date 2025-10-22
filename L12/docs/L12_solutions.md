# L12 – Lösningsförslag till lektionsuppgifter

## Del 1 - Repetitionsuppgifter

### 1.1 - Linjär förstärkning
Sambandet mellan den linjära förstärkningen samt förstärkningen mätt i dB visas nedan:

```math
G_{dB}=20*log_{10}G_{lin} 
```

där
* $G_{dB}$ = förstärkningen i $dB$,
* $G_{lin}$ = den linjära förstärkningen.

En ljudförstärkare har en förstärkning på $26$ $dB$. Beräkna den motsvarande linjära spänningsförstärkningen.

---

### Lösning

Vi skriver upp det givna uttrycket som en ekvation:

```math
G_{dB}=20*log_{10}G_{lin} = 26
```

Vi vill erhålla ett uttryck för $G_{lin}$. Vi börjar med att dividera med $20$ i respektive led:

```math
log_{10}G_{lin} = 1,3
```

Vi upphöjer sedan med basen $10$ i båda led för att bli av med $log_{10}$ i vänsterledet:

```math
G_{lin} = 10^{1,3} \approx 20
```

Därmed gäller att den linjära förstärkningen är ungefär lika med $20$.

---

### 1.2 - Utefter i dBm samt mW
Sambandet mellan en given effekt i $W$ samt motsvarande effekt i $dBm$ ($dB$ i förhållande till $1$ $mW$) visas nedan:

```math
P_{dBm}=10*log_{10}⁡\frac{P}{1 mW},
```

där 
* $P$ = effekten i $mW$,
* $P_{dBm}$ = motsvarande effekt i $dBm$.

En radiosändare har en uteffekt på $17$ $dBm$. Ange uteffekten i $mW$.

---

### Lösning

Vi skriver upp det givna uttrycket som en ekvation:

```math
P_{dBm}=10*log_{10}⁡\frac{P}{1 mW} = 17
```

Vi vill erhålla ett uttryck för $P$. Vi börjar med att dividera med $10$ i respektive led:

```math
log_{10}⁡\frac{P}{1 mW} = 1,7
```

Vi upphöjer sedan med basen $10$ i båda led för att bli av med $log_{10}$ i vänsterledet:

```math
\frac{P}{1 mW} =  10^{1,7}
```

Slutligen multiplicerar vi med $1$ $mW$ i respektive led för att beräkna $P$:


```math
P =  10^{1,7} * 1 mW \approx 50 mW
```

Uteffekten uppgår därmed till ca $50$ $mW$.

---

### 1.3 - Ljudnivå från multipla ljudkällor
För ett godtyckligt antal lika starka ljudkällor gäller att den totala ljudnivån kan beräknas enligt nedan:

```math
L_{tot}=L_{enkel}+10*log_{10}n,
```

där
* $L_{tot}$ = den totala ljudnivån,  
* $L_{enkel}$ = ljudnivån orsakad av en ljudkälla,
* $n$ = antalet ljudkällor.

Beräkna antalet lika starka ljudkällor om ljudet från en ljudkälla är $68$ $dB$ och den totala ljudnivån uppgår till $72,8$ dB.

---

### Lösning

Vi vänder på det givna uttrycket:

```math
L_{enkel}+10*log_{10}n = L_{tot} 
```

Vi vill erhålla ett uttryck för $n$. Vi börjar med att subtrahera med $L_{enkel}$ i respektive led:

```math
10*log_{10}n = L_{tot} - L_{enkel},
```

där 

```math
L_{tot} - L_{enkel} = 72,8 - 68 = 4,8
```

Därmed kan uttrycket skrivas om till

```math
10*log_{10}n = 4,8
```

Vi dividerar sedan med $10$ i respektive led:

```math
log_{10}n = \frac{4,8}{10},
```

vilket kan skrivas om till

```math
log_{10}n = 0,48
```

Vi upphöjer sedan med basen $10$ i båda led för att bli av med $log_{10}$ i vänsterledet:

```math
n = 10^{0,48} \approx 3
```

Antalet lika starka ljudkällor är därmed $3$.

## Del 2 - Nytt stoff

### 2.1 - Derivering av funktioner
Derivera följande funktioner:

**a)** $f(x) = -2x^2 + 2x + 4$

**b)** $f(x) = 3x^3 - 6x^2 + \frac{3x}{4} - 5$

**c)** $f(x) = -x^4 + x^3 + \frac{2x^2}{3} - 3x + 2$

---

### Lösning

**a)** $f(x) = -4x + 2$

**b)** $f(x) = 9x^2 - 12x + \frac{3}{4}$

**c)** $f(x) = -4x^3 + 3x^2 + \frac{4x}{3} - 3$

---

### 2.2 – Analys av en parabel

Betrakta följande funktion:

```math
f(x) = -x^2 + 6x - 5
```

**a)** Derivera funktionen $f(x)$, dvs. bestäm uttrycket för $f'(x)$.  
**b)** Bestäm var funktionen är stationär, dvs. lös ekvationen $f'(x) = 0$.  
**c)** Avgör med hjälp av den andra derivatan om punkten är ett **maximum** eller **minimum**.  
**d)** Beräkna funktionens största eller minsta värde.  
**e)** Rita upp grafen till $f(x)$ via [Geogebra](https://www.geogebra.org/graphing?lang=en), kontrollera att
dina svar stämmer.

---

### Lösning

**a)** Vi deriverar $f(x)$ för att bestämma $f'(x)$:

```math
 f'(x) = -2x + 6
 ```

**b)** Vi bestämmer när $f'(x) = 0$:

```math 
f'(x) = -2x + 6 = 0
```

Vi adderar $2x$ i respektive led och erhåller då följande uttryck:

```math
6 = 2x
```

Genom att vända på uttrycket samt dividera med $2$ i båda led ser vi att $f'(x) = 0$ när $x = 3$:

```math
x = 3
```

**c)** Vi bestämmer den andra derivatan $f''(x)$ genom att derivera $f'(x)$:

```math
f''(x) = -2
```

Vi är intresserade av den andra derivatan i extrempunkten $x = 3$, dvs. $f''(3)$.\
Efersom $f''(x) = 2$ för alla $x$ gäller att

```math
f''(3) = f''(x) = -2
```

Eftersom $f''(3) = -2$ gäller att funktionen har ett maximum när $x = 3$:
* $f'(3) = 0$ indikerar att lutningen i denna punkt är $0$ => kurvan vänder.
* $f''(3) < 0$ indikerar att lutningen är på väg att minska => aktuellt värde är ett maximum och kurvan är därmed på väg nedåt.

**d)** Vi beräknar funktionens maxvärde genom att sätta in extremvärdet $x=3$ i den givna funktionen $f(x)$.\
Därmed beräknar vi $f(3)$:

```math
f(3) = -3^2 + 6*3 - 5 = -9 + 18 - 5 = 4
```

Funktionen har därmed en maximipunkt i $(x, y) = (3, 4)$.

**e)** Funktionen graf visas nedan. Denna indikerar att våra beräkningar stämmer:

![Funktionens graf ritad i `Geogebra`](./images/2_2_geogebra.png)

---

## 2.3 – Analys av strömförlopp i en RC-krets

Strömmen genom en viss RC-krets kan approximeras med följande polynomfunktion:

```math
i(t) = -0,4t^3 + 2,4t^2 - 3t + 1,2
```

där  
* $i(t)$ = strömmen genom kretsen i $A$,  
* $t$ = tiden i sekunder.

**a)** Derivera funktionen för att bestämma uttrycket för strömmens förändring (strömändringshastigheten) $i'(t)$.\
**b)** Beräkna den tidpunkt (eller tidpunkter) då strömmen är stationär, dvs. när $i'(t) = 0$.\
**c)** Bestäm med hjälp av den **andra derivatan** om respektive stationär punkt är ett **maximum** eller **minimum**.\
**d)** Beräkna den maximala och minimala strömmen $i(t)$ i kretsen.\
**e)** Rita grafen till $i(t)$ via [Geogebra](https://www.geogebra.org/graphing?lang=en), kontrollera att
dina svar stämmer.

--- 

### Lösning

**a)** Vi deriverar $i(t)$ för att bestämma $i'(t)$:

```math
i'(t) = -1,2t^2 + 4,8t - 3
```

**b)** Vi bestämmer när $i'(t) = 0$:

```math
i'(t) = -1,2t^2 + 4,8t - 3 = 0
```

Ovanstående uttryck kan skrivas om till

```math
1,2t^2 = 4,8t - 3
```

Vi dividerar med $1,2$ i respektive led och erhåller då följande uttryck:

```math
t^2 = 4t - 2,5
```

Vi beräknar rötterna för $t$ via PQ-formeln:

```math
t = \frac{4}{2} \pm \sqrt{(\frac{4}{2})^2 - 2,5},
```

vilket kan skrivas om till

```math
t = 2 \pm \sqrt{2^2 - 2,5},
```

där

```math
2^2 - 2,5 = 1,5
```

Därmed gäller att

```math
t = 2 \pm \sqrt{1,5}
```

Därmed kan vi beräkna rötterna:


```math
t_1 = 2 - \sqrt{1,5} \approx 0,78 s
```

```math
t_2 = 2 + \sqrt{1,5} \approx 3,22 s
```

Strömmen är därmed stationär efter ungefär $0,78$ $s$ samt $3,22$ $s$.

**c)** Vi bestämmer den andra derivatan $i''(t)$ genom att derivera $i'(t)$:

```math
i''(t) = -2,4t + 4,8
```

Vi är intresserade av den andra derivatan i extrempunkterna $t_1$ samt $t_2$.\

Vi börjar med att bestämma $f''(t_1)$:

```math
f''(t_1) \approx f''(0,78) = -2,4 * 0,78 + 4,8 \approx 2,94 => minvärde
```

Eftersom $f''(t_1) > 0 $ gäller att funktionen har ett minimum vid tiden $t_1$:
* $f'(t_1) = 0$ indikerar att lutningen i denna punkt är $0$ => kurvan vänder.
* $f''(t_1) > 0$ indikerar att lutningen är på väg att öka => aktuellt värde är ett minimum och kurvan är därmed på väg uppåt.

Vi bestämmer sedan $f''(t_2)$:

```math
f''(t_2) \approx f''(3,22) = -2,4 * 3,22 + 4,8 \approx -2,94 => maxvärde
```

Eftersom $f''(t_2) < 0 $ gäller att funktionen har ett maximum vid tiden $t_2$:
* $f'(t_2) = 0$ indikerar att lutningen i denna punkt är $0$ => kurvan vänder.
* $f''(t_2) < 0$ indikerar att lutningen är på väg att minska => aktuellt värde är ett maximum och kurvan är därmed på väg nedåt.

**d)** Vi beräknar funktionens min- respektive maxvärde genom att sätta in extrempunkterna $t_1$ samt $t_2$ i den givna funktionen $i(t)$.\

Vi börjar med att beräkna mimimupunkten $i(t_1)$:

```math
i(t_1) \approx i(0,78) = -0,4 * 0,78^3 + 2,4 * 0,78^2 - 3 * 0,78 + 1,2 \approx 0,13 A
```

Funktionen har därmed en minimipunkt $0,13$ $A$ efter ca $0,78$ $s$.

Vi beräknar sedan maximipunkten $i(t_2)$:

```math
i(t_2) \approx i(3,22) = -0,4 * 3,22^3 + 2,4 * 3,22^2 - 3 * 3,22 + 1,2 \approx 3,07 A
```
Funktionen har därmed en maximipunkt $3,07$ $A$ efter ca $3,22$ $s$.

**e)** Funktionen graf visas nedan. Denna indikerar att våra beräkningar stämmer:

![Funktionens graf ritad i `Geogebra`](./images/2_3_geogebra.png)
