# LIVRABLE 6 : Quantite a Produire pour etre Rentable

## 6.1 Donnees economiques du procede

### Source : GRANTA EDUPACK - Gravity Die Casting

| Parametre | Valeur min | Valeur max | Unite |
|-----------|------------|------------|-------|
| Cout capital (machine) | 16 000 | 64 200 | EUR |
| Cout outillage (coquille) | 4 810 | 19 300 | EUR |
| Duree de vie outillage | 10 000 | 100 000 | pieces |
| Cadence de production | 5 | 50 | pieces/h |
| Taux utilisation matiere | 60 | 80 | % |
| Batch economique | 1 000 | 100 000 | pieces |

---

## 6.2 Hypotheses de calcul

| Parametre | Valeur retenue |
|-----------|----------------|
| Masse piece | 0.5 kg |
| Cout matiere (AS7G) | 7 EUR/kg |
| Cout outillage moyen | 12 000 EUR |
| Cout horaire machine | 60 EUR/h |
| Cadence moyenne | 20 pieces/h |
| Cout usinage/piece | 15 EUR |

---

## 6.3 Decomposition du cout par piece

### Formule :

**Cout piece = Cout matiere + Cout fonderie + Cout usinage + (Cout outillage / Nb pieces)**

### Calcul :

| Poste | Calcul | Valeur |
|-------|--------|--------|
| Cout matiere | 0.5 kg x 7 EUR/kg | 3.50 EUR |
| Cout fonderie | 60 EUR/h / 20 pcs/h | 3.00 EUR |
| Cout usinage | forfait | 15.00 EUR |
| **Sous-total (hors outillage)** | | **21.50 EUR** |

---

## 6.4 Evolution du cout selon la quantite

| Quantite | Cout matiere | Cout fonderie | Cout usinage | Amortissement outillage | **Cout total/piece** |
|----------|--------------|---------------|--------------|------------------------|---------------------|
| 100 | 3.50 EUR | 3.00 EUR | 15 EUR | 120.00 EUR | **141.50 EUR** |
| 200 | 3.50 EUR | 3.00 EUR | 15 EUR | 60.00 EUR | **81.50 EUR** |
| 500 | 3.50 EUR | 3.00 EUR | 15 EUR | 24.00 EUR | **45.50 EUR** |
| 1 000 | 3.50 EUR | 3.00 EUR | 15 EUR | 12.00 EUR | **33.50 EUR** |
| 2 000 | 3.50 EUR | 3.00 EUR | 15 EUR | 6.00 EUR | **27.50 EUR** |
| 5 000 | 3.50 EUR | 3.00 EUR | 15 EUR | 2.40 EUR | **23.90 EUR** |
| 10 000 | 3.50 EUR | 3.00 EUR | 15 EUR | 1.20 EUR | **22.70 EUR** |
| 50 000 | 3.50 EUR | 3.00 EUR | 15 EUR | 0.24 EUR | **21.74 EUR** |

---

## 6.5 Comparaison avec l'usinage complet

Pour une piece usinee a partir d'un brut cylindrique (sans fonderie) :

| Poste | Cout |
|-------|------|
| Cout matiere brut | 8 EUR |
| Cout usinage complet | 60-80 EUR |
| **Cout total usinage** | **68-88 EUR/piece** |

**Ce cout est constant quelle que soit la quantite** (pas d'outillage specifique).

---

## 6.6 Determination du seuil de rentabilite

### Point d'equilibre Fonderie vs Usinage :

- Cout usinage complet : **~75 EUR/piece** (constant)
- Cout fonderie : **diminue avec la quantite**

### Calcul :

```
Cout fonderie = Cout usinage complet

21.5 + (12000 / N) = 75

12000 / N = 53.5

N = 12000 / 53.5

N = 224 pieces
```

**Seuil de rentabilite theorique : 224 pieces**

---

## 6.7 Graphique comparatif

```
Cout/piece (EUR)
     |
 150 +  *
     |    \
 100 +      *
     |        \
  75 +----------*-----------------------  Usinage complet
     |            \
  50 +              *
     |                *
  33 +                  *-----------     Fonderie + usinage
     |                      *  *  *
  21 +................................   Cout mini (hors outillage)
     |
     +----+----+----+----+----+----+---> Quantite
         100  200  500  1k   5k  10k
```

---

## 6.8 Conclusion

### Recommandation :

| Quantite | Procede recommande | Cout/piece estime |
|----------|-------------------|-------------------|
| < 200 pieces | Usinage complet | ~75 EUR |
| 200 - 500 pieces | Zone de transition | 45-75 EUR |
| 500 - 1000 pieces | Fonderie + usinage | 33-45 EUR |
| > 1000 pieces | **Fonderie + usinage** | < 33 EUR |

### Quantite minimale rentable : **500 pieces**

A partir de 500 pieces, la fonderie en coquille devient clairement avantageuse par rapport a l'usinage complet.

### Quantite optimale : **1 000 - 10 000 pieces**

Cette plage correspond au batch economique du procede et permet un cout par piece de **22 - 33 EUR**.

---

**Document realise dans le cadre du TD Design for Manufacturing - ESILV**
