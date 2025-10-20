# L14 - Lektionsuppgifter

## Del 1 - Repetitionsuppgifter

### 1.1 - Ström genom en spole

Spänningsfallet över genom en kondensator varierar över tid enligt följande funktion:

```math
u(t) = 5sin(100{\pi}t + \frac{\pi}{4})
```

där
* $u(t)$ = spänningsfallet över kondensatorn i $V$,
* $t$ = tiden i sekunder.

**a)** Derivera funktionen.\
**b)** Beräkna $u'(t)$ vid tiden $t = 50$ $ms$.

## Del 2 - Nytt stoff

---
### 2.1 - Effekt i en RC-krets vid urladdning
En kondensator urladdas i enlighet med följande formel:

```math
u(t) = U_0 e^{-t/RC}, 
```
där
* $U_0$ = begynnelsespänningen,
* $t$ = tiden i sekunder,
* $RC$ = kretsens tidskonstant.

Strömmen genom kondensatorn kan beskrivas med följande formel:

```math
i(t) = \dfrac{U_0}{R} e^{-t/RC}  
```

Den momentana effekten $p(t)$ i kondensatorn kan beräknas med följande formel: 

```math
p(t) = u(t)*i(t)  
```

**a)** Bestäm ett uttryck för effekten $p(t)$.  
**b)** Beräkna $p'(t)$.  
**c)** Bestäm $p(t)$ i punkterna $t=0$ och $t=\infty$ samt ange om effekten ökar eller minskar i dessa punkter.

---

---
### 2.2 – Ström genom en varierande resistans

Strömmen $i(t)$ genom en resistans kan beskrivas med följande formel:

```math
i(t) = \dfrac{U_c}{R_0} \cdot e^{at},
```

där
* $U_c$ = spänningsfallet över kondensatorn,
* $R_0$ = begynnelseresistansen,
* $t$ = tiden i sekunder,
* $a$ = temperaturkoefficienten.

**a)** Beräkna $i'(t)$.  
**b)** Förenkla uttrycket och bestäm om strömmen ökar eller minskar för $a > 0$.

---

### 2.3 – Logaritmisk strömfunktion

En ström $i(t)$ beskrivs av följande formel:

```math
i(t) = \ln\!(1 + e^{t/RC})
```

där  
- $RC$ = kretsens tidskonstant, 
- $t$ = tiden i sekunder.

**a)** Bestäm $i'(t)$ med kedjeregeln.  
**b)** Undersök vad som händer med $i'(t)$ när $t \to 0$ och $t \to \infty$.

---
