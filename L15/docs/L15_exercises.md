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
* $L$ = spolens induktans,
* $i(t)$ = strömmen genom spolen,
* $i'(t)'$ = strömförändringen genom spolen.

Energin $W$ som lagras i spolen ges av följande funktion:

```math
W = \int_0^t p(t) dt
```

Energin mäts i $J$ $(Joule)$.

**a)** Bestäm $p(t)$.\
**b)** Bestäm hur mycket energi som har lagrats i spolen under de första $3$ sekunderna $(0{\le}\,t\,{\le}\,3)$.

---

### 2.2 - Integrering av en växelspänning

En krets bestående av en resistor $R = 1 k{\Omega}$ matas med följande växelspänning $u(t)$:

```math
u(t) = 230sin(100{\pi}t)
```

Effektutvecklingen $p(t)$ i kretsen ges av följande funktion:

```math
p(t) = u(t) * i(t),
```

där
* $u(t)$ = matningsspänningen,
* $i(t)$ = strömmen genom kretsen.

Strömmen $i(t)$ kan beräknas med Ohms lag:

```math
i(t) = \frac{u(t)}{R}
```

Beräkna den genomsnittliga effekten $P_{avg}$ under en period $T$ via integrering.
