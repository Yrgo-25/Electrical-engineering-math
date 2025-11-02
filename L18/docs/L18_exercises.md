# L18 - Lektionsuppgifter

## Del 1 - Repetitionsuppgifter

### 1.1 - Vektorer i det komplexa talplanet

Du har följande vektorer: $a = (2;1)$, $b = (2;-1)$ samt $c = (-3, 4)$. \
I uppgifterna nedan ska varje vektor $(x;y)$ tolkas som ett komplext tal $z = x + jy$.

**a)** Skriv vektorerna på komplex rektangulär form.\
**b)** Rita ut vektorerna i det komplexa talplanet (x-axeln = reell del, y-axeln = imaginär del).\
**c)** Bestäm vektorernas längder, dvs. absolutbeloppet av respektive tal.\
**d)** Bestäm längden (absolutbeloppet) av $a + b + c$, dvs. $|a + b + c|$.\
**e)** Bestäm vektorernas vinklar.\
**f)** Bestäm en vektor $d$ med längden $8$ som är motsatt riktad $c$.

---

### 1.2 - Eulers form => rektangulär form

En ström $i(t)$ i en växelströmskrets skrivs på Eulers form enligt nedan:

```math
i(t) = 2e^{j(100πt + \frac{π}{6})}\,mA,
```

där t= tiden i sekunder.

**a)** Skriv om $i(t)$ till rektangulär form via Eulers formel.\
**b)** Beräkna strömmens värde vid tiden $t = 5$ $ms$, dvs. $i(0,005)$.\
**c)** Rita ut strömmens värde vid tiden tiden $t = 5$ $ms$ i det komplexa talplanet (x-axeln = reell del, y-axeln = imaginär del).

---

### 1.3 - Rektangulär form => Eulers form

En spänning $u(t)$ i en växelströmskrets skrivs på rektangulär form enligt nedan:

```math
u(t) = 3 - j6 V
```

**a)** Rita ut spänningen i det komplexa talplanet (x-axeln = reell del, y-axeln = imaginär del).\
**b)** Uttryck spänningen på Eulers form, dvs. bestäm absolutbeloppet $|U|$ samt fasvinkeln $δ$ så att $U = |U|e^{jδ}$.\
**c)** Anta att strömmens frekvens $f = 50$ $Hz$. Bestäm vinkelhastigheten $w$.\
**d)** Skriv $u(t)$ som en tidsberoende funktion $u(t)=|U|*e^(j(wt+δ))$.

---

## Del 2 - Nytt stoff

### 2.1 - Addition av tre strömmar i AC-krets

En nod i en elektrisk krets matas med tre sinusformade strömmar: 

```math
i_1(t) = 5{\sin (\omega t + 30^{\circ})}\,\,mA
```

```math
i_2(t) = 3{\sin (\omega t - 30^{\circ})}\,\,mA
```

```math
i_3(t) = 4{\sin (\omega t + 120^{\circ})}\,\,mA
```

Den totala strömmen i kretsen $I_{tot}$ beräknas enligt nedan:

```math
I_{tot}(t) = i_1(t) + i_2(t) + i_3(t)
```

**a)** Skriv om strömmarna $i_1(t)$, $i_2(t)$ samt $i_3(t)$ till fasor $I_1$, $I_2$ samt $I_3$ i komplex rektangulär form.\
**b)** Beräkna fasorsumman $I_{tot} = I_1 + I_2 + I_3$.\
**c)** Omvandla tillbaka resultatet till en sinusformad ström i tidsdomänen på följande form:

```math
i_{tot}(t) = |I_{tot}|{\sin}(\omega t + δ)
```

---