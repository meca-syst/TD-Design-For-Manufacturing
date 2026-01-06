# LIVRABLE 7 : Encadrement du Cout par Piece

## 7.1 Lecture des courbes GRANTA EDUPACK

### Source : Fiche "Cout - Gravity Die Casting"

### Parametres de reference :
- Masse piece : 1 kg
- Cout matiere : 6.81 EUR/kg
- Overhead rate : 128 EUR/h
- Capital write-off : 5 ans
- Load factor : 0.5

---

## 7.2 Cout relatif par piece (reference 1 kg)

| Taille de lot | Cout min (EUR) | Cout max (EUR) |
|---------------|----------------|----------------|
| 1 | ~10 000 | ~30 000 |
| 10 | ~2 000 | ~5 000 |
| 100 | ~200 | ~600 |
| **1 000** | **22.9** | **51** |
| 10 000 | ~15 | ~35 |
| 100 000 | ~12 | ~28 |
| 1 000 000 | ~10 | ~25 |

---

## 7.3 Adaptation a notre piece

### Hypotheses pour le chapeau :

| Parametre | Valeur |
|-----------|--------|
| Masse estimee | **0.5 kg** |
| Materiau | AS7G (AlSi7Mg) |
| Cout matiere aluminium | ~7 EUR/kg |

### Correction pour masse 0.5 kg :

Le cout matiere represente environ 20-30% du cout total.

Pour une piece de 0.5 kg au lieu de 1 kg :

**Facteur de correction : ~0.85** (reduction du cout matiere)

---

## 7.4 Encadrement du cout - FONDERIE seule (brut)

| Taille de lot | Cout min (EUR) | Cout max (EUR) |
|---------------|----------------|----------------|
| 100 | 170 | 510 |
| 500 | 50 | 120 |
| **1 000** | **19** | **43** |
| 5 000 | 14 | 32 |
| **10 000** | **13** | **30** |
| 100 000 | 10 | 24 |

---

## 7.5 Cout total (Fonderie + Usinage secondaire)

### Decomposition par poste :

| Poste | Cout min (EUR) | Cout max (EUR) | Justification |
|-------|----------------|----------------|---------------|
| Brut fonderie (1000 pcs) | 19 | 43 | Courbe GRANTA |
| Tournage (S1, S2, S4) | 8 | 15 | 5-8 min x 100 EUR/h |
| Fraisage (S3) | 3 | 6 | 2-3 min x 100 EUR/h |
| Percage (S5) | 2 | 4 | 2-3 min x 100 EUR/h |
| Rectification (S3, optionnel) | 3 | 8 | 3-5 min x 100 EUR/h |
| Controle | 2 | 4 | 2 min |
| **TOTAL (sans rectification)** | **34** | **72** | |
| **TOTAL (avec rectification)** | **37** | **80** | |

---

## 7.6 Synthese - Encadrement du cout

### Pour une production de 1 000 pieces :

| Scenario | Cout/piece |
|----------|-----------|
| **Estimation basse** | **34 EUR** |
| **Estimation haute** | **80 EUR** |
| **Estimation moyenne** | **~50 EUR** |

### Pour une production de 10 000 pieces :

| Scenario | Cout/piece |
|----------|-----------|
| **Estimation basse** | **28 EUR** |
| **Estimation haute** | **60 EUR** |
| **Estimation moyenne** | **~40 EUR** |

---

## 7.7 Graphique recapitulatif

```
Cout/piece (EUR)
    |
500 +  *
    |    *
200 +      *
    |        *
100 +          *
 80 +............*..............................  Estimation haute
    |              *
 50 +                *  *  *  *  *  *  *  *      Estimation moyenne
    |                    *
 34 +....................*......................  Estimation basse
    |                        *  *  *  *  *  *
 20 +
    |
    +----+----+----+----+----+----+----+----+--> Quantite
        100  500  1k   2k   5k  10k  50k 100k
```

---

## 7.8 Tableau recapitulatif final

| Quantite | Cout FONDERIE brut | Cout USINAGE | **Cout TOTAL** |
|----------|-------------------|--------------|----------------|
| 500 | 50-120 EUR | 15-30 EUR | **65-150 EUR** |
| **1 000** | 19-43 EUR | 15-30 EUR | **34-80 EUR** |
| 5 000 | 14-32 EUR | 15-30 EUR | **29-62 EUR** |
| **10 000** | 13-30 EUR | 15-30 EUR | **28-60 EUR** |
| 100 000 | 10-24 EUR | 15-30 EUR | **25-54 EUR** |

---

## 7.9 Conclusion

### Encadrement du cout par piece pour le chapeau en fonderie coquille :

| Quantite | Cout minimum | Cout maximum |
|----------|--------------|--------------|
| **1 000 pieces** | **34 EUR** | **80 EUR** |
| **10 000 pieces** | **28 EUR** | **60 EUR** |

### Cout moyen estime : **40-50 EUR/piece**

Pour une production de 1 000 a 10 000 pieces.

---

**Document realise dans le cadre du TD Design for Manufacturing - ESILV**
