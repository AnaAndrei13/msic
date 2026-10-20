# MSIC – Proiect semestrial

> **Template repository** pentru disciplina **MSIC**.
> Apăsați **„Use this template” → „Create a new repository”** pentru a porni propriul proiect.

---

## 👤 Date student / echipă

| Câmp | Valoare |
|---|---|
| Nume și prenume | _completați_ |
| Grupa | _completați_ |
| An universitar | 2026–2027 |
| Cadru didactic | _completați_ |
| Varianta aleasă | ☐ **A** – Proiect existent ☐ **B** – Dezvoltarea unui proiect |
| Limbaj / tehnologii | _ex. Java 21, Python 3.12, C#/.NET 8_ |
| Link proiect original (doar Varianta A) | _URL_ |

---

## 📌 Descrierea proiectului

_Descrieți pe scurt aplicația: scop, utilizatori, funcționalități principale._

---

## 🗂️ Structura repository-ului

```
.
├── README.md                     ← acest fișier (prezentare generală)
├── src/                          ← codul sursă al aplicației
├── evaluare-1-metrici/           ← Evaluarea intermediară I
│   ├── README.md
│   ├── metrici.md                ← tabelul cu metrici și valori
│   └── rapoarte/                 ← exporturi din instrumente (CSV, HTML, capturi)
├── evaluare-2/                   ← Evaluarea intermediară II
│   ├── README.md
│   └── rapoarte/
├── evaluare-3/                   ← Evaluarea intermediară III
│   ├── README.md
│   └── rapoarte/
├── prezentare-finala/            ← Evaluarea finală (sesiunea de iarnă)
│   ├── README.md
│   ├── raport-template.md        ← schelet pentru raportul PDF
│   └── raport.pdf                ← raportul final (de adăugat)
└── .github/
    └── pull_request_template.md
```

---

## 🧭 Variante de proiect

| Etapă | Varianta A – Proiect existent | Varianta B – Dezvoltarea unui proiect |
|---|---|---|
| **Evaluare I** | Set de **minim 10 metrici** referitoare la **codul sursă** + determinarea valorilor | Set de **minim 10 metrici** referitoare la **proiectarea orientată pe obiecte** + determinarea valorilor |
| **Evaluare II** | **Refactorizarea** codului sursă astfel încât toate metricile să fie în plaja de valori admise | **Scrierea codului sursă** și prezentarea funcționalității aplicației |
| **Evaluare III** | Adăugarea a **cel puțin 3 funcționalități noi** (agreate cu cadrul didactic), cu metricile în plaja admisă | Scrierea codului sursă și prezentarea **funcționalităților finale** ale aplicației |
| **Evaluare finală** | Raport PDF + prezentarea funcționalității aplicației | Raport PDF + prezentarea funcționalității aplicației |

Detalii pentru fiecare etapă se găsesc în README-ul din folderul corespunzător.

---

## ✅ Progres

| Etapă | Folder | Termen | Status | Tag Git |
|---|---|---|---|---|
| Evaluare intermediară I | [`evaluare-1-metrici/`](evaluare-1-metrici/) | _dd.mm.yyyy_ | ⬜ | `eval-1` |
| Evaluare intermediară II | [`evaluare-2/`](evaluare-2/) | _dd.mm.yyyy_ | ⬜ | `eval-2` |
| Evaluare intermediară III | [`evaluare-3/`](evaluare-3/) | _dd.mm.yyyy_ | ⬜ | `eval-3` |
| Evaluare finală | [`prezentare-finala/`](prezentare-finala/) | sesiunea de iarnă | ⬜ | `final` |

Legendă: ⬜ neînceput · 🟨 în lucru · ✅ predat

---

## 🏷️ Convenții de lucru

- Fiecare etapă predată se marchează cu un **tag Git**, ca valorile metricilor să poată fi comparate între versiuni:
  ```bash
  git tag -a eval-1 -m "Evaluare intermediara I"
  git push origin eval-1
  ```
- Rapoartele generate de instrumente (CSV, HTML, JSON, capturi de ecran) se salvează în subfolderul `rapoarte/` al etapei.
- Mesajele de commit sunt descriptive (ex. `refactor: extrage metoda validateOrder din OrderService`).
- Pentru Varianta A, păstrați un commit inițial cu **codul original nemodificat** (tag `original`).

---

## ▶️ Rulare aplicație

```bash
# completați comenzile de build / rulare
```

---

## 📄 Licență

_Completați (ex. MIT) sau respectați licența proiectului original pentru Varianta A._
