# Evaluarea intermediară I – Stabilirea și determinarea metricilor

⬅️ [Înapoi la README-ul general](../README.md)

## 🎯 Cerință

- **Varianta A – Proiect existent:** stabilirea unui set de metrici (**minim 10 metrici**) care se referă la **codul sursă** și determinarea valorilor acestora.
- **Varianta B – Dezvoltarea unui proiect:** stabilirea unui set de metrici (**minim 10 metrici**) care se referă la **proiectarea orientată pe obiecte** și determinarea valorilor acestora.

## 📦 Ce trebuie predat

- [ ] Varianta aleasă bifată în [README-ul general](../README.md)
- [ ] [`metrici.md`](metrici.md) completat: minim 10 metrici, cu definiție, plajă admisă, valoare măsurată
- [ ] Instrumentele folosite (nume, versiune, configurare)
- [ ] Exporturile brute din instrumente în [`rapoarte/`](rapoarte/)
- [ ] Lista elementelor (clase / metode / fișiere) **în afara plajei admise**
- [ ] Varianta A: codul original în `src/`, marcat cu tag-ul `original`
- [ ] Varianta B: diagrama de clase (UML) în `rapoarte/` (ex. `diagrama-clase.png`)
- [ ] Tag Git `eval-1`

## 💡 Exemple de metrici

### Varianta A – metrici de cod sursă

| Metrică | Descriere | Plajă orientativă |
|---|---|---|
| LOC / SLOC | Linii de cod (totale / fără comentarii și linii goale) | – (informativ) |
| CLOC / densitatea comentariilor | Linii de comentariu / LOC | 15–40% |
| Complexitate ciclomatică (McCabe) | Număr de căi independente într-o metodă | ≤ 10 |
| Complexitate cognitivă | Dificultatea de înțelegere a unei metode | ≤ 15 |
| Lungimea metodei | Linii de cod pe metodă | ≤ 30–50 |
| Număr de parametri | Parametri pe metodă | ≤ 4–5 |
| Adâncimea de imbricare | Nivelul maxim de blocuri imbricate | ≤ 3–4 |
| Duplicarea codului | Procent de linii duplicate | ≤ 3–5% |
| Metricile Halstead | Volum, dificultate, efort | relativ |
| Indice de mentenabilitate (MI) | Combinație LOC + CC + Halstead | ≥ 65 (sau ≥ 20 în scala Visual Studio) |
| Lungimea fișierului / clasei | Linii pe fișier | ≤ 400–500 |
| Code smells / issues | Probleme raportate de analizorul static | 0 critice |

### Varianta B – metrici de proiectare orientată pe obiecte

| Metrică | Descriere | Plajă orientativă |
|---|---|---|
| WMC | Weighted Methods per Class (suma complexităților) | ≤ 20–50 |
| DIT | Depth of Inheritance Tree | ≤ 5 |
| NOC | Number of Children | ≤ 10 |
| CBO | Coupling Between Objects | ≤ 14 |
| RFC | Response For a Class | ≤ 50 |
| LCOM / LCOM4 | Lack of Cohesion of Methods | LCOM4 = 1 |
| MHF | Method Hiding Factor (MOOD) | 10–25% metode publice → MHF mare |
| AHF | Attribute Hiding Factor (MOOD) | ≈ 100% |
| MIF / AIF | Method / Attribute Inheritance Factor | 20–80% |
| PF / POF | Polymorphism Factor | 2–10% |
| CF | Coupling Factor (MOOD) | ≤ 12% |
| Instabilitate (I) / Abstractizare (A) | Metricile lui Robert C. Martin pe pachete | distanța D = \|A + I − 1\| ≤ 0.3 |
| NOM / NOA | Număr de metode / atribute pe clasă | ≤ 20 / ≤ 10 |

> Plajele sunt orientative și trebuie **justificate** (literatură, recomandări ale instrumentului) și **agreate cu cadrul didactic**.

## 🛠️ Instrumente sugerate

| Limbaj | Instrumente |
|---|---|
| Multi-limbaj | SonarQube / SonarCloud, `lizard`, `cloc`, PMD (CPD pentru duplicate) |
| Java | CK (`mauricioaniche/ck`), MetricsReloaded / MetricsTree (IntelliJ), JDepend, Checkstyle |
| Python | `radon` (cc, mi, raw, hal), `pylint`, `wily` (evoluție în timp) |
| C# / .NET | Visual Studio Code Metrics, NDepend |
| C / C++ | `lizard`, `cppcheck`, Understand (SciTools) |
| JavaScript / TypeScript | ESLint (reguli `complexity`, `max-depth`, `max-params`), `plato`, `escomplex` |

Exemple de comenzi:

```bash
cloc src/ --csv --out=evaluare-1-metrici/rapoarte/cloc.csv
lizard src/ --csv > evaluare-1-metrici/rapoarte/lizard.csv
radon cc src/ -s -a -j > evaluare-1-metrici/rapoarte/radon-cc.json
radon mi src/ -s -j > evaluare-1-metrici/rapoarte/radon-mi.json
java -jar ck.jar src/ true 0 false evaluare-1-metrici/rapoarte/
```

## 🎤 Structura prezentării (sugestie)

1. Proiectul ales (scop, dimensiune, tehnologii)
2. Setul de metrici: definiție + de ce a fost ales + plajă admisă
3. Instrumentele și modul de măsurare
4. Rezultate (tabel + grafice)
5. Elementele în afara plajei → plan pentru etapa următoare
