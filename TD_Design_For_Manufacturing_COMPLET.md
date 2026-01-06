# TD : DESIGN FOR MANUFACTURING
## Conception d'un chapeau de maintien de joint a levres
### Famille de procedes : FONDERIE

**ESILV - Ecole d'Ingenieurs**

---

# TABLE DES MATIERES

1. Surfaces fonctionnelles
2. Procede de mise en oeuvre
3. Gamme de fabrication
4. Procedes secondaires/tertiaires
5. Materiau retenu
6. Quantite rentable
7. Cout par piece

---

# 1. IDENTIFICATION DES SURFACES FONCTIONNELLES

## 1.1 Analyse du mecanisme

Le chapeau a pour fonction de :
- Maintenir le joint a levres en position
- Assurer l'etancheite dynamique (entre l'arbre tournant et le chapeau via le joint)
- Assurer l'etancheite statique (entre le chapeau et le carter)
- Etre fixe sur le carter par vissage

## 1.2 Surfaces fonctionnelles identifiees

| Ref | Surface | Fonction technique | Rugosite Ra |
|-----|---------|-------------------|-------------|
| **S1** | Alesage logement joint | Centrage et maintien radial du joint | **<= 3.2 um** |
| **S2** | Epaulement arriere | Appui axial du joint | **<= 3.2 um** |
| **S3** | Face contact carter | Etancheite statique | **<= 0.8 um** |
| **S4** | Face d'appui carter | Mise en position axiale | **<= 3.2 um** |
| **S5** | Trous de fixation | Assemblage par vis | **<= 6.3 um** |
| **S6** | Surfaces externes | Esthetique | **<= 12.5 um** |

## 1.3 Justifications (Annexes SKF)

- **S1** : Armature apparente metal -> Ra <= 3.2 um, Rz <= 10 um
- **S2** : "Axial faces of all grooves" -> Ra <= 3.2 um
- **S3** : Etancheite statique sous pression -> Ra <= 0.8 um
- **S4** : Surface de reference positionnement
- **S5** : Fonction passage vis, rugosite standard

---

# 2. PROCEDE DE MISE EN OEUVRE

## 2.1 Analyse comparative

| Critere | Fonderie | Forgeage | Emboutissage | Additif |
|---------|----------|----------|--------------|---------|
| Forme 3D creuse | OUI | NON | LIMITE | OUI |
| Cout (1000 pcs) | 23-51 EUR | 27-50 EUR | 18-38 EUR | 103-3790 EUR |
| Ra brut | 3.4-6.3 um | 3.2-12.5 um | 0.8-3.2 um | Variable |
| Batch economique | 1k-100k | 100-10M | 1k-100k | 1-10 |

## 2.2 Procede retenu : FONDERIE COQUILLE PAR GRAVITE

### Justification :
1. Geometrie adaptee (piece creuse avec alesage)
2. Rugosite compatible avec les exigences
3. Cout optimal en moyenne serie
4. Compatible aluminium

### Regles de conception :
- Depouilles : 5 degres
- Epaisseur uniforme : 8-10 mm
- Rayons : R >= 3 mm
- Surepaisseurs usinage : 1.5 mm

---

# 3. GAMME DE FABRICATION

| Phase | Operation | Machine | Surface |
|-------|-----------|---------|---------|
| 10 | Coulee en coquille | Machine coulee | - |
| 20 | Parachevement (sciage, ebarbage) | Scie, meuleuse | - |
| 30 | Controle brut | Poste controle | Toutes |
| 40 | Tournage (alesage, dressage) | Tour CN | S1, S2, S4 |
| 50 | Surfacage | Fraiseuse CN | S3 |
| 60 | Percage trous fixation | Fraiseuse CN | S5 |
| 70 | Rectification (optionnel) | Rectifieuse | S3 |
| 80 | Ebavurage, lavage | Manuel | Toutes |
| 90 | Controle final | MMT | S1, S2, S3 |
| 100 | Conditionnement | Manuel | - |

---

# 4. PROCEDES SECONDAIRES/TERTIAIRES

| Surface | Ra requis | Ra brut | Procede | Justification |
|---------|-----------|---------|---------|---------------|
| S1 | 3.2 um | 3.4-6.3 um | Tournage finition | Ra brut insuffisant |
| S2 | 3.2 um | 3.4-6.3 um | Tournage dressage | Planeite + Ra |
| S3 | 0.8 um | 3.4-6.3 um | Surfacage + Rectif. | Etancheite statique |
| S4 | 3.2 um | 3.4-6.3 um | Tournage dressage | Positionnement |
| S5 | 6.3 um | N/A | Percage | Non moulable |
| S6 | 12.5 um | 3.4-6.3 um | Aucun | Ra suffisant |

### Capabilites Ra par procede :
- Fonderie brut : 3.4-6.3 um
- Tournage finition : 0.8-3.2 um
- Percage : 3.2-6.3 um
- Rectification : 0.2-0.8 um

---

# 5. MATERIAU RETENU

## Alliage : AS7G (AlSi7Mg / A356 / EN AC-42100)

| Propriete | Valeur |
|-----------|--------|
| Densite | 2.68 g/cm3 |
| Limite elastique | 180-220 MPa |
| Resistance traction | 250-290 MPa |
| Durete | 75-90 HB |
| Module Young | 72 GPa |

## Justification :
1. **Coulabilite** : Excellent en fonderie coquille
2. **Usinabilite** : Tres bonne
3. **Legerete** : 3x moins que l'acier
4. **Corrosion** : Bonne resistance
5. **Cout** : 6-8 EUR/kg

---

# 6. QUANTITE RENTABLE

## Donnees economiques (GRANTA EDUPACK)

| Parametre | Valeur |
|-----------|--------|
| Cout outillage | 4 810 - 19 300 EUR |
| Batch economique | 1 000 - 100 000 pieces |
| Cadence | 5 - 50 pieces/h |

## Evolution du cout

| Quantite | Cout/piece |
|----------|------------|
| 100 | 141.50 EUR |
| 500 | 45.50 EUR |
| 1 000 | 33.50 EUR |
| 10 000 | 22.70 EUR |

## Seuil de rentabilite

**Fonderie rentable a partir de ~500 pieces**

Comparaison avec usinage complet : ~75 EUR/piece

---

# 7. COUT PAR PIECE

## Encadrement (source GRANTA EDUPACK)

### Pour 1 000 pieces :

| Poste | Cout min | Cout max |
|-------|----------|----------|
| Brut fonderie | 19 EUR | 43 EUR |
| Usinage | 15 EUR | 30 EUR |
| Controle | 2 EUR | 4 EUR |
| **TOTAL** | **34 EUR** | **80 EUR** |

### Pour 10 000 pieces :

| Scenario | Cout/piece |
|----------|-----------|
| Estimation basse | 28 EUR |
| Estimation haute | 60 EUR |
| **Moyenne** | **~40 EUR** |

---

# CONCLUSION

| Element | Choix retenu |
|---------|--------------|
| Procede primaire | Fonderie coquille par gravite |
| Materiau | Aluminium AS7G |
| Procedes secondaires | Tournage, fraisage, percage, rectification |
| Quantite rentable | >= 500 pieces |
| Cout estime | 40-50 EUR/piece (serie 1000-10000) |

### Avantages de la solution :
- Bon compromis cout/qualite
- Piece legere (aluminium)
- Resistant a la corrosion
- Usinage limite aux surfaces fonctionnelles

---

**Document realise dans le cadre du TD Design for Manufacturing - ESILV**
