# Python-programmering

Et sett med Python-løsninger på fem oppgaver, fra algoritmer til en full dataanalyse med pandas og visualiseringer. Alt ligger i én Jupyter-notatbok.

## Innhold

Se [`python_programming.ipynb`](python_programming.ipynb). Hver oppgave har forklaringer i markdown før og etter koden.

| Oppgave | Tema | Hva den viser |
|------|-------|---------------|
| 1 | **Supernacci-følgen** | En iterativ (ikke rekursiv) tallfølge bygget med listeutsnitt (slicing) |
| 2 | **Feilsøk terningspillet** | Finne og rette 10 feil i et program som ikke virker, med forklaring av hver feil |
| 3 | **Ordbøker og geografi** | Finne nærmeste by eller interessepunkt, bygrenser, og fordele og rangere interessepunkter med `min()`/`sorted()` og lambdaer |
| 4 | **Spor i NumPy** | Regne ut sporet til en matrise med en sjekk for kvadratisk matrise, kontrollert mot `np.trace()` |
| 5 | **Karakterstatistikk fra Udir** | Laste inn, rydde og analysere ekte karakterdata fra videregående skoler i Oslo |

## Høydepunkt: Oppgave 5, analyse av karakterer i Oslo

Med ekte karakterdata fra Udir (Oslo, 2024–25) gjør notatboken følgende:

- Laster inn en rotete tabulatorseparert eksport i UTF-16, filtrerer på Oslo, gir kolonnene nye navn og gjør om norske desimalkomma til tall
- Lager tre visualiseringer: snittkarakter per vurderingsform, et boksplott av fordelingen og de 10 skolene med høyest standpunktkarakter
- Svarer på et forskningsspørsmål: **følger skolene i Oslo det nasjonale mønsteret der muntlig > standpunkt > skriftlig eksamen?** (det gjør de: 4,34 > 4,09 > 3,51)
- Rangerer skolene etter forskjellen mellom standpunkt og skriftlig eksamen, og drøfter hva forskjellen betyr, med ærlige forbehold om fagsammensetning, utvalgsstørrelse og data fra bare ett år

## Teknologi

Python · Jupyter · NumPy · pandas · matplotlib · seaborn

## Kjøre den

```bash
pip install numpy pandas matplotlib seaborn jupyter
jupyter notebook python_programming.ipynb
```

Oppgave 5 forventer CSV-filen fra Udir i en `data/`-mappe ved siden av notatboken. Hvordan du laster den ned, står beskrevet i selve notatboken.
