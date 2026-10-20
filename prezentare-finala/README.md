# Evaluarea finală

⬅️ [Înapoi la README-ul general](../README.md)

## 🎯 Cerință

Evaluarea finală se face **în timpul examenului, în sesiunea de iarnă**, și presupune:

1. **Realizarea unui raport (în format PDF)** cu:
   - descrierea **metricilor utilizate**;
   - descrierea **instrumentelor folosite** pentru determinarea acestora;
   - evidențierea **metricilor care au necesitat refactorizarea codului / re-proiectarea orientată pe obiecte**.
2. **Prezentarea funcționalității aplicației.**

## 📦 Ce trebuie predat

- [ ] `raport.pdf` în acest folder (pornind de la [`raport-template.md`](raport-template.md))
- [ ] Aplicația în stare de rulare (instrucțiuni în [README-ul general](../README.md#️-rulare-aplicație))
- [ ] Tabelul de evoluție a metricilor complet în [`metrici.md`](../evaluare-1-metrici/metrici.md#4-evoluția-valorilor-între-etape)
- [ ] Toate tag-urile prezente: `eval-1`, `eval-2`, `eval-3`, `final` (+ `original` pentru Varianta A)
- [ ] Opțional: scurtă înregistrare demo în `demo/` sau link în acest README

## 📝 Generarea raportului PDF

Completați [`raport-template.md`](raport-template.md), apoi convertiți-l, de exemplu cu Pandoc:

```bash
cd prezentare-finala
pandoc raport-template.md -o raport.pdf \
  --pdf-engine=xelatex -V geometry:margin=2.5cm -V mainfont="DejaVu Serif" \
  --toc --number-sections
```

Alternativ: Word / LibreOffice / Overleaf → *Export as PDF*.

## ✅ Checklist pentru ziua examenului

- [ ] Aplicația pornește pe laptop fără configurare suplimentară
- [ ] Date de test pregătite pentru demo
- [ ] Raportul PDF descărcat local și urcat în repository
- [ ] Rapoartele instrumentelor pot fi regenerate live (comenzi pregătite)
- [ ] Pot explica fiecare metrică: definiție, plajă, de ce a fost aleasă

## 🔗 Demo

_Link înregistrare / capturi de ecran (opțional)._
