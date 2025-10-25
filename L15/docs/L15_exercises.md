# L15 - Lektionsuppgifter

## Del 1 - Repetitionsuppgifter

### 1.1 - Deriveringsregler

Derivera följande funktioner:
* **a)** $f(x) = x^2 * e^4x$
* **b)** $f(x) = x^3 * ln 2x$
* **c)** $f(x) = \frac{e^2x}{log_{10}{4x}}$

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
* $i'(t)'$ = strömförändringen genom spolen i $A/s$.

Energin $w(t)$ som lagras i spolen ges av följande funktion:

```math
w(t) = \int_0^t p(t)\,dt
```

Energin mäts i $J$ $(Joule)$.

**a)** Bestäm $p(t)$.\
**b)** Bestäm den primitiva funktionen $P(t)$ till $p(t)$.\
**c)** Bestäm ett uttryck för energin i spolen $w(t)$ som en funktion av tiden.\
**d)** Spolen är oladdad vid start, dvs. $w(0) = 0$. Bestäm integrationskonstanten $C$.\
**e)** Bestäm hur mycket energi som har lagrats i spolen under de första $3$ sekunderna $(0{\le}\,t\,{\le}\,3)$.

---

### 2.2 - Integrering av en växelspänning (svår)

En resistor $R = 10$ $\Omega$ matas med följande växelspänning $u(t)$:

```math
u(t) = 230sin(100{\pi}t)
```

Effektutvecklingen $p(t)$ i resistorn ges av följande funktion:

```math
p(t) = u(t) * i(t),
```

där
* $u(t)$ = matningsspänningen,
* $i(t)$ = strömmen genom kretsen.

Strömmen $i(t)$ kan beräknas med Ohms lag:

```math
i(t) = \frac{u(t)}{R},
```

vilket ger

```math
p(t) = \frac{u^2(t)}{R} = \frac{230^2}{10}\sin^2(100{\pi}t),
```

där $w$ = $100{\pi}$ är vinkelfrekvensen i $rad/s$.

Via den trigonometriska identiteten:

```math
sin^2(x) = \frac{1}{2}\big(1 - \cos(2x)\big),
```

som motsvarar att

```math
sin^2(100{\pi}t) = \frac{1}{2}\big(1 - \cos(200{\pi}t)\big)
```

kan $p(t)$ skrivas om till

```math
p(t) = \frac{230^2}{10} * \frac{1}{2}\big(1 - \cos(200{\pi}t)\big) = \frac{230^2}{20}\big(1 - \cos(200{\pi}t)\big),
```

vilket kan förenklas till

```math
p(t) = 2645\big(1 - \cos(200{\pi}t)\big)
```

Sambandet mellan periodtiden $T$, frekvensen $f$ samt vinkelfrekvensen $w$ ges av följande samband:

```math
T = \frac{1}{f},
```

där frekvensen $f$ kan uttryckas med hjälp av vinkelfrekvensen $w$:

```math
w = 2{\pi}f => f = \frac{w}{2{\pi}}
```


**a)** Bestäm den primitiva funktionen $P(t)$ till $p(t)$.\
**b)** Beräkna den genomsnittliga effektutvecklingn $P_{avg}$ i resistorn under en period $T$ via följande formel:

```math
P_{avg} = \frac{1}{T} \int_0^T{p(t)}\,dt
```