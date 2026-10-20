# Evaluarea intermediară II

⬅️ [Înapoi la README-ul general](../README.md)

## 🎯 Cerință

- **Varianta A – Proiect existent:** **refactorizarea codului sursă** astfel încât **toate metricile** stabilite la prima prezentare să fie în **plaja de valori admise**.
- **Varianta B – Dezvoltarea unui proiect:** **scrierea codului sursă** și **prezentarea funcționalității** aplicației.

---

## 🅰️ Varianta A – Refactorizare

### Ce trebuie predat

- [ ] Codul refactorizat în `src/`
- [ ] Metricile re-măsurate (aceleași instrumente și setări ca la Evaluarea I), exporturi în [`rapoarte/`](rapoarte/)
- [ ] Coloana **Eval II** completată în [`../evaluare-1-metrici/metrici.md`](../evaluare-1-metrici/metrici.md#4-evoluția-valorilor-între-etape)
- [ ] Jurnalul de refactorizări (tabelul de mai jos)
- [ ] Dovada că funcționalitatea a rămas neschimbată (teste care trec înainte și după)
- [ ] Tag Git `eval-2`

### Jurnal de refactorizări

| # | Element | Metrică afectată | Valoare înainte | Valoare după | Tehnică de refactorizare | Commit |
|---|---|---|---|---|---|---|
| 1 | _ex. `OrderService.process()`_ | _CC_ | _18_ | _6_ | _Extract Method_ | _`abc123`_ |
| 2 | | | | | | |
| 3 | | | | | | |

Tehnici uzuale (Fowler): *Extract Method / Class*, *Move Method / Field*, *Replace Conditional with Polymorphism*, *Introduce Parameter Object*, *Decompose Conditional*, *Replace Magic Number with Constant*, *Remove Duplicated Code*, *Replace Temp with Query*.

### Comparație înainte / după

```bash
git diff original eval-2 --stat
```

| Metrică | Plajă | Eval I | Eval II | Status |
|---|---|---|---|---|
| | | | | ✅ / ❌ |

---

## 🅱️ Varianta B – Implementare

### Ce trebuie predat

- [ ] Codul sursă în `src/`, conform proiectării de la Evaluarea I
- [ ] Funcționalitățile implementate (lista de mai jos)
- [ ] Instrucțiuni de build și rulare în [README-ul general](../README.md#️-rulare-aplicație)
- [ ] Capturi de ecran / demo în [`rapoarte/`](rapoarte/)
- [ ] Metricile OO măsurate pe codul scris; abaterile față de proiectare explicate
- [ ] Coloana **Eval II** completată în [`metrici.md`](../evaluare-1-metrici/metrici.md#4-evoluția-valorilor-între-etape)
- [ ] Tag Git `eval-2`

### Funcționalități implementate

| # | Funcționalitate | Clase implicate | Status | Captură / demo |
|---|---|---|---|---|
| 1 | | | ✅ / 🟨 | |
| 2 | | | | |
| 3 | | | | |

### Abateri de la proiectare

| Element | Proiectat | Implementat | Motiv | Impact asupra metricilor |
|---|---|---|---|---|
| | | | | |

---

## 🎤 Structura prezentării (sugestie)

1. Recapitulare: metricile și plajele admise
2. **A:** principalele refactorizări (exemple de cod înainte/după) · **B:** arhitectura și demo
3. Tabel comparativ al metricilor Eval I → Eval II
4. Probleme rămase / plan pentru Evaluarea III
