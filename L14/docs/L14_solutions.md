# L14 - Lösningsförslag till övningsuppgifter

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

---

### Lösning

**a)** Sätt $x$ = $100{\pi}t + \frac{\pi}{4}$. Då gäller att

```math
u(t) = 5sin(x)
```

samt att

```math
u'(t) = 5cos(x) * x'
```

Vidare gäller att

```math
x' = 100{\pi}t + \frac{\pi}{4} = 100{\pi}
```

Därmed gäller att:

```math
u'(t) = 5cos(100{\pi}t + \frac{\pi}{4}) \cdot 100{\pi},
```

vilket kan skrivas om till

```math
u'(t) = 500{\pi}cos(100{\pi}t + \frac{\pi}{4})
```

***Notering***: Här användes den så kallade inre derivatan för deriveringen. Vi kommer gå
igenom detta mer djupgående idag.

**b)** $t = 0,05$ $s$ i uttrycket för $u'(t)', dvs. vi bestämmer $u'(0,05)$:

```math
u'(t) = 500{\pi}cos(100{\pi} * 0,05 + \frac{\pi}{4}) \approx -1170,7\,V/s
```

Spänningsförändringen efter $50$ $ms$ uppgår alltså till ungefär $-1170,7$ $V/s$.

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

### Lösning

**a)** Vi börjar med uttrycket för effekten:

```math
p(t) = u(t) \cdot i(t) = (U_0 e^{-t/RC}) \cdot (\frac{U_0}{R} e^{-t/RC}),
```

vilket kan skrivas som

```math
p(t) = \frac{U_0^2}{R} \cdot e^{-2t/RC}
```

**b)** Vi bestämmer $p'(t)$ med produktregeln:

```math
p'(t) = (\frac{U_0^2}{R})' \cdot e^{-2t/RC} + \frac{U_0^2}{R} \cdot (e^{-2t/RC})',
```

där

```math
(\frac{U_0^2}{R})' = 0
```

samt 

```math
(e^{-2t/RC})' = -\frac{2}{RC} * e^{-2t/RC}
```

Därmed gäller att

```math
p'(t) = 0 \cdot e^{-2t/RC} + \frac{U_0^2}{R} \cdot (-\frac{2}{RC}) \cdot e^{-2t/RC},
```

vilket kan skrivas om till

```math
p'(t) = -\frac{2U_0^2}{R^2C} \cdot e^{-2t/RC},
```

**c)** Vi börjar med att beräkna effekten vid tiden $t = 0$, dvs. $p(0)$:

```math
p(0) = \frac{U_0^2}{R} \cdot e^{-2*0/RC},
```

där

```math
e^{-2*0/RC} = e^{0} = 1, 
```

vilket innebär att

```math
p(0) = \frac{U_0^2}{R} \cdot 1 = \frac{U_0^2}{R}
```

Vi bestämmer sedan ifall effekten ökar eller minskar i denna punkt genom att beräkna $p'(0)$:

```math
p'(0) = -\frac{2U_0^2}{R^2C} \cdot e^{-2*0/RC},
```

där

```math
e^{-2*0/RC} = e^{0} = 1, 
```

vilket innebär att

```math
p'(0) = -\frac{2U_0^2}{R^2C} \cdot 1 = -\frac{2U_0^2}{R^2C}
```

Förutsatt att $U_0 > 0$ gäller då att effektiven minskar, då

```math
p'(0) = -\frac{2U_0^2}{R^2C} < 0\,\text{då}\,U_0 > 0
```

Vid tiden $t = 0$ är kondensatorn alltså fulladdad, men är i full gång att urladdas.

Vi beräknar sedan effekten när tiden $t$ går mot oändligheten, dvs. $p(\infty)$:

```math
p(0) = \frac{U_0^2}{R} \cdot e^{-2*\infty/RC},
```

där

```math
e^{-2*\infty/RC} \approx 0,
```

vilket innebär att

```math
p(\infty) \approx \frac{U_0^2}{R} \cdot 0 = 0
```

Vi bestämmer sedan ifall effekten ökar eller minskar i denna punkt genom att beräkna $p'(\infty)$:

```math
p'(\infty) = -\frac{2U_0^2}{R^2C} \cdot e^{-2*\infty/RC},
```

där

```math
e^{-2*\infty/RC} \approx 0,
```

vilket innebär att

```math
p'(\infty) \approx -\frac{2U_0^2}{R^2C} \cdot 0 = 0
```

Effekten upphör att minska när tiden $t$ går mot oändligheten, vilket beror på att kondensatorn är urladdad.

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

### Lösning

**2.2** Vi deriverar $i(t)$ med kvotregeln:

```math
i'(t) = \dfrac{u'v - u v'}{v^2} 
      = \dfrac{0\cdot v - U_0 \cdot (R_0 \alpha e^{\alpha t})}{(R_0 e^{\alpha t})^2} 
      = -\,\dfrac{U_0 \alpha}{R_0}\, e^{-\alpha t}.

```

Eftersom $\alpha > 0$ är $i'(t) < 0$ för alla värden på $t$, vilket indikerar att strömmen minskar över tid.

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
**b)** Undersök vad som händer med $i'(t)$ när $t \to 0$ och $t \to \infty$. Tolka resultatet fysiskt.

---

### Lösning

Sätt 

```math
f(x)=\ln x
```

samt 

```math
g(t)=1+e^{t/RC}
```

Då gäller att 

```math
i(t)=f(g(t))
```

samt att

```math
i'(t) = f'(g(t)) \cdot g'(t)
```

Vi deriverar $(f(x))$ samt $g(t)$:

```math
f'(x) = (ln x)' = \frac{1}{x}
```

```math
g'(t) = (1+e^{t/RC})' = \frac{1}{RC} \cdot e^{t/RC}
```

Vidare gäller att

```math
f'(g(t)) = \frac{1}{g(t)} = \frac{1}{1+e^{t/RC}}
```

Vi använder sedan kedjeregeln:

```math
i'(t) = f'(g(t)) \cdot g'(t) = \frac{1}{1+e^{t/RC}} \cdot \frac{1}{RC} \cdot e^{t/RC},
```

vilket kan utvecklas till

```math
i'(t) = \frac{e^{t/RC}}{RC(1+e^{t/RC})}
```

Vi undersöker sedan $i'(0)$ samt $i'(\infty)$:

```math
i'(0) = \frac{e^{0/RC}}{RC(1+e^{0/RC})} = \frac{1}{RC(1+1)} = \frac{1}{2RC}
```

```math
i'(\infty) = \frac{e^{\infty/RC}}{RC(1+e^{\infty/RC})},
```

där

```math
e^{\infty/RC} => \infty,
```

vilket innebär att

```math
i'(\infty) = \frac{e^{\infty/RC}}{RC(1+e^{\infty/RC})} \approx \frac{\infty}{RC \cdot \infty} = \frac{1}{RC}
```

Strömförändingen ökar från $\frac{1}{2RC}$ till $\frac{1}{RC}$ och stabiliseras sedan. Detta indikerar att
strömförändringen inte avtar, utan når ett konstant värde över tid.

---