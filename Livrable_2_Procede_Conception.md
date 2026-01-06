# LIVRABLE 2 : Conception du Chapeau - Procede de Mise en Oeuvre

## 2.1 Analyse comparative des familles de procedes

| Critere | Fonderie (Gravity Die) | Forgeage (Hot Closed Die) | Metaux en feuilles (Deep Drawing) | Additif (SLM) |
|---------|------------------------|---------------------------|-----------------------------------|---------------|
| **Forme 3D creuse** | Oui | Non (solide uniquement) | Limite (forme emboutie) | Oui |
| **Rugosite brute** | 3.4 - 6.3 um | 3.2 - 12.5 um | 0.8 - 3.2 um | Variable |
| **Tolerance** | 0.25 - 2 mm | 0.4 - 2 mm | 0.2 - 0.5 mm | Bonne |
| **Cout/piece (1000 pcs)** | 22.9 - 51 EUR | 27.4 - 50.5 EUR | 18.5 - 38.1 EUR | 103 - 3790 EUR |
| **Batch economique** | 1 000 - 100 000 | 100 - 10 000 000 | 1 000 - 100 000 | 1 - 10 |
| **Materiaux** | Al, Cu, Mg, Zn, Fonte | Acier, Al, Cu | Toles ductiles | Poudres metalliques |

---

## 2.2 Procede retenu : FONDERIE - Coulee en coquille par gravite

### Gravity Die Casting

**Principe :** Le metal en fusion est coule par gravite dans un moule metallique permanent (coquille) ou il se solidifie. Le moule est ensuite ouvert et la piece demoulee.

### Justification du choix :

1. **Geometrie adaptee** : Le chapeau est une piece 3D creuse avec un alesage central - la fonderie permet d'obtenir cette forme directement avec un noyau

2. **Rugosite compatible** : La rugosite brute (3.4-6.3 um) est proche des exigences des surfaces fonctionnelles, minimisant les operations d'usinage

3. **Cout optimal** : Pour une production de moyenne serie (1000-10000 pieces), la fonderie en coquille offre un bon compromis cout/qualite

4. **Materiau** : Compatible avec les alliages d'aluminium, offrant legerete et resistance a la corrosion

### Pourquoi pas les autres procedes :

| Procede | Raison du rejet |
|---------|-----------------|
| **Forgeage** | Ne permet pas les formes creuses, necessiterait un usinage complet de l'alesage |
| **Deep drawing** | Limite aux formes cylindriques simples type "gobelet", pas adapte a une bride avec trous |
| **SLM** | Cout prohibitif (100-3000 EUR/piece), reserve au prototypage ou petites series |

---

## 2.3 Caracteristiques du procede (source GRANTA EDUPACK)

| Parametre | Valeur |
|-----------|--------|
| Masse piece | 0.5 - 50 kg |
| Epaisseur paroi | 5 - 45 mm |
| Tolerance | 0.25 - 2 mm |
| Rugosite | 3.4 - 6.3 um |
| Batch economique | 1 000 - 100 000 pieces |
| Cout outillage | 4 810 - 19 300 EUR |
| Cadence | 5 - 50 pieces/heure |

---

## 2.4 Regles de conception pour la fonderie en coquille

| Parametre | Valeur recommandee | Application au chapeau |
|-----------|-------------------|----------------------|
| **Epaisseur de paroi** | 5 - 45 mm | 8-10 mm uniforme |
| **Depouilles** | 5 - 10 degres | 5 degres sur surfaces demoulees |
| **Rayons de raccordement** | R >= 3 mm | R = 3 mm mini aux angles |
| **Surepaisseur usinage** | 1.5 - 2 mm | Sur S1, S2, S3 |
| **Plan de joint** | Au diametre max | Plan horizontal au niveau de la bride |

---

## 2.5 Conception du chapeau brut de fonderie

### Modifications par rapport a la piece finie :

- Ajout de depouilles 5 degres sur les parois verticales
- Surepaisseurs de 1.5 mm sur les surfaces a usiner (S1, S2, S3)
- Rayons de raccordement R3 minimum
- Noyau metallique pour realiser l'alesage central
- Masselottes pour alimentation en metal liquide

### Schema du brut vs piece finie :

```
BRUT DE FONDERIE                    PIECE FINIE

   _______________                    _______________
  /               \                  |               |
 /   Depouille     \                 |               |
|    5 deg          |                |               |
|                   |                |               |
|   ___________     |                |   _________   |
|  |           |    |      =>        |  |         |  |
|  | Surepaiss.|    |   USINAGE      |  | Alesage |  |
|  |  +1.5mm   |    |                |  |  fini   |  |
|  |___________|    |                |  |_________|  |
|___________________|                |_______________|
```

---

**Document realise dans le cadre du TD Design for Manufacturing - ESILV**
