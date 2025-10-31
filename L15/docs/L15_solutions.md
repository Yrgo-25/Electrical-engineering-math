# L15 - Lösningsförslag till lektionsuppgifter

## Del 1 - Repetitionsuppgifter

### 1.1 - Deriveringsregler

Derivera följande funktioner:
* **a)** $f_1(x) = x^2 * e^{4x}$
* **b)** $f_2(x) = x^3 * \ln 2x$
* **c)** $f_3(x) = \frac{x^3}{\ln x^2}$

---

### Lösning

**a)** Vi använder produktregeln: 

```math
f_1(x)' = (x^2)' * e^{4x} + x^2 * (e^{4x})',
```

där

```math
(x^2)' = 2x
```

samt

```math
(e^{4x})' = e^{4x} * (4x)' = 4e^{4x},
```

Därmed gäller att

```math
f_1(x)' = 2x * e^{4x} + x^2 * 4e^{4x},
```

som kan skrivas om till

```math
f_1(x)' = 2xe^{4x} + 4x^2 * e^{4x}
```

Slutligen kan vi bryta ut $2xe^{4x}$:

```math
f_1(x)' = 2xe^{4x}(1 + 2x),
```

som är ekvivalent med

```math
f_1(x)' = 2xe^{4x}(2x + 1)
```

**b)** Vi använder produktregeln kombinerat med kedjeregeln:

```math
f_2(x)' = (x^3)' * \ln 2x + x^3 * (\ln 2x)',
```

där

```math
(x^3)' = 3x^2
```

samt

```math
(\ln 2x)' = \frac{1}{2x} * (2x)' = \frac{1}{2x} * 2 = \frac{1}{x}
```

Därmed gäller att

```math
f_2(x)' = 3x^2 * \ln 2x + x^3 * \frac{1}{x}
```

Vidare gäller att

```math
x^3 * \frac{1}{x} = \frac{x^3}{x} = x^{3-1} = x^2,
```

vilket innebär att

```math
f_2(x)' = 3x^2 * \ln 2x + x^2
```

Slutligen kan vi bryta ut $x^2$:

```math
f_2(x)' = x^2(3{\ln 2x} + 1)
```

**c)** Vi använder kvotregeln i kombination med kedjeregeln:

```math
f_3(x)' = \frac{(x^3)' * \ln x^2 - x^3 * (\ln x^2)'}{(\ln x^2)^2},
```

där

```math
(x^3)' = 3x^2
```

samt

```math
(\ln x^2)' = \frac{1}{x^2} * (x^2)' = \frac{1}{x^2} * 2x = \frac{2x}{x^2} = \frac{2}{x}
```

Därmed gäller att

```math
f_3(x)' = \frac{3x^2 * \ln x^2 - x^3 * \frac{2}{x}}{(\ln x^2)^2}
```

Vidare gäller att

```math
x^3 * \frac{2}{x} = \frac{2x^3}{x} = 2x^{3-1} = 2x^2,
```

vilket innebär att

```math
f_3(x)' = \frac{3x^2{\ln x^2} - 2x^2}{(\ln x^2)^2}
```

#### Extrasteg

Vi kan också bryta ut $2x^2$ ur täljaren:

```math
f_3(x)' = \frac{2x^2(1,5{\ln x^2} - 1)}{(\ln x^2)^2}
```

Vi kan också utnyttja att $\ln x^2 = 2{\ln |x|}$:

```math
f_3(x)' = \frac{2x^2(1,5 * 2{\ln |x|} - 1)}{(2{\ln |x|})^2},
```

som kan skrivas om till

```math
f_3(x)' = \frac{2x^2(3{\ln |x|} - 1)}{(2{\ln |x|})^2},
```

Vidare gäller att

```math
(2{\ln |x|})^2 = 4(\ln |x|)^2,
```

vilket innebär att 

```math
f_3(x)' = \frac{2x^2(3{\ln |x|} - 1)}{4(\ln |x|)^2},
```

som slutligen kan förenklas till

```math
f_3(x)' = \frac{x^2(3{\ln |x|} - 1)}{2(\ln |x|)^2},
```

---

## Del 2 - Nytt stoff

### 2.1 - Energi lagrad i en spole
Strömmen genom en spole är tidsberoende och ges av följande funktion:

```math
i(t) = 5t,
```

där $t$ = tiden i sekunder. Strömmen mäts i $A$ $(Ampere)$.

Spolens induktans $L = 0,20$ $H$ $(Henry)$.

Effektutvecklingen $p(t)$ i spolen ges av följande funktion:

```math
p(t) = L * i(t) * i'(t),
```

där
* p(t) = effektutvecklingen i $W$ $(Watt)$,
* $L$ = spolens induktans i $H$ $(Henry)$,
* $i(t)$ = strömmen genom spolen i $A$ $(Ampere)$,
* $i'(t)$ = strömförändringen genom spolen i $A/s$.

Energin $w(t)$ som lagras i spolen mellan tiden $0 - t$ ges av följande funktion:

```math
w(t) = \int_0^t p(t)\,dt
```

Energin mäts i $J$ $(Joule)$.

**a)** Bestäm $p(t)$.\
**b)** Bestäm den primitiva funktionen $P(t)$ till $p(t)$.\
**c)** Bestäm ett uttryck för energin i spolen $w(t)$ som en funktion av tiden.\
**d)** Spolen är oladdad vid start, dvs. $w(0) = 0$. Bestäm integrationskonstanten $C$.\
**e)** Bestäm hur mycket energi som har lagrats i spolen under de första $3$ sekunderna $(0{\le}\,t\,{\le}\,3)$.\

---

### Lösning

**a)** För att bestämma $p(t)$ måste vi bestämma $i'(t)$:

```math
i'(t) = (5t)' = 5
```

Därmed kan vi bestämma ett uttryck för $p(t)$:

```math
p(t) = L * i(t) * i'(t) = 0,2 * 5t * 5 = 5t
```

**b)** För att bestämma $P(t)$ integrerar vi $p(t)$ utan tidsintervall:

```math
P(t) = \int p(t)\,dt = \int (5t)\,dt = \frac{5t^2}{2} + C,
```

där $C$ = integrationskonstanten.

**c)** Eftersom energin $w(t)$ som lagras i spolen mellan tiden $0 - t$ ges av funktionen

```math
w(t) = \int_0^t p(t)\,dt
```

så gäller att energin i spolen $w(t)$ som en funktion av tiden, dvs. utan tidsintervall, är ekvivalent
med den primitiva funktionen $P(t)$, då

```math
w(t) = \int p(t)\,dt = \int (5t)\,dt = \frac{5t^2}{2} + C
```

Notera att uttrycket är identiskt med $P(t)$.

**d)** Genom att bestämma $w(0)$ via det framtagna uttrycket ser vi att $C = 0$, då

```math
w(0) = \frac{5 * 0^2}{2} + C = 0 => C = 0
```

Därmed kan yttrycket $w(t)$ slutligen fastställas:

```math
w(t) = \frac{5t^2}{2}
```

**e)** Vi integrerar $p(t)$ för $0$ $\le$ $t$ $\le$ $3$:

```math
w(t) = \int_0^3 p(t)\,dt = \int_0^3 (5t)\,dt = \big[\frac{5t^2}{2} + C\big]_0^3,
```

som kan utvecklas till

```math
w(t) = \big(\frac{5 * 3^2}{2} + C\big) - \big(\frac{5*0^2}{2} + C\big),
```

vilket kan förenklas till

```math
w(t) = \big(\frac{5 * 9}{2} + C\big) - C = 22,5 J
```

Under de tre första sekunderna lagras alltså $22,5$ $J$ i spolen.

---