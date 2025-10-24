# L13 – Lektionsuppgifter

## Del 1 - Repetitionsuppgifter

### 1.1 – Analys av en kubisk funktion

Betrakta följande funktion:

```math
f(x) = -0,5x^3 + 1,5x^2 + 4,5x - 3
```

**a)** Derivera funktionen $f(x)$ och bestäm uttrycket för $f'(x)$.  
**b)** Bestäm var funktionen är stationär, dvs. lös ekvationen $f'(x) = 0$.  
**c)** Avgör med hjälp av den andra derivatan om respektive stationär punkt är ett maximum eller minimum.  
**d)** Beräkna funktionens största och minsta värde.  
**e)** Rita upp grafen till $f(x)$ via [Geogebra](https://www.geogebra.org/graphing?lang=en), kontrollera att
dina svar stämmer.

---

### Lösning

**a)** Vi deriverar $f(x)$ för att bestämma $f'(x)$:

```math
f'(x) = -1,5x^2 + 3x + 4,5
```

**b)** Vi bestämmer när $f'(x) = 0$:

```math
f'(x) = -1,5x^2 + 3x + 4,5 = 0
```

Ovanstående uttryck kan skrivas om till

```math
1,5x^2 = 3x + 4,5
```

Vi dividerar med $1,5$ i respektive led och erhåller då följande uttryck:

```math
x^2 = 2x + 3
```

Vi beräknar rötterna för $x$ via PQ-formeln:

```math
x = \frac{2}{2} \pm \sqrt{(\frac{2}{2})^2 + 3},
```

vilket kan skrivas om till

```math
x = 1 \pm \sqrt{1 + 3},
```

där

```math
\sqrt{1 + 3} = \sqrt{4} = 2
```

Därmed gäller att

```math
x = 1 \pm 2
```

Därmed kan vi beräkna rötterna:

```math
x_1 = 1 + 2 = 3
```

```math
x_2 = 1 - 2 = -1
```

Funktionen är därmed stationär när $x = 3$ samt $x = -1$.

**c)** Vi bestämmer den andra derivatan $f''(x)$ genom att derivera $f'(x)$:

```math
f''(x) = -3x + 3
```

Vi är intresserade av den andra derivatan i extrempunkterna $x_1$ samt $x_2$.\

Vi börjar med att bestämma $f''(x_1)$:

```math
f''(x_1) = f''(3) = -3 * 3 + 3 = -6 => maxvärde
```

Eftersom $f''(x_1) < 0 $ gäller att funktionen har ett maximum i denna punkt:
* $f'(x_1) = 0$ indikerar att lutningen i denna punkt är $0$ => kurvan vänder.
* $f''(x_1) < 0$ indikerar att lutningen är på väg att minska => aktuellt värde är ett maximum och kurvan är därmed på väg nedåt.

Vi bestämmer sedan $f''(x_2)$:

```math
f''(x_2) = f''(-1) = -3 * (-1) + 3 = 6 => minvärde
```

Eftersom $f''(x_2) > 0 $ gäller att funktionen har ett minimum i denna punkt:
* $f'(x_2) = 0$ indikerar att lutningen i denna punkt är $0$ => kurvan vänder.
* $f''(x_2) > 0$ indikerar att lutningen är på väg att öka => aktuellt värde är ett minimum och kurvan är därmed på väg uppåt.

**d)** Vi beräknar funktionens min- respektive maxvärde genom att sätta in extrempunkterna $x_1$ samt $x_2$ i den givna funktionen $f(x)$.

Vi börjar med att beräkna maximipunkten $f(x_1)$:

```math
f(x_1) = -0,5 * 3^3 + 1,5 * 3^2 + 4,5 * 3 - 3 = 10,5
```

Funktionen har därmed en maximipunkt i $(x; y)$ = $(3; 10,5)$.

Vi beräknar sedan minimipunkten $f(x_2)$:

```math
f(x_2) = -0,5 * (-1)^3 + 1,5 * (-1)^2 + 4,5 * (-1) - 3 = -5,5
```
Funktionen har därmed en minimipunkt i $(x; y)$ = $(-1; -5,5)$.

**e)** Funktionen graf visas nedan. Denna indikerar att våra beräkningar stämmer:

![Funktionens graf ritad i `Geogebra`](./images/1.1_geogebra.png)

---

## 1.2 - Analys av spänning över en kondensator

En kondensator i en RC-krets laddas och urladdas upprepade gånger. Spänningen över kondensatorn kan beskrivas med följande funktion:

```math
u(t) = -0,2t^3 + 1,2t^2 - 1,4625t + 3,
```

där

* $u(t)$ = spänningen över kondensatorn i $V$,
* $t$ = tiden i sekunder, där $0 ≤ t ≤ 6$.

**a)** Derivera funktionen och bestäm uttrycket för spänningens förändringshastighet $u'(t)$.\
**b)** Bestäm den tidpunkt (eller tidpunkter) då spänningen är stationär, dvs. när $u'(t) = 0$.\
**c)** Avgör med hjälp av den andra derivatan om punkterna är maximi- eller minimipunkter.\
**d)** Beräkna spänningens största och minsta värde.\
**e)** Rita upp grafen för $u(t)$ via [Geogebra](https://www.geogebra.org/graphing?lang=en), kontrollera att
dina svar stämmer.

---

### Lösning

**a)** Vi deriverar $u(t)$ för att bestämma $u'(t)$:

```math
u'(t) = -0,6t^2 + 2,4t - 1,4625
```

**b)** Vi bestämmer när $u'(t) = 0$:

```math
u'(t) = -0,6t^2 + 2,4t - 1,4625 = 0
```

Ovanstående uttryck kan skrivas om till

```math
0,6t^2 = 2,4t - 1,4625
```

Vi dividerar med $0,6$ i respektive led och erhåller då följande uttryck:

```math
t^2 = 4t - 2,4375
```

Vi beräknar rötterna för $t$ via PQ-formeln:

```math
t = \frac{4}{2} \pm \sqrt{(\frac{4}{2})^2 - 2,4375},
```

vilket kan skrivas om till

```math
t = 2 \pm \sqrt{1,5625},
```

där

```math
\sqrt{1,5625} = 1,25
```

Därmed gäller att

```math
t = 2 \pm 1,25
```

Därmed kan vi beräkna rötterna:

```math
t_1 = 2 - 1,25 = 0,75\,s
```

```math
t_2 = 2 + 1,25 = 3,25\,s
```

Spänningen är därmed stationär när $t$ = $0,75$ $s$ samt $t$ = $3,25$ $s$.

**c)** Vi bestämmer den andra derivatan $u''(t)$ genom att derivera $u'(t)$:

```math
u''(t) = -1,2t + 2,4
```

Vi är intresserade av den andra derivatan i extrempunkterna $t_1$ samt $t_2$.\

Vi börjar med att bestämma $u''(t_1)$:

```math
u''(t_1) = u''(0,75) = -1,2 * 0,75 + 2.4 = 1,5 => minpunkt
```

Eftersom $u''(t_1) > 0 $ gäller att funktionen har ett minimum i denna punkt:
* $u'(t_1) = 0$ indikerar att lutningen i denna punkt är $0$ => kurvan vänder.
* $u''(t_1) > 0$ indikerar att lutningen är på väg att öka => aktuellt värde är ett minimum och kurvan är därmed på väg uppåt.

Vi bestämmer sedan $u''(t_2)$:

```math
u''(t_2) = u''(3,25) = -1,2 * 3,25 + 2.4 = -1,5 => maxpunkt
```

Eftersom $u''(t_2) < 0 $ gäller att funktionen har ett maximum i denna punkt:
* $u'(t_2) = 0$ indikerar att lutningen i denna punkt är $0$ => kurvan vänder.
* $u''(t_2) < 0$ indikerar att lutningen är på väg att minska => aktuellt värde är ett maximum och kurvan är därmed på väg nedåt.

**d)** Vi beräknar spänningens min- respektive maxvärde genom att sätta in extrempunkterna $t_1$ samt $t_2$ i den givna funktionen $u(t)$.

Vi börjar med att beräkna minimipunkten $u(t_1)$:

```math
u(t_1) = u(0,75) = -0,2 * 0,75^3 + 1,2 * 0,75^2 - 1,4625 * 0,75 + 3 \approx 2,49 V
```

Spänningen har därmed en minimipunkt i $(t; u(t))$ \approx $(0,75; 2,49)$.\

Vi beräknar sedan maximipunkten $u(t_2)$:

```math
u(t_2) = u(3,25) = -0,2 * 3,25^3 + 1,2 * 3,25^2 - 1,4625 * 3,25 + 3 \approx 4,06 V
```
Spänningen har därmed en maximipunkt i $(t; u(t))$ \approx $(3,25; 4,06)$.\

**e)** Funktionen graf visas nedan. Denna indikerar att våra beräkningar stämmer:

![Funktionens graf ritad i `Geogebra`](./images/1.2_geogebra.png)

## Del 2 - Nytt stoff

### 2.1 - Ström genom en spole

Strömmen genom en spole varierar över tid enligt följande funktion:

```math
i(t) = 4sin(50t)
```

där
* $i(t)$ = strömmen genom spolen i $A$,
* $t$ = tiden i sekunder.

**a)** Derivera funktionen och bestäm uttrycket för $i'(t)$.\
**b)** Bestäm den tidpunkt (eller tidpunkter) då strömmen är stationär, dvs. när $i'(t) = 0$.\
**c)** Avgör med hjälp av den andra derivatan om punkterna är maximi- eller minimipunkter.\
**d)** Beräkna strömmens största och minsta värde. Fundera om detta stämmer med våra förväntningar.

---

### Lösning

**a)** Vi deriverar $i(t)$ för att bestämma $i'(t)$. När $sin$ deriveras resulterar detta i $cos$. 
Vi tar också den så kallade inre derivatan i beaktning genom multiplicera med derivatan av $50t$, vilket är $50$:

```math
i'(t) = 4cos(50t) * 50,
```

som kan skrivas om till

```math
i'(t) = 200cos(50t)
```

**Notering**: Ovan användes den så kallade kedjeregeln, som säger att för en given funktion $f(x)$:

```math
f(x) = a * sin(bx),
```

kan motsvarande derivata $f'(x)$ beräknas enligt nedan:

```math
f'(x) = a * cos(bx) * \frac{d}{dx}(bx),
```

där $\frac{d}{dx}(bx)$ är den inre derivatan av $cos(bx)$ och bestäms enligt nedan:

```math
\frac{d}{dx}(bx) = b
```

Därmed gäller att

```math
f'(x) = a * cos(bx) * b,
```

vilket kan skrivas om till

```math
f'(x) = ab * cos(bx)
```

**b)** Vi bestämmer när $i'(t)$ = $0$:

```math
i'(t) = 200cos(50t) = 0
```

Vi dividerar med $200$ i respektive led:

```math
cos(50t) = 0
```

För att få bort $cos$ ur vänsterleder lägger vi till $cos^-1$ i båda led. Detta ger oss följande:

```math
50t = cos^{-1}(0) \pm k{\pi}, = \frac{\pi}{2} \pm k{\pi}
```

där $k = 0, 1, 2... n$.


Vi använder de två minsta rötterna, vilket vi får när $k$ = $0$ respektive $1$. 
Därmed gäller att vi kan beräkna tiderna $t_1$ samt $t_2$.

Vi börjar med att bestämma $t_1$ med $k$ = $0$:

```math
50t_1 = \frac{\pi}{2},
```

vilket via division med $50$ i både led ger oss att $t_1$ är ca $31$ $ms$, då

```math
t_1 = \frac{\pi}{2 * 50} \approx 0,031 s 
```

Vi bestämmer sedan $t_2$ med $k$ = $1$:

```math
50t_2 = \frac{\pi}{2} + {\pi} = \frac{3{\pi}}{2},
```

vilket via division med $50$ i både led ger oss att $t_2$ är ca $94$ $ms$, då

```math
t_2 = \frac{3{\pi}}{2 * 50} \approx 0,094 s 
```

**c)** Vi bestämmer andraderivatan $i''(t)$. När $cos$ deriveras resulterar detta i $-sin$. Vi tar
också den inre derivatan i beaktning genom multiplicera med derivatan av $50t$, vilket är $50$:

```math
i''(t) = 200 * (-sin(50t)) * 50, 
```

vilket kan skrivas om till

```math
i''(t) = -10000sin(50t) 
```

Vi bestämmer sedan ifall $t_1$ samt $t_2$ är min- eller maxpunkter genom att sätta in dessa i $i''(t)$:

```math
i''(t_1) \approx i''(0,031) = -10000sin(50 * 0,031) = -10000 => max
```

```math
i''(t_2) \approx i''(0,094) = -10000sin(50 * 0,094) = 10000 => min
```

Vi ser då att strömmens maxvärde nås efter $t_1 \approx 0,031$ $s$. Vi ser då också att strömmens
minvärde nås efter $t_2 \approx 0,094$ $s$. Detta är rimligt, då en sinusström når sitt maxvärde efter en
fjärdedel av periodtiden, medan minvärdet nås efter tre fjärdedelar av periodtiden.

**d)** Vi beräknar strömmens min- och maxvärde genom att sätta in $t_1$ samt $t_2$ i formeln för $i(t)$:

```math
i(t_1) \approx i(0,031) = 4sin(50 * 0,031) \approx 4 A
```

```math
i(t_2) \approx i(0,094) = 4sin(50 * 0,094) \approx -4 A
```

Eftersom strömmens amplitud $|I|$ = $4$ $A$ är max- och minvärdet förväntat:
* Strömmens maxvärde $4$ $A$ nås efter en fjärdedel av periodtiden, vilket är efter $t_1 \approx 0,031$ $s$.
* Strömmens minvärde $-4$ $A$ nås tre fjärdedelar av periodtiden, vilket är efter $t_2 \approx 0,094$ $s$.

---

### 2.2 - Urladdning av kondensator
Spänningen över en kondensator som urladdas ges av följande funktion:

```math
u(t) = 12 e^{-0,4t}
```

där
* $u(t)$ = spänningen över kondensatorn i $V$,
* $t$ = tiden i sekunder.

**a)** Derivera funktionen och bestäm uttrycket för $u'(t)$.\
**b)** Beräkna spänningens förändringshastighet vid $t = 2$ $s$.\
**c)** Ange om spänningsförändringen ökar eller minskar i denna punkt, dvs. bestäm $u''(2)$.

---

### Lösning

**a)** Vi deriverar funktionen $u(t)$ för att bestämma $u'(t)$. Vi använder följande regel:

```math
\frac{d}{dx}(e^{ax}) = e^{ax} * a = ae^{ax}
```

Den yttre derivatan av $e^{ax}$ är alltid samma, dvs. $e^{ax}$. Vi tar den inre derivatan i åtanke
genom att multiplicera den yttre derivatan med derivatan av exponenten $ax$, vilket blir $a$:

```math
\frac{d}{dx}(ax) = a
```

Vi gör samma för aktuell ekvation $u(t)$:

```math
u'(t) = 12e^{-0,4t} * -0,4,
```

vilket kan skrivas om till

```math
u'(t) = -4,8e^{-0,4t}
```

**b)** Vi beräknar spänningens förändringshastighet vid $t = 2$ $s$ genom att beräkna $u'(2)$:

```math
u'(2) = -4,8e^{-0,4 * 2} \approx -2,16\,V/s
```

**c)** Vi bestämmer andraderivatan $u''(t)$ genom att derivera $u'(t)$. Vi använder samma tillvägagångssätt
för att derivera $e^{ax}$ som visades tidigare:

```math
u''(t) = -4,8e^{-0,4t} * (-0,4),
```

vilket kan skrivas om till

```math
u''(t) = 1,92e^{-0,4t}\,V/s^2
```

Vi bestämmer sedan $u''(2)$:

```math
u''(2) = 1,92e^{-0,4 * 2} \approx 0,86 \,V/s^2
```

Eftersom $u''(2)$ > $0$ gäller att spänningsförändringen ökar vid tiden $t$ = $2$ $s$.

---

### 2.3 - Förstärkning i dB
Den logaritmiska förstärkningen i ett förstärkarsystem beskrivs av följande funktion:

```math
G(x) = 10log_{10}(2x + 1)
```

där
* $G(x)$ = förstärkningen i $dB$,
* $x$ = insignalsnivån (dimensionslös faktor).

**a)** Beräkna för vilket värde på $x$ som förstärkningen $G(x)$ = $2$ $dB$.\
**b)** Beräkna förstärkningens förändringshastighet $G'(x)$ i denna punkt.

***Notering**: Förändringshastigheten $G'(x)$ indikerar hur snabbt förstärkningen ändras när insignal $x$ förändras*.

---

### Lösning

**a)** Vi sätter upp en ekvation med $G(x)$ = $2$ $dB$:

```math
G(x) = 10log_{10}(2x + 1) = 2
```

Vi dividerar med $10$ i respektive led:

```math
log_{10}(2x + 1) = 0,2
```

Vi höjer båda led med basen $10$ för att få bort $log_{10}$ ur vänsterledet:

```math
2x + 1 = 10^{0,2}
```

Vi subtraherar sedan med $1$ i respektive led:


```math
2x = 10^{0,2} - 1
```

Slutligen dividerar vi med $2$ i båda led för att bestämma $x$:


```math
x = \frac{10^{0,2} - 1}{2} \approx 0,29
```

Vi kontrollräknar det beräknade värdet $x$ \approx $0,29$. Om vi har räknat rätt bör $G(x)$ bli $2$ $dB$
i denna punkt:

```math
G(0,29) = 10log_{10}(2 * 0,29 + 1) = 2 => OK
```

**b)** Vi utnyttjar följande regel för en given ekvation $f(x)$:

```math
f(x) = log_{10}(ax)
```

att dess derivata $f'(x)$ kan beräknas enligt nedan:

```math
f'(x) = \frac{1}{ax * \ln 10} * \frac{d}{dx}(ax)
```

där

```math
\frac{d}{dx}(ax) = a
```

Vi deriverar $G'(x)$ med denna regel:

```math
G'(x) = 10 * \frac{1}{(2x + 1) * \ln 10} * \frac{d}{dx}(2x + 1), 
```

där

```math
\frac{d}{dx}(2x + 1) = 2
```

Därmed gäller att

```math
G'(x) = \frac{10 * 1}{(2x + 1) * \ln 10} * 2, 
```

vilket kan skrivas om till

```math
G'(x) = \frac{20}{(2x + 1) * \ln 10}
```

Slutligen beräknar vi förstärkningens förändringshastighet $G'(x)$ när $x \approx 0,29$, dvs. $G(0,29)$:

```math
G'(0,29) \approx \frac{20}{(2 * 0,29 + 1) * \ln 10} \approx 5,48
```
