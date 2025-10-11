# L09 – Funktioner (del II)

## Del 1 - Repetitionsuppgifter

### 1.1 – Temperaturmätning med `TMP36`
Rumstemperaturen kan mätas med temperatursensor `TMP36` enligt funktionen:

```math
f(x)=100x-50,
```

där
* $x$ är inspänningen i $V$ (Volt),
* $f(x)$ är rumstemperaturen i $°C$ (grader Celsius).

Anta att temperatursensorn är ansluten till mikroprocessorn `ATmega328P` med en matningsspänning på $5 V$.

**a)** Bestäm funktionens definitionsmängd i $V$.\
**b)** Beräkna funktionens värdemängd i $°C$.\
**c)** Rita grafen till funktionen.\
**d)** Beräkna inspänningen när rumstemperaturen är $30 °C$.\
**e)** Mikroprocessorns `ADC` (AD-omvandlare) har en upplösning på $10$ bitar, vilket innebär att inspänningen $0-5 V$ omvandlas till ett värde mellan $0-2^10-1$ = $0-1023$.\
Vilken temperatur motsvarar en ADC-avläsning på $205$?

### 1.2 – Datamängdens tillväxt i ett maskininlärningsprojekt
Antalet träningsdatapunkter i ett pågående maskininlärningsprojekt växer över tid när systemet samlar in fler exempel från användare och sensorer.\
Antalet datapunkter $f(x)$ efter $x$ år kan beskrivas av en exponentialfunktion:

```math
f(x)=C*a^x,
```

där 
* $C$ = startstorleken på datamängden,
* $a$ = den årliga tillväxtfaktorn,
* $x$ = antal år som passerat.

Anta att startstorleken är $6 000 000$ datapunkter och att den årliga tillväxten är $3 %$.

**a)** Ange en funktion som beskriver datamängdens storlek $f(x)$ efter $x$ år.\
**b)** Beräkna datamängdens storlek efter fem år.\
**c)** Bestäm funktionens definitionsmängd och värdemängd för tidsintervallet $0–20$ år.\
**d)** Efter hur många år har datamängden fördubblats?

## Del 2 - Nytt stoff

### 2.1 - Exponentialfunktion

Anta att en exponentialfunktion har ekvationen  

```math
f(x) = 0,5e^{x} - 0,25
```

med definitionsmängden $-2 <= x <= 2$.

**a)** Beräkna $f(0)$.\
**b)** Beräkna funktionens värdemängd.\
**c)** Bestäm för vilket värde på $x$ som $f(x) = 0$.

### 2.2 - Polynomfunktion

En polynomfunktion är given som  

```math
f(x) = 2x^2 - 4
```

med definitionsmängden $-2 <= x <= 2$.

**a)** Beräkna följande värden via ovanstående ekvation:

* $f(-2)$
* $f(-1)$
* $f(0)$
* $f(1)$
* $f(2)$

**b)** Rita funktionens graf utefter de beräknade värdena i $a)$.  

**c)** Beräkna för vilka värden på $x$ som $f(x) = 10$.

### 2.3 - Rationellt uttryck

Förenkla uttrycket och ange de $x$-värden som inte är tillåtna:

```math
f(x) = \frac{x^2 - 9}{x^2 - 2x - 15}
```

**Tips**: Faktorisera både täljare och nämnare innan du förkortar.
